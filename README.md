**Outlines**

[MULTIPROCESSING](#One)

[TASK SCHEDULER](#Two)

**Multiprocessing** <a id="One"> </a>

This section introduces two method of multiprocessing

**Method1:Pool**

Sample code:

<p align="center">
  <img src="https://github.com/globalaiorg/ParallelProcessing-MemoryMgt-TaskScheduler/blob/main/image/Picture26.png">
</p>

Change the eval\_formula to the function you want to multiprocess, and change ecpression\_list as the input list for the function.

**Method 2:Process**

Sample code:

<p align="center">
  <img src="https://github.com/globalaiorg/ParallelProcessing-MemoryMgt-TaskScheduler/blob/main/image/Picture27.png">
</p>

Change the eval\_formula to the function you want to multiprocess, and change ecpression\_list as the input list for the function.

**TASK SCHEDULER** <a id="Two"> </a>

Task scheduler can be achieved on Linux by creating cron jobs.

Steps:

1. Open bash terminal in mac and type Crontab -e

<p align="center">
  <img src="https://github.com/globalaiorg/ParallelProcessing-MemoryMgt-TaskScheduler/blob/main/image/Picture28.png">
</p>

1. Hit &#39;i&#39; to put the editor into INSERT mode, and type the below cron expression in terminal:

DATE EXPRESSION cd PATH OF THE FILE YOU WANT TO SCHEDULED &amp;&amp; /Users/mac/anaconda3/bin/python FILE YOU WANT TO SCHEDULED

<p align="center">
  <img src="https://github.com/globalaiorg/ParallelProcessing-MemoryMgt-TaskScheduler/blob/main/image/Picture29.png">
</p>

For example: you want to run the process.py every day at 1:00 am. The process.py is under the path: &#39;/Users/mac/Desktop/SDG/automate\_MXUS\_Fiona&#39;.

Then the cron expression is:

0 1 \* \* \* cd /Users/mac/Desktop/SDG/automate\_MXUS\_Fiona &amp;&amp; /Users/mac/anaconda3/bin/python FILE YOU WANT TO SCHEDULED

Here:

cd /Users/mac/Desktop/SDG/automate\_MXUS\_Fiona is the path of the process.py. /Users/mac/anaconda3/bin/python is the location of the Python

How to set DATE EXPRESSION:

<p align="center">
  <img src="https://github.com/globalaiorg/ParallelProcessing-MemoryMgt-TaskScheduler/blob/main/image/Picture30.png">
</p>

1. Hit esc and then type : wq
