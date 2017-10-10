
```
data(wheat_example)
Markers <- wheat_example$Markers
y <- wheat_example$y
cvSampleList <- cvSampleIndex(length(y),10,1)
## cross validation set
cvIdx <- 1
trainIdx <- cvSampleList[[cvIdx]]$trainIdx
testIdx <- cvSampleList[[cvIdx]]$testIdx
## set DeepGS paramaters
conv_kernel <- c("4*4","5*5") ## convolution kernels (fileter shape)
conv_num_filter <- c(20,28) ## number of filters
pool_act_type <- c("relu","relu") ## active function for next pool
pool_type <- c("max","max") ## Max pooling shape
pool_kernel <- c("2*2","2*2") ## pooling shape
pool_stride <- c("2*2","2*2") ## number of pool kernerls
fullayer_num_hidden <- c(56,1)
fullayer_act_type <- c("sigmoid")
cnnFrame <- list(conv_kernel =conv_kernel,conv_num_filter = conv_num_filter,
                 pool_act_type = pool_act_type,pool_type = pool_type,pool_kernel =pool_kernel,
                 pool_stride = pool_stride,fullayer_num_hidden= fullayer_num_hidden,
                 fullayer_act_type = fullayer_act_type)

trainGSmodel <- train_GSModel(trainMat = Markers[trainIdx,],trainPheno = y[trainIdx],
                              imageSize = "35*35", cnnFrame = cnnFrame,device_type = "cpu",
                              gpuNum = 1, eval_metric = "mae", num_round = 100000,
                              array_batch_size= 100,learning_rate = 0.01, momentum = 0,
                              wd = 0, randomseeds = 0,initializer_idx = 0.01)

predscores <- predict_GSModel(GSModel = trainGSmodel,testMat = Markers[testIdx,],imageSize = "35*35")
class(predscores)
class(y[testIdx])

cor.test(as.numeric(predscores), y[testIdx])
plot(as.numeric(predscores), y[testIdx])
meanNDCG(realScores = y[testIdx],predScores = as.numeric(predscores), topK = 10)

```
