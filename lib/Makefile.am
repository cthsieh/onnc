INCDIR=../include/onnc

ONNC_SOURCES = \
	IRReader/ONNXReader.cpp \
	IR/ComputeRegOperand.cpp \
	IR/ComputeMemOperand.cpp \
	IR/ComputeOperand.cpp \
	IR/ComputeOperator.cpp \
	IR/ComputeGraph.cpp \
	IR/Module.cpp \
	IR/Dump.cpp \
	IR/Define.cpp \
	IR/ONNXNodeVisitor.cpp \
	IR/ONNXUtils.cpp \
	IR/Quadruple.cpp \
	IR/InsertionPoint.cpp \
	IR/IRBuilder.cpp \
	IR/ONNCModulePrinter.cpp \
	IR/CodeEmit.cpp \
	IR/Compute/Value.cpp \
	IR/Compute/Scalar.cpp \
	IR/Compute/Scale.cpp \
	IR/Compute/Tensor.cpp \
	IR/Compute/Use.cpp \
	IR/Compute/ATen.cpp \
	IR/Compute/Abs.cpp \
	IR/Compute/Acos.cpp \
	IR/Compute/Add.cpp \
	IR/Compute/And.cpp \
	IR/Compute/Affine.cpp \
	IR/Compute/Attributes.cpp \
	IR/Compute/AveragePool.cpp \
	IR/Compute/BatchNormalization.cpp \
	IR/Compute/Conv.cpp \
	IR/Compute/Concat.cpp \
	IR/Compute/Flatten.cpp \
	IR/Compute/Gemm.cpp \
	IR/Compute/GlobalAveragePool.cpp \
	IR/Compute/LRN.cpp \
	IR/Compute/LeakyRelu.cpp \
	IR/Compute/MaxPool.cpp \
	IR/Compute/Mul.cpp \
	IR/Compute/PRelu.cpp \
	IR/Compute/Upsample.cpp \
	IR/Compute/Relu.cpp \
	IR/Compute/Reshape.cpp \
	IR/Compute/Softmax.cpp \
	IR/Compute/Sum.cpp \
	IR/Compute/Split.cpp \
	IR/Compute/Transpose.cpp \
	IR/Compute/Xor.cpp \
	IR/Compute/Initializer.cpp \
	IR/Compute/InputOperator.cpp \
	IR/Compute/OutputOperator.cpp \
	IR/Tensor/InitializerProxy.cpp \
	Transforms/DeadNodeElimination.cpp \
	Transforms/RemoveTrainingNodes.cpp \
	Transforms/BookONNXGraphs.cpp \
	Transforms/GraphBuildingPass.cpp \
	Transforms/BuildInitializers.cpp \
	Transforms/BuildInputOperators.cpp \
	Transforms/BuildOutputOperators.cpp \
	Transforms/TensorSel.cpp \
	Transforms/TensorSel/Lower.cpp \
	Transforms/TensorSel/LowerRegistry.cpp \
	Transforms/TensorSel/DefaultAttributes.cpp \
	Transforms/TensorSel/AddLower.cpp \
	Transforms/TensorSel/AcosLower.cpp \
	Transforms/TensorSel/AbsLower.cpp \
	Transforms/TensorSel/AndLower.cpp \
	Transforms/TensorSel/ATenLower.cpp \
	Transforms/TensorSel/AffineLower.cpp \
	Transforms/TensorSel/ConvLower.cpp \
	Transforms/TensorSel/SoftmaxLower.cpp \
	Transforms/TensorSel/AveragePoolLower.cpp \
	Transforms/TensorSel/GemmLower.cpp \
	Transforms/TensorSel/GlobalAveragePoolLower.cpp \
	Transforms/TensorSel/LeakyReluLower.cpp \
	Transforms/TensorSel/MaxPoolLower.cpp \
	Transforms/TensorSel/MulLower.cpp \
	Transforms/TensorSel/SumLower.cpp \
	Transforms/TensorSel/BatchNormalizationLower.cpp \
	Transforms/TensorSel/LRNLower.cpp \
	Transforms/TensorSel/ReluLower.cpp \
	Transforms/TensorSel/PReluLower.cpp \
	Transforms/TensorSel/ConcatLower.cpp \
	Transforms/TensorSel/ReshapeLower.cpp \
	Transforms/TensorSel/TransposeLower.cpp \
	Transforms/TensorSel/UpsampleLower.cpp \
	Transforms/TensorSel/SplitLower.cpp \
	Transforms/TensorSel/FlattenLower.cpp \
	Transforms/TensorSel/XorLower.cpp \
	Core/PassRegistry.cpp \
	Core/PassManager.cpp \
	Core/PassInfo.cpp \
	Core/AnalysisUsage.cpp \
	Core/AnalysisResolver.cpp \
	Core/Pass.cpp \
	Core/ObjectWriter.cpp \
	Core/Application.cpp \
	Core/InitializePasses.cpp \
	Analysis/LivenessAnalysis.cpp \
	Analysis/MemoryAllocation.cpp \
	Analysis/NodeIRScheduler.cpp \
	Analysis/SplitNode.cpp \
	Analysis/UpdateGraphOutputSize.cpp \
	CodeGen/BuildMemOperand.cpp \
	CodeGen/FuseInplaceValue.cpp \
	CodeGen/LinearScanMemAlloc.cpp \
	CodeGen/LiveInterval.cpp \
	CodeGen/LiveIntervals.cpp \
	CodeGen/LiveValueMatrix.cpp \
	CodeGen/MemAllocData.cpp \
	CodeGen/SetMemOperand.cpp \
	CodeGen/SlotIndexes.cpp \
	ADT/PolicyNodeIterator.cpp \
	ADT/Digraph.cpp \
	ADT/Buffer.cpp \
	ADT/ConstBuffer.cpp \
	ADT/Any.cpp \
	ADT/Color.cpp \
	ADT/TypeTag.cpp \
	ADT/TopologyIterator.cpp \
	ADT/IList.cpp \
	ADT/IListIterator.cpp \
	ADT/Rope.cpp \
	ADT/StringList.cpp \
	ADT/StringRef.cpp \
	Support/Debug.cpp \
	Support/AsyncPipe.cpp \
	Support/CArgu.cpp \
	Support/CArguRef.cpp \
	Support/CEnv.cpp \
	Support/Directory.cpp \
	Support/DirIterator.cpp \
	Support/ErrorCode.cpp \
	Support/Environ.cpp \
	Support/Expansion.cpp \
	Support/Glob.cpp \
	Support/Host.cpp \
	Support/IOStream.cpp \
	Support/IndentOStreamBuf.cpp \
	Support/ManagedStatic.cpp \
	Support/MappedFileRegion.cpp \
	Support/MemoryMap.cpp \
	Support/Path.cpp \
	Support/Pipe.cpp \
	Support/FileHandle.cpp \
	Support/FileLock.cpp \
	Support/FileInfo.cpp \
	Support/FileStatus.cpp \
	Support/FileSystem.cpp \
	Support/Timer.cpp \
	Support/Random.cpp \
	Support/Readline.cpp \
	Support/linenoise.cpp \
	Support/SelfPipe.cpp \
	Support/Signal.cpp \
	Support/Unix/AsyncPipe.inc \
	Support/Unix/Expansion.inc \
	Support/Unix/Glob.inc \
	Support/Unix/Path.inc \
	Support/Unix/Pipe.inc \
	Support/Unix/FileSystem.inc \
	Support/Unix/Random.inc \
	Support/Unix/SelfPipe.inc \
	Support/Windows/Path.inc \
	Support/Windows/FileSystem.inc \
	Support/Dragon/Path.inc \
	Support/Dragon/FileSystem.inc \
	JSON/Array.cpp \
	JSON/Object.cpp \
	JSON/Value.cpp \
	JSON/JsonParser.ypp \
	JSON/JsonScanner.lpp \
	JSON/String.cpp \
	JSON/Notation.cpp \
	Diagnostic/Diagnostic.cpp \
	Diagnostic/DiagnosticInfoMap.cpp \
	Diagnostic/Engine.cpp \
	Diagnostic/GeneralOptions.cpp \
	Diagnostic/MsgHandler.cpp \
	Diagnostic/MsgHandling.cpp \
	Diagnostic/Policy.cpp \
	Diagnostic/Logger.cpp \
	Diagnostic/SysLog.cpp \
	Diagnostic/StreamLog.cpp \
	Config/AboutLicense.cpp \
	Config/AboutData.cpp \
	ONNXWrapper/ONNXWrapper.cpp \
	Option/Alias.cpp \
	Option/CommandLine.cpp \
	Option/OptDefs.cpp \
	Option/Option.cpp \
	Option/OptionPool.cpp \
	Option/OptParser.cpp \
	Runtime/onnc-runtime.c \
	Runtime/operator/abs.c \
	Runtime/operator/acos.c \
	Runtime/operator/add.c \
	Runtime/operator/affine.c \
	Runtime/operator/and.c \
	Runtime/operator/argmax.c \
	Runtime/operator/argmin.c \
	Runtime/operator/asin.c \
	Runtime/operator/atan.c \
	Runtime/operator/aten.c \
	Runtime/operator/averagepool.c \
	Runtime/operator/batchnormalization.c \
	Runtime/operator/cast.c \
	Runtime/operator/ceil.c \
	Runtime/operator/clip.c \
	Runtime/operator/concat.c \
	Runtime/operator/constant.c \
	Runtime/operator/constantfill.c \
	Runtime/operator/conv.c \
	Runtime/operator/convtranspose.c \
	Runtime/operator/cos.c \
	Runtime/operator/crop.c \
	Runtime/operator/depthtospace.c \
	Runtime/operator/div.c \
	Runtime/operator/dropout.c \
	Runtime/operator/elu.c \
	Runtime/operator/equal.c \
	Runtime/operator/exp.c \
	Runtime/operator/expand.c \
	Runtime/operator/flatten.c \
	Runtime/operator/floor.c \
	Runtime/operator/gather.c \
	Runtime/operator/gemm.c \
	Runtime/operator/giventensorfill.c \
	Runtime/operator/globalaveragepool.c \
	Runtime/operator/globallppool.c \
	Runtime/operator/globalmaxpool.c \
	Runtime/operator/greater.c \
	Runtime/operator/gru.c \
	Runtime/operator/gruunit.c \
	Runtime/operator/hardmax.c \
	Runtime/operator/hardsigmoid.c \
	Runtime/operator/identity.c \
	Runtime/operator/if.c \
	Runtime/operator/imagescaler.c \
	Runtime/operator/instancenormalization.c \
	Runtime/operator/leakyrelu.c \
	Runtime/operator/less.c \
	Runtime/operator/log.c \
	Runtime/operator/logsoftmax.c \
	Runtime/operator/loop.c \
	Runtime/operator/lpnormalization.c \
	Runtime/operator/lppool.c \
	Runtime/operator/lrn.c \
	Runtime/operator/lstm.c \
	Runtime/operator/matmul.c \
	Runtime/operator/max.c \
	Runtime/operator/maxpool.c \
	Runtime/operator/maxroipool.c \
	Runtime/operator/mean.c \
	Runtime/operator/meanvariancenormalization.c \
	Runtime/operator/min.c \
	Runtime/operator/mul.c \
	Runtime/operator/multinomial.c \
	Runtime/operator/neg.c \
	Runtime/operator/not.c \
	Runtime/operator/or.c \
	Runtime/operator/pad.c \
	Runtime/operator/parametricsoftplus.c \
	Runtime/operator/pow.c \
	Runtime/operator/prelu.c \
	Runtime/operator/randomnormal.c \
	Runtime/operator/randomnormallike.c \
	Runtime/operator/randomuniform.c \
	Runtime/operator/randomuniformlike.c \
	Runtime/operator/reciprocal.c \
	Runtime/operator/reducel1.c \
	Runtime/operator/reducel2.c \
	Runtime/operator/reducelogsum.c \
	Runtime/operator/reducelogsumexp.c \
	Runtime/operator/reducemax.c \
	Runtime/operator/reducemean.c \
	Runtime/operator/reducemin.c \
	Runtime/operator/reduceprod.c \
	Runtime/operator/reducesum.c \
	Runtime/operator/reducesumsquare.c \
	Runtime/operator/relu.c \
	Runtime/operator/reshape.c \
	Runtime/operator/rnn.c \
	Runtime/operator/scale.c \
	Runtime/operator/scaledtanh.c \
	Runtime/operator/scan.c \
	Runtime/operator/selu.c \
	Runtime/operator/shape.c \
	Runtime/operator/sigmoid.c \
	Runtime/operator/sin.c \
	Runtime/operator/size.c \
	Runtime/operator/slice.c \
	Runtime/operator/softmax.c \
	Runtime/operator/softplus.c \
	Runtime/operator/softsign.c \
	Runtime/operator/spacetodepth.c \
	Runtime/operator/split.c \
	Runtime/operator/sqrt.c \
	Runtime/operator/squeeze.c \
	Runtime/operator/sub.c \
	Runtime/operator/sum.c \
	Runtime/operator/tan.c \
	Runtime/operator/tanh.c \
	Runtime/operator/thresholdedrelu.c \
	Runtime/operator/tile.c \
	Runtime/operator/topk.c \
	Runtime/operator/transpose.c \
	Runtime/operator/unsqueeze.c \
	Runtime/operator/upsample.c \
	Runtime/operator/xor.c

ONNC_INCLUDES = @LIBONNC_INCLUDES@ @ONNX_INCLUDES@ -I${srcdir}/Target

ONNC_LIBS = @ONNX_LIBS@

ONNC_CPPFLAGS=-Waddress -Wchar-subscripts -Wcomment -Wformat -Wparentheses -Wreorder -Wreturn-type -Wsequence-point -Wstrict-aliasing -Wstrict-overflow=1 -Wswitch -Wtrigraphs -Wuninitialized -Wunknown-pragmas -Wunused-function -Wunused-label -Wunused-value -Wunused-variable -Wvolatile-register-var -Wno-return-stack-address

if ENABLE_DEBUG
ONNC_CPPFLAGS += -O0 -g3
endif

if ENABLE_OPTIMIZE
ONNC_CPPFLAGS += -O2 -DNDEBUG
endif

AM_CPPFLAGS = ${ONNC_INCLUDES} ${ONNC_CPPFLAGS}

AM_YFLAGS = -d
AM_LFLAGS = -olex.yy.c

#####################################
# Target-depednet files and settings
ONNC_TARGET_SOURCES = Target/Target.cpp \
	Target/TargetOptions.cpp \
	Target/TargetRegistry.cpp \
	Target/TargetStandardPasses.cpp \
	Target/NPUTargetBackend.cpp

if ENABLE_X86_TARGET
include $(srcdir)/Target/X86/Makefile.am
endif

# FIXME: embraced by flag?
include $(srcdir)/Target/Vanilla/Makefile.am

#####################################
# Build shared libraries
lib_LIBRARIES = libonnc.a

libonnc_a_SOURCES = ${ONNC_SOURCES} ${ONNC_TARGET_SOURCES}

libonnc_a_LIBADD = ${ONNC_LIBS}

if HAVE_PTHREADS
libonnc_a_LDFLAGS = -lpthread
endif
