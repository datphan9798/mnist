# NEURAL NETWORK cho MNIST
## Muc dich
- Xay dung Neural Network (build from scratch) co 1 hidden layer cho bo du lieu MNIST
## Du lieu
- MNIST data set voi training-data-size = 42000
- Chia ra lam 2 data set: training data(37000) va validation data(5000)
## Kien truc Network
- Co 3 layer: 1 input layer(size = 784), 1 hidden layer(ReLU - size = 392), 1 output layer(Softmax - size = 10)
## Qua trinh huan luyen
- Ban dau su dung batch gradient decent de huan luyen voi batch_size = 16, learning-rate = 1, bo trong so mo hinh w1, w2 duoc khoi tao ngau nhien theo phan phoi Gaussian(voi mean = 0, variance = 1), b1, b2 khoi tao bang vecto 0. Sau 10 epoch, ket qua la accuracy_training = 9.65%, accuracy_validation = 9.98%
- Giu nguyen cac thong so tren, giam learning-rate tu 1 xuong 0.1, ket qua khong thay doi nhieu: accuracy_training = 9.94%, accuracy_validation = 10.18%
- Giu nguyen cac thong so tren, tang so node cua ReLU layer tu 392 len 784, ket qua khong thay doi nhieu: accuracy_training = 9.78%, accuracy_validation = 10.22%
- Giu nguyen cac thong so tren, tang so training-epoch tu 10 len 50, ket qua khong thay doi nhieu: accuracy_training = 9.98%, accuracy_validation = 9.62%
- Giu nguyen cac thong so tren, khoi tao w1, w2 bang ma tran 0, ket qua khong thay doi nhieu: accuracy_training = 10.43%, accuracy_validation = 10.78%
- Thay doi batch_size len thanh 37000(toan bo training data), moi lan training se cho toan bo du lieu vao network. Ket qua van khong thay doi nhieu: accuracy_training = 11.14%, accuracy_validation = 11.2%

Ket qua huan luyen cho thay trong qua trinh huan luyen, accuracy cua mo hinh khong thay doi nhieu, cho du thay doi nhieu gia tri tham so.
