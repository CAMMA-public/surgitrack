# Surgitrack: Fine-Grained Multi-Class Multi-Tool Tracking in Surgical Videos

*C.I. Nwoye and N. Padoy*

A publication of Elsevier Medical Image Analysis, 2025

- Accepted for IPCAI 2025 Long Abstract Presentation, Berlin Germany.


<br> 
<div align="justify"> 
    <b style="color:blue">Abstract:</b>
    Accurate tool tracking is essential for the success of computer-assisted intervention. Previous efforts often modeled tool trajectories rigidly, overlooking the dynamic nature of surgical procedures, especially tracking scenarios like out-of-body and out-of-camera views. Addressing this limitation, the new CholecTrack20 dataset provides detailed labels that account for multiple tool trajectories in three perspectives: (1) intraoperative, (2) intracorporeal, and (3) visibility, representing the different types of temporal duration of tool tracks. These fine-grained labels enhance tracking flexibility but also increase the task complexity. Re-identifying tools after occlusion or re-insertion into the body remains challenging due to high visual similarity, especially among tools of the same category. This work recognizes the critical role of the tool operators in distinguishing tool track instances, especially those belonging to the same tool category. The operators’ information are however not explicitly captured in surgical videos. We therefore propose SurgiTrack, a novel deep learning method that leverages YOLOv7 for precise tool detection and employs an attention mechanism to model the originating direction of the tools, as a proxy to their operators, for tool re-identification. To handle diverse tool trajectory perspectives, SurgiTrack employs a harmonizing bipartite matching graph, minimizing conflicts and ensuring accurate tool identity association. Experimental results on CholecTrack20 demonstrate SurgiTrack’s effectiveness, outperforming baselines and state-of-the-art methods with real-time inference capability. This work sets a new standard in surgical tool tracking, providing dynamic trajectories for more adaptable and precise assistance in minimally invasive surgeries.
</div>
<br />

<center><img src="flow.png" height="100%" width="auto" align="center"></center>

<br><br>
>> <a href="https://arxiv.org/abs/2405.20333" target="_blank" class="external-link button is-normal is-rounded is-dark"> <span class="icon"> <i class="ai ai-arxiv"></i> 📰</span> <span>arXiv Preprint</span> </a><br />
>> <a href="https://www.sciencedirect.com/science/article/pii/S1361841524003633#mmc1" target="_blank" class="external-link button is-normal is-rounded is-dark"> <span class="icon"> <i class="ai ai-arxiv"></i> 📰</span> <span>Medical Image Analysis Journal</span> </a>

<br>

## Results
#### Multi-Perspective Multi-Tool Tracking Results @ 25 FPS.
<center><img src="images/multip.png" height="100%" width="auto" align="center"></center>
<br />
#### Class-wise tracking accuracy and Impact of KB algorithm on state of the art models; [Intraoperative Perspective @ 25 FPS]
<center><img src="images/classw.png" height="100%" width="auto" align="center"></center>
<br />
#### Impact of Direction Estimation in Tracking Surgical Tools at Varying Video Sampling Rates (i.e. 1, 5, 25 frames per seconds FPS). A demonstration is included in the qualitative video.
<center><img src="images/fps.png" height="100%" width="auto" align="center"></center>
<br />
#### Performance Assessment of SurgiTrack Amidst Surgical Visual Challenges.
<center><img src="images/vchanllenge.png" height="100%" width="auto" align="center"></center>
<br />
#### Qualitative result of SurgiTrack in comparison with some existing methods.
<center><img src="images/demo1.png" height="100%" width="auto" align="center"></center>
<br />
#### Qualitative result of SurgiTrack in comparison with a state of the art method (BotSORT) on tracking across variable frame rates (1FPS, 5FPS
and 25FPS)
<center><img src="images/demo2.png" height="100%" width="auto" align="center"></center>


#### Video Demos


### CItation
-------------
<pre><code>@article{nwoye2024surgitrack,
  title={SurgiTrack: Fine-grained multi-class multi-tool tracking in surgical videos},
  author={Nwoye, Chinedu and Padoy, Nicolas},
  journal={Medical Image Analysis},
  pages={103438},
  year={2024},
  publisher={Elsevier}
}</code></pre>

<hr />
<br/>

**Code**: Coming soon !
