# ecse415-assignment-4-image-segmentation-using-k-means-solved
**TO GET THIS SOLUTION VISIT:** [ECSE415 Assignment 4-Image Segmentation using K-means Solved](https://www.ankitcodinghub.com/product/ecse415-assignment-4-image-segmentation-using-k-means-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;92538&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ECSE415 Assignment 4-Image Segmentation using K-means Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Image Segmentation using K-means

</div>
</div>
<div class="layoutArea">
<div class="column">
Implement K-means algorithm using only the numpy library. You can use opencv and matplotlib libraries only to read and display images. Apply K- means to the images ‘home’ and ‘flower’ shown in Figure 1. Try K=2 and K=3. Run the algorithm for 10 iterations and display the resulting segmented images in each case. (10 points)

1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
(a) (b)

Figure 1: Segment above images using K-means algorithm.

(a) (b) (c)

Figure 2: A pair of stereo images (a) left image (b) right image (c) disparity map (expected output).

2 Disparity

In this section, we will compute disparity map D from a pair of stereo images captured using parallel cameras. The images are shown in Figure 2(a) and 2(b). We will solve correspondence problem with the window search algorithm. Refer to slides 58-59 in Lecture 18 – Stereo Vision. Instead of searching for a matching window on the entire scanline, we will restrict the search on a small region on the scanline.

1. Extract a 5 × 5 window centered at each pixel-location (i, j)L in the left image. Let’s call these windows reference windows. (2 points)

2. For each reference window in the left image do the following.

<ol>
<li>(a) &nbsp;Ontherightscanline,createasearchregionboundedbypixel-locations (i,j−47)R and (i,j)R. Extract 5×5 windows centered at every pixel- location in this search region. (2 points)</li>
<li>(b) &nbsp;For few boarder pixel-locations either the reference window or the search region lie outside the boundary of the image. Set disparity
2
</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
(a) (b)

Figure 3: Input frames for optical flow computation. (a) frame1 (b) frame2.

</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
<div class="column">
D(i, j) = 48 for these pixel-locations. For the remaining locations do the following. (2 points)

(c) Compute sum-of-square-difference(SSD) between the windows in the search region and the reference window. (2 points)

(d) Find a location (i′,j′)R with minimum SSD and compute disparity D(i, j) = jL − j′R. (Note that 0 ≤ D(i, j) ≤ 47 as the search region contains 48 pixel-locations.) (1 point)

3. Display the final disparity map D with the cmap argument of plt.imshow set to ‘gray r’. The expected output is shown in Figure 2(c). (1 point)

Optical Flow

</div>
</div>
<div class="layoutArea">
<div class="column">
In this section, we will observe the effect of the window-size on the prediction accuracy of optical flow. The input frames are shown in Figure 3(a-b) and the ground-truth flow in given in ‘flow10.npz’ file. Read ground truth flow as follows: gt = np.load(‘flow10.npz’)[‘flow’]

<ol>
<li>Use calcOpticalFlowFarneback from OpenCV to compute optical flow between the input frames with the arguments set as follows. (2 points)
• flow=None, pyr scale=0.5, levels=3, iterations=3, poly n=5, poly sigma=1.2 and flags=0.

• Very winsize from 5 to 21 in the steps of 2.
</li>
<li>For each setting of winsize, measure mean squared error(MSE) between estimated optical flow and the ground truth optical flow. Plot MSE (y- axis) vs winsize (x-axis). (2 points)</li>
<li>Do you observe any trend in the plot above? Does the error increase or decrease with increasing window-size? Explain the effect of window-size on the prediction error. (2 points)</li>
</ol>
</div>
</div>
</div>
