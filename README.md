## **Stochastic Gradient Descent**
- Here, In this repository, I have tried the Simple Impementation of PyTorch in building **Stochastic Gradient Descent from Scratch**.
   
- In addition, I have tried to present the example of creating animation using Matplotlib which was quite interesting for me at first. Here,
```javascript
from matplotlib import animation, rc
rc('animation', html='jshtml')

a = nn.Parameter(tensor(-1., 1))

fig = plt.figure()
plt.scatter(x[:, 0], y, c="orange")
line, = plt.plot(x[:, 0], x@a.detach())
plt.close()

def animate(i):
  update()
  line.set_ydata(x@a.detach())
  return line,

animation.FuncAnimation(fig, animate, np.arange(1, 200), interval=20)
```
