
build anomaly detector where it detect anomaly on chip images data using autoencoder model after it succesfully trained on good images and test on defect chip images and it will finally find anomaly on images by giving red dot on images


#train model
python train.py --name type_1 --loss ssim_loss --im_resize 256 --patch_size 128 --z_dim 100 --grayscale --do_aug --epochs 300

#test model
python test.py --name type_1 --loss ssim_loss --im_resize 256 --patch_size 128 --z_dim 100 --grayscale
