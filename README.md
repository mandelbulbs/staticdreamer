Dependencies

skimage

python-pip

numpy

scipy

tensorflow-gpu

cd staticdreamer

wget https://storage.googleapis.com/download.tensorflow.org/models/inception5h.zip

unzip -d model inception5h.zip


python staticdreamer.py --input_image input.png --output_image output.png --octaves 40 --iter 30 --layer mixed4d_3x3_bottleneck_pre_relu --channel 139 --tile_size 512 --model staticdreamer/inception5h/tensorflow_inception_graph.pb

python staticdreamer.py --input_image staticdreamer/inputs/content/eli3.jpg --output_image staticdreamer/results/eli3009.png --channel 9  --model staticdreamer/inception5h/tensorflow_inception_graph.pb --octaves 10 --iter 40 --octave_scale 1.6 --tile_size 512 --step_size 2 --layer mixed4c_pool_reduce



