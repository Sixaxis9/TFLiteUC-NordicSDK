PROJECT_NAME     := blinky_pca10040
TARGETS          := nrf52832_xxaa
OUTPUT_DIRECTORY := _build

SDK_ROOT := /Users/mg/Downloads/nRF5_17
PROJ_DIR := ..

$(OUTPUT_DIRECTORY)/nrf52832_xxaa.out: \
  LINKER_SCRIPT  := blinky_gcc_nrf52.ld

# Source files common to all targets
SRC_FILES += \
  $(SDK_ROOT)/modules/nrfx/mdk/gcc_startup_nrf52.S \
  $(SDK_ROOT)/components/libraries/log/src/nrf_log_frontend.c \
  $(SDK_ROOT)/components/libraries/log/src/nrf_log_str_formatter.c \
  $(SDK_ROOT)/components/boards/boards.c \
  $(SDK_ROOT)/components/libraries/util/app_error.c \
  $(SDK_ROOT)/components/libraries/util/app_error_handler_gcc.c \
  $(SDK_ROOT)/components/libraries/util/app_error_weak.c \
  $(SDK_ROOT)/components/libraries/util/app_util_platform.c \
  $(SDK_ROOT)/components/libraries/util/nrf_assert.c \
  $(SDK_ROOT)/components/libraries/atomic/nrf_atomic.c \
  $(SDK_ROOT)/components/libraries/balloc/nrf_balloc.c \
  $(SDK_ROOT)/external/fprintf/nrf_fprintf.c \
  $(SDK_ROOT)/external/fprintf/nrf_fprintf_format.c \
  $(SDK_ROOT)/components/libraries/memobj/nrf_memobj.c \
  $(SDK_ROOT)/components/libraries/ringbuf/nrf_ringbuf.c \
  $(SDK_ROOT)/components/libraries/strerror/nrf_strerror.c \
  $(SDK_ROOT)/modules/nrfx/soc/nrfx_atomic.c \
  $(SDK_ROOT)/modules/nrfx/mdk/system_nrf52.c \
  # $(PROJ_DIR)/main.c \




SRC_FILES += \
  $(PROJ_DIR)/tensorflow/lite/micro/all_ops_resolver.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/debug_log.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/flatbuffer_utils.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/memory_helpers.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/micro_allocator.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/micro_error_reporter.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/micro_graph.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/micro_interpreter.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/micro_profiler.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/micro_resource_variable.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/micro_string.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/micro_time.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/micro_utils.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/mock_micro_graph.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/recording_micro_allocator.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/recording_simple_memory_allocator.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/simple_memory_allocator.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/system_setup.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/test_helpers.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/memory_planner/greedy_memory_planner.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/memory_planner/linear_memory_planner.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/memory_planner/non_persistent_buffer_planner_shim.cc \
  $(PROJ_DIR)/tensorflow/lite/kernels/kernel_util.cc \
  $(PROJ_DIR)/tensorflow/lite/kernels/internal/reference/portable_tensor_utils.cc \
  $(PROJ_DIR)/tensorflow/lite/kernels/internal/quantization_util.cc \
  $(PROJ_DIR)/tensorflow/lite/core/api/error_reporter.cc \
  $(PROJ_DIR)/tensorflow/lite/core/api/tensor_utils.cc \
  $(PROJ_DIR)/tensorflow/lite/core/api/flatbuffer_conversions.cc \
  $(PROJ_DIR)/tensorflow/lite/core/api/op_resolver.cc \
  $(PROJ_DIR)/tensorflow/lite/schema/schema_utils.cc \
  $(PROJ_DIR)/tensorflow/lite/c/common.c   \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ActivationFunctions/arm_nn_activations_q15.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ActivationFunctions/arm_nn_activations_q7.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ActivationFunctions/arm_relu6_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ActivationFunctions/arm_relu_q15.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ActivationFunctions/arm_relu_q7.c             \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/BasicMathFunctions/arm_elementwise_add_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/BasicMathFunctions/arm_elementwise_mul_s8.c         \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConcatenationFunctions/arm_concatenation_s8_w.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConcatenationFunctions/arm_concatenation_s8_x.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConcatenationFunctions/arm_concatenation_s8_y.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConcatenationFunctions/arm_concatenation_s8_z.c           \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_1_x_n_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_1x1_HWC_q7_fast_nonsquare.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_1x1_s8_fast.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_HWC_q15_basic.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_HWC_q15_fast.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_HWC_q15_fast_nonsquare.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_HWC_q7_RGB.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_HWC_q7_basic.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_HWC_q7_basic_nonsquare.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_HWC_q7_fast.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_HWC_q7_fast_nonsquare.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_fast_s16.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_s16.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_wrapper_s16.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_convolve_wrapper_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_depthwise_conv_3x3_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_depthwise_conv_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_depthwise_conv_s8_opt.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_depthwise_conv_u8_basic_ver1.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_depthwise_conv_wrapper_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_depthwise_separable_conv_HWC_q7.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_depthwise_separable_conv_HWC_q7_nonsquare.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_nn_depthwise_conv_s8_core.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_nn_mat_mult_kernel_q7_q15.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_nn_mat_mult_kernel_q7_q15_reordered.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_nn_mat_mult_kernel_s8_s16.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_nn_mat_mult_kernel_s8_s16_reordered.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ConvolutionFunctions/arm_nn_mat_mult_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/FullyConnectedFunctions/arm_fully_connected_mat_q7_vec_q15.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/FullyConnectedFunctions/arm_fully_connected_mat_q7_vec_q15_opt.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/FullyConnectedFunctions/arm_fully_connected_q15.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/FullyConnectedFunctions/arm_fully_connected_q15_opt.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/FullyConnectedFunctions/arm_fully_connected_q7.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/FullyConnectedFunctions/arm_fully_connected_q7_opt.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/FullyConnectedFunctions/arm_fully_connected_s16.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/FullyConnectedFunctions/arm_fully_connected_s8.c                   \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_nn_accumulate_q7_to_q15.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_nn_add_q7.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_nn_depthwise_conv_nt_t_padded_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_nn_depthwise_conv_nt_t_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_nn_mat_mul_core_1x_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_nn_mat_mul_core_4x_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_nn_mat_mul_kernel_s16.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_nn_mat_mult_nt_t_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_nn_mult_q15.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_nn_mult_q7.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_nn_vec_mat_mult_t_s16.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_nn_vec_mat_mult_t_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_nn_vec_mat_mult_t_svdf_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_nntables.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_q7_to_q15_no_shift.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_q7_to_q15_reordered_no_shift.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_q7_to_q15_reordered_with_offset.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/NNSupportFunctions/arm_q7_to_q15_with_offset.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/PoolingFunctions/arm_avgpool_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/PoolingFunctions/arm_max_pool_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/PoolingFunctions/arm_pool_q7_HWC.c         \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/ReshapeFunctions/arm_reshape_s8.c     \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/SVDFunctions/arm_svdf_s8.c     \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/SoftmaxFunctions/arm_softmax_q15.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/SoftmaxFunctions/arm_softmax_q7.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/SoftmaxFunctions/arm_softmax_s8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/SoftmaxFunctions/arm_softmax_u8.c \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Source/SoftmaxFunctions/arm_softmax_with_batch_q7.c             \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/activations.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/activations_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/cmsis_nn/add.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/add_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/add_n.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/arg_min_max.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/assign_variable.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/batch_to_space_nd.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/call_once.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/cast.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/ceil.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/circular_buffer.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/circular_buffer_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/comparisons.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/concatenation.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/cmsis_nn/conv.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/conv_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/cumsum.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/depth_to_space.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/cmsis_nn/depthwise_conv.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/depthwise_conv_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/dequantize.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/dequantize_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/detection_postprocess.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/elementwise.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/elu.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/ethosu.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/exp.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/expand_dims.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/fill.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/floor.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/floor_div.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/floor_mod.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/cmsis_nn/fully_connected.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/fully_connected_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/gather.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/gather_nd.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/hard_swish.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/hard_swish_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/if.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/kernel_runner.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/kernel_util_micro.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/l2norm.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/l2_pool_2d.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/leaky_relu.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/leaky_relu_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/logical.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/logical_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/logistic.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/logistic_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/log_softmax.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/maximum_minimum.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/cmsis_nn/mul.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/mul_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/neg.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/pack.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/pad.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/cmsis_nn/pooling.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/pooling_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/prelu.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/prelu_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/quantize.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/quantize_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/read_variable.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/reduce.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/reshape.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/resize_bilinear.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/resize_nearest_neighbor.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/round.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/shape.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/slice.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/cmsis_nn/softmax.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/softmax_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/space_to_batch_nd.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/space_to_depth.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/split.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/split_v.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/squeeze.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/strided_slice.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/sub.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/sub_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/cmsis_nn/svdf.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/svdf_common.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/tanh.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/transpose.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/transpose_conv.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/unpack.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/var_handle.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/zeros_like.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/examples/hello_world/main.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/examples/hello_world/main_functions.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/examples/hello_world/output_handler.cc \
  $(PROJ_DIR)/tensorflow/lite/micro/examples/hello_world/constants.cc\
  $(PROJ_DIR)/tensorflow/lite/micro/examples/hello_world/hello_world_model_data.cc\
  $(PROJ_DIR)/tensorflow/lite/micro/examples/hello_world/model.cc\



# Include folders common to all targets
INC_FOLDERS += \
  $(SDK_ROOT)/components \
  $(SDK_ROOT)/modules/nrfx/mdk \
  $(PROJ_DIR) \
  $(SDK_ROOT)/components/libraries/strerror \
  $(SDK_ROOT)/components/toolchain/cmsis/include \
  $(SDK_ROOT)/components/libraries/util \
  $(SDK_ROOT)/components/libraries/balloc \
  $(SDK_ROOT)/components/libraries/ringbuf \
  $(SDK_ROOT)/modules/nrfx/hal \
  $(SDK_ROOT)/components/libraries/bsp \
  $(SDK_ROOT)/components/libraries/log \
  $(SDK_ROOT)/modules/nrfx \
  $(SDK_ROOT)/components/libraries/experimental_section_vars \
  $(SDK_ROOT)/components/libraries/delay \
  $(SDK_ROOT)/integration/nrfx \
  $(SDK_ROOT)/components/drivers_nrf/nrf_soc_nosd \
  $(SDK_ROOT)/components/libraries/atomic \
  $(SDK_ROOT)/components/boards \
  $(SDK_ROOT)/components/libraries/memobj \
  $(SDK_ROOT)/external/fprintf \
  $(SDK_ROOT)/components/libraries/log/src \

INC_FOLDERS += \
  $(PROJ_DIR)/ \
  $(PROJ_DIR)/tensorflow/lite \
  $(PROJ_DIR)/tensorflow/lite/micro/ \
  $(PROJ_DIR)/tensorflow/lite/micro/examples/hello_world \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels \
  $(PROJ_DIR)/tensorflow/lite/micro/kernels/cmsis_nn \
  $(PROJ_DIR)/tensorflow/lite/micro/memory_planner \
  $(PROJ_DIR)/tensorflow/lite/micro/testing \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/Core/Include \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/DSP/Include \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/DSP/Include/dsp \
  $(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Include \
  $(PROJ_DIR)/tensorflow/lite/kernels \
  $(PROJ_DIR)/tensorflow/lite/kernels/internal \
  $(PROJ_DIR)/tensorflow/lite/kernels/internal/optimized \
  $(PROJ_DIR)/tensorflow/lite/kernels/internal/reference \
  $(PROJ_DIR)/tensorflow/lite/kernels/internal/reference/integer_ops \
  $(PROJ_DIR)/tensorflow/lite/core/api \
  $(PROJ_DIR)/tensorflow/lite/c \
  $(PROJ_DIR)/tensorflow/lite/schema \
  $(PROJ_DIR)/third_party/gemmlowp \
  $(PROJ_DIR)/third_party/flatbuffers/include \
  $(PROJ_DIR)/third_party/ruy \


# Libraries common to all targets
LIB_FILES += \

# Optimization flags
OPT = -O3 -g3
# Uncomment the line below to enable link time optimization
#OPT += -flto

# C flags common to all targets
CFLAGS += $(OPT)
CFLAGS +=  -std=c11 -DTF_LITE_STATIC_MEMORY -DTF_LITE_DISABLE_X86_NEON -DCMSIS_NN -DTF_LITE_USE_CTIME -I. -I$(PROJ_DIR)/third_party/gemmlowp -I$(PROJ_DIR)/third_party/flatbuffers/include -I$(PROJ_DIR)/third_party/ruy -I$(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Include -I$(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/DSP/Include -I$(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/Core/Include -I$(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/DSP/Include -I$(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis -I$(PROJ_DIR)

# -Wimplicit-function-declaration -Werror -fno-unwind-tables -ffunction-sections -fdata-sections -fmessage-length=0 -Wsign-compare -Wdouble-promotion -Wshadow -Wunused-variable -Wmissing-field-initializers -Wunused-function -Wswitch -Wvla -Wall -Wextra -Wstrict-aliasing -Wno-unused-parameter

CFLAGS += -DBOARD_PCA10040
CFLAGS += -DBSP_DEFINES_ONLY
CFLAGS += -DCONFIG_GPIO_AS_PINRESET
CFLAGS += -DFLOAT_ABI_HARD
CFLAGS += -DNRF52
CFLAGS += -DNRF52832_XXAA
CFLAGS += -DNRF52_PAN_74
CFLAGS += -mcpu=cortex-m4
CFLAGS += -mthumb -mabi=aapcs
CFLAGS += -Wall -Werror
CFLAGS += -mfloat-abi=hard -mfpu=fpv4-sp-d16
# keep every function in a separate section, this allows linker to discard unused ones
CFLAGS += -ffunction-sections -fdata-sections -fno-strict-aliasing
CFLAGS += -fno-builtin -fshort-enums

# C++ flags common to all targets
CXXFLAGS += $(OPT)
CXXFLAGS += -std=c++11 -fno-rtti -fno-exceptions -DTF_LITE_STATIC_MEMORY -DTF_LITE_DISABLE_X86_NEON -DCMSIS_NN -DTF_LITE_USE_CTIME -I. -I$(PROJ_DIR) -I$(PROJ_DIR)/third_party/gemmlowp -I$(PROJ_DIR)/third_party/flatbuffers/include -I$(PROJ_DIR)/third_party/ruy -I$(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/NN/Include -I$(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/DSP/Include -I$(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/Core/Include -I$(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis/CMSIS/DSP/Include -I$(PROJ_DIR)/tensorflow/lite/micro/tools/make/downloads/cmsis

CXXFLAGS += -fno-rtti -fno-exceptions -fno-threadsafe-statics -Werror -fno-unwind-tables -ffunction-sections -fdata-sections -fmessage-length=0 -Wsign-compare -Wdouble-promotion -Wshadow -Wunused-variable -Wmissing-field-initializers -Wunused-function -Wswitch -Wvla -Wall -Wextra -Wstrict-aliasing -Wno-unused-parameter

CXXFLAGS += -DBOARD_PCA10056
CXXFLAGS += -DBSP_DEFINES_ONLY
CXXFLAGS += -DCONFIG_GPIO_AS_PINRESET
CXXFLAGS += -DFLOAT_ABI_HARD
CXXFLAGS += -DNRF52840_XXAA
CXXFLAGS += -mcpu=cortex-m4
CXXFLAGS += -mthumb -mabi=aapcs
CXXFLAGS += -Wall -Werror
CXXFLAGS += -mfloat-abi=hard -mfpu=fpv4-sp-d16
# keep every function in a separate section, this allows linker to discard unused ones
CXXFLAGS += -ffunction-sections -fdata-sections -fno-strict-aliasing
CXXFLAGS += -fno-builtin -fshort-enums



# Assembler flags common to all targets
ASMFLAGS += -g3
ASMFLAGS += -mcpu=cortex-m4
ASMFLAGS += -mthumb -mabi=aapcs
ASMFLAGS += -mfloat-abi=hard -mfpu=fpv4-sp-d16
ASMFLAGS += -DBOARD_PCA10040
ASMFLAGS += -DBSP_DEFINES_ONLY
ASMFLAGS += -DCONFIG_GPIO_AS_PINRESET
ASMFLAGS += -DFLOAT_ABI_HARD
ASMFLAGS += -DNRF52
ASMFLAGS += -DNRF52832_XXAA
ASMFLAGS += -DNRF52_PAN_74

# Linker flags
LDFLAGS += $(OPT)
LDFLAGS += -mthumb -mabi=aapcs -L$(SDK_ROOT)/modules/nrfx/mdk -T$(LINKER_SCRIPT)

LDFLAGS += -mcpu=cortex-m4
LDFLAGS += -mfloat-abi=hard -mfpu=fpv4-sp-d16
# let linker dump unused sections
LDFLAGS += -Wl,--gc-sections
# use newlib in nano version
LDFLAGS += --specs=nano.specs
# # TFLite
# LDFLAGS += -L/usr/local/opt/zlib/lib -lm

nrf52832_xxaa: CFLAGS += -D__HEAP_SIZE=8192
nrf52832_xxaa: CFLAGS += -D__STACK_SIZE=8192
nrf52832_xxaa: ASMFLAGS += -D__HEAP_SIZE=8192
nrf52832_xxaa: ASMFLAGS += -D__STACK_SIZE=8192

# Add standard libraries at the very end of the linker input, after all objects
# that may need symbols provided by these libraries.
LIB_FILES += -lc -lnosys -lm


.PHONY: default help

# Default target - first one defined
default: nrf52832_xxaa

# Print all targets that can be built
help:
	@echo following targets are available:
	@echo		nrf52832_xxaa
	@echo		sdk_config - starting external tool for editing sdk_config.h
	@echo		flash      - flashing binary

TEMPLATE_PATH := $(SDK_ROOT)/components/toolchain/gcc


include $(TEMPLATE_PATH)/Makefile.common

$(foreach target, $(TARGETS), $(call define_target, $(target)))

.PHONY: flash erase

# Flash the program
flash: default
	@echo Flashing: $(OUTPUT_DIRECTORY)/nrf52832_xxaa.hex
	nrfjprog -f nrf52 --program $(OUTPUT_DIRECTORY)/nrf52832_xxaa.hex --sectorerase
	nrfjprog -f nrf52 --reset

erase:
	nrfjprog -f nrf52 --eraseall

SDK_CONFIG_FILE := ../sdk_config.h
CMSIS_CONFIG_TOOL := $(SDK_ROOT)/external_tools/cmsisconfig/CMSIS_Configuration_Wizard.jar
sdk_config:
	java -jar $(CMSIS_CONFIG_TOOL) $(SDK_CONFIG_FILE)
