# Error_Ellipse_Calculation
## Purpose of this project

In this project, the user opens *index.html* to upload a `.txt` file containing the **X and Y coordinates** of the control points of the area of interest, along with their **variance** values with respect to the X and Y axes and their **covariance** values. The input `.txt` file should follow the structure below (see also the example in **DATA.txt**):

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
The output of the project consists of PNG images that depict the error ellipse for each control point based on its variance and covariance values. Example of an output PNG file:
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



