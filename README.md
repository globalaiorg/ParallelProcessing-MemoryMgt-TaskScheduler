**Outlines**

MULTIPROCESSING

TASK SCHEDULER

**Multiprocessing**

This section introduces two method of multiprocessing

**Method1:Pool**

Sample code:

![](RackMultipart20210129-4-1gn3qlp_html_29a43618816999c8.png)

Change the eval\_formula to the function you want to multiprocess, and change ecpression\_list as the input list for the function.

**Method 2:Process**

Sample code:

![](RackMultipart20210129-4-1gn3qlp_html_6d6bd98c6d6b431f.png)

Change the eval\_formula to the function you want to multiprocess, and change ecpression\_list as the input list for the function.

**TASK SCHEDULER**

Task scheduler can be achieved on Linux by creating cron jobs.

Steps:

1. Open bash terminal in mac and type Crontab -e

![](RackMultipart20210129-4-1gn3qlp_html_d2068d448f62b6ec.png)

1. Hit &#39;i&#39; to put the editor into INSERT mode, and type the below cron expression in terminal:

DATE EXPRESSION cd PATH OF THE FILE YOU WANT TO SCHEDULED &amp;&amp; /Users/mac/anaconda3/bin/python FILE YOU WANT TO SCHEDULED

![](RackMultipart20210129-4-1gn3qlp_html_8378d86ae4f278c1.png)

For example: you want to run the process.py every day at 1:00 am. The process.py is under the path: &#39;/Users/mac/Desktop/SDG/automate\_MXUS\_Fiona&#39;.

Then the cron expression is:

0 1 \* \* \* cd /Users/mac/Desktop/SDG/automate\_MXUS\_Fiona &amp;&amp; /Users/mac/anaconda3/bin/python FILE YOU WANT TO SCHEDULED

Here:

cd /Users/mac/Desktop/SDG/automate\_MXUS\_Fiona is the path of the process.py. /Users/mac/anaconda3/bin/python is the location of the Python

How to set DATE EXPRESSION:

![](RackMultipart20210129-4-1gn3qlp_html_7a9ce7d8ef9def7c.png)

1. Hit esc and then type : wq
