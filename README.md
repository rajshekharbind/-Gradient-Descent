# -Gradient-Descent

📉 Gradient Descent from Scratch with Animations

This project demonstrates Gradient Descent for Linear Regression implemented from scratch using NumPy, along with animated visualizations to build strong intuition.

We cover:

Gradient Descent fundamentals

Step-by-step parameter updates

Gradient Descent animation for both m and b

Gradient Descent animation for only b

Loss (cost) curve animation

Mathematical intuition behind updates

📌 Topics Covered
1️⃣ Gradient Descent (Concept)

Gradient Descent is an iterative optimization algorithm used to minimize a loss function by updating parameters in the direction of the negative gradient.

2️⃣ Gradient Descent – Step by Step

At each epoch:

Compute predictions

Calculate loss (Mean Squared Error)

Compute gradients

Update parameters (m, b)

Repeat until convergence

3️⃣ Gradient Descent Animation (Both m and b)

Visualizes the optimization path on the loss surface

Shows how slope (m) and intercept (b) change together

Helps understand why gradients point downhill

4️⃣ Gradient Descent Animation (Only b)

Keeps slope (m) constant

Shows how changing intercept (b) affects loss

Ideal for beginners to understand 1D optimization

5️⃣ Gradient Descent Code from Scratch

No ML libraries like sklearn.linear_model are used for training.
Everything is implemented manually using NumPy.

🧠 Mathematical Intuition
Linear Model
𝑦
^
=
𝑚
𝑥
+
𝑏
y
^
	​

=mx+b
Loss Function (Mean Squared Error)
𝐽
(
𝑚
,
𝑏
)
=
1
𝑛
∑
𝑖
=
1
𝑛
(
𝑦
𝑖
−
(
𝑚
𝑥
𝑖
+
𝑏
)
)
2
J(m,b)=
n
1
	​

i=1
∑
n
	​

(y
i
	​

−(mx
i
	​

+b))
2
Gradients
∂
𝐽
∂
𝑚
=
−
2
𝑛
∑
𝑥
𝑖
(
𝑦
𝑖
−
𝑦
^
𝑖
)
∂m
∂J
	​

=−
n
2
	​

∑x
i
	​

(y
i
	​

−
y
^
	​

i
	​

)
∂
𝐽
∂
𝑏
=
−
2
𝑛
∑
(
𝑦
𝑖
−
𝑦
^
𝑖
)
∂b
∂J
	​

=−
n
2
	​

∑(y
i
	​

−
y
^
	​

i
	​

)
Update Rules
𝑚
=
𝑚
−
𝛼
∂
𝐽
∂
𝑚
m=m−α
∂m
∂J
	​

𝑏
=
𝑏
−
𝛼
∂
𝐽
∂
𝑏
b=b−α
∂b
∂J
	​


where α is the learning rate.

🎥 Visualizations Included

✔ Regression line updating per epoch
✔ Loss vs Epoch animation
✔ Optimization path on contour plot
✔ GIF animations using matplotlib.animation

🛠 Dependencies & Installation
✅ Required Libraries
pip install numpy matplotlib scikit-learn pillow ipython

📦 Dependency Purpose
Library	Usage
numpy	Numerical computation
matplotlib	Plotting & animation
scikit-learn	Dataset generation only
pillow	Save GIF animations
ipython	Animation display
▶ How to Run

Clone the repository

git clone <your-repo-url>
cd gradient-descent-animation


Open Jupyter Notebook

jupyter notebook


Run notebooks in order:

01_gradient_descent_from_scratch.ipynb

02_gradient_descent_only_b.ipynb

03_gradient_descent_m_and_b_animation.ipynb

04_loss_curve_animation.ipynb

📂 Project Structure
gradient-descent-animation/
│
├── data/
│   └── synthetic_data.py
│
├── notebooks/
│   ├── gradient_descent_step_by_step.ipynb
│   ├── gradient_descent_only_b.ipynb
│   ├── gradient_descent_m_b_animation.ipynb
│   └── loss_curve_animation.ipynb
│
├── outputs/
│   ├── animation1.gif
│   ├── animation2.gif
│
├── README.md

🎯 Learning Outcomes

After completing this project, you will:

Understand why gradient descent works

Visualize optimization in 1D and 2D

Implement gradient descent without ML libraries

Debug common animation & indexing errors

Build strong ML fundamentals

📚 References

Andrew Ng – Machine Learning (Coursera)

Stanford CS229 Notes

Deep Learning Book – Ian Goodfellow

Matplotlib Animation Docs

NumPy Documentation
