# Error_Ellipse_Calculation
## Purpose of this project

In this project, the user opens the *index.html* to upload a txt file containing the **X and Y coordinates** of the control points of the area of interest, their **variance** values in respect to the X and Y axis and their **covariance** values. The data txt file should have the following structure (Please also check the example of **DATA.txt**):

> **Approximate Coordinates**
>
> **POINT x y**
>
> *point_name x-coordinate y-coordinate*
>
> **Variance-Covariance**
>
> point_name
>
> **sigmax2** *σx²_value*  
> **sigmay2** *σy²_value*  
> **sigmaxy** *σxy_value*

## Output
The output of the projects are png images that depict the error ellipse for each of the control points based on their variance and covariance values. Example of a output png file:
<img src="docs/figs/Ellipse_A.png" alt="Description of the figure" width="800"/>
 
## Setup Instructions
Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
## Running the Code
Activate the uvicorn server through which backend.py is running:
 ```bash
   python uvicorn backend:app --reload
   ```



