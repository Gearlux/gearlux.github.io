<a href="denoising.html"><img src="images/prev.png" width="40" height="40"></a>
<a href="index.html"><img src="images/back.png" width="40" height="40"></a>
<a href="Portfolio.html"><img src="images/next.png" width="40" height="40"></a>

# Personal Details 

<table class="tg">
<thead>
  <tr>
    <td class="tg-73oq"><a href="https://gearlux.github.io/"><img src="images/Profile.png" width="200" height="150"></a></td>
    <td class="tg-73oq"><a href="https://gearlux.github.io/">
                        <img src="images/qr-code.png" width="150" height="150"></a></td>
  </tr>
  <tr>
    <td class="tg-73oq">Name</td>
    <td class="tg-73oq">Behiels</td>
  </tr>
  <tr>
    <td class="tg-73oq">First name</td>
    <td class="tg-73oq">Gert</td>
  </tr>
  <tr>
    <td class="tg-73oq">Date of birth</td>
    <td class="tg-73oq">Feb 1972</td>
  </tr>
  <tr>
    <td class="tg-73oq">Place of residence</td>
    <td class="tg-73oq">Edegem - Belgium</td>
  </tr>
  <tr>
    <td class="tg-73oq">Nationality</td>
    <td class="tg-73oq">Belgian</td>
  </tr>
</thead>
</table>

# Portfolio

## Neural Network accelerator

### License plate recognition

Let's see how the NightVision network and the Denoising network can be used to optimize the license plate recognition of following image.

<img src="images/car.png"/>

Taken from an image with a longer exposure time, we know that the license plate is **5NON243**

<img src="images/licenseplate.png"/>

#### Car detection

The original image above is a 20MP image. Processing such an image requires a lot of processing power.
To recognize the license plate, we first detect the car on a low resolution image with the a `fasterrcnn_mobilenet_v3_large_320_fpn` network. We see that applying the NightVision network first, the confidence of car detection increases from **90%** to **97%**. 

<img src="images/original_car.png"/> <img src="images/nightvision_car.png"/>

If you look closely to images, you can also see that the bounding box of the car on the original image is a little bit too small, not completely including the license plate.

#### License plate recognition

Let's further extend the image processing pipeline. We use following  [license plate recognizer](https://platerecognizer.com/) to identify the license plate on the original and derived images.

<table class="tg">
<thead>
<tr> <td> <b>Original</b> </td> <td> <b>Denoised</b> </td> </tr> 
<tr> 
<td> <img src="images/lp_original.png"/> </td>
<td> <img src="images/lp_denoised.png"/> </td>
</tr>
<tr> <td><b>Night Vision</b></td> <td><b>Denoised + Night Vision</b></td> </tr>
<td> <img src="images/lp_nightvision.png"/> </td>
<td> <img src="images/lp_combined.png"/> </td>
</thead>
</table>

Construction of a good image processing pipeline, when done in the correct order, can improve the results of classification and detection networks.
