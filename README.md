# HW4_Image_super_resolution
code for  Super Resolution Challenge. <br>

download the checkpoint for EDSR [EDSRorig_x3](https://drive.google.com/drive/u/2/folders/1bO4IDB241njwJPAnAQG6S7knGixDztaQ)

download the checkpoint for SWINIR [10000_E](https://drive.google.com/drive/u/2/folders/1bO4IDB241njwJPAnAQG6S7knGixDztaQ)

## Hardware
● Windows 10 <br>
● Intel(R) CORE i7 7th Gen @ 4.00GHz <br>
● NVIDIA GeForce GTX 1050 Ti <br>

You can see the detail in each folder.
Also put the test dataset in corresponding folder.

Run the code to get the reference by SWINIR.

    python main_test_swinir.py --task classical_sr --scale 3 --training_patch_size 48 --model_path ./10000_E.pth --folder_lq testsets/hw4/LR --folder_gt testsets/hw4/HR
    

Run the code to get the reference by EDSR.

    python main.py --upscale --scale 3 --image ../testing_lr_images/13.png
