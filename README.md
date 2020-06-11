import numpy as np
from scipy import signal
import matplotlib.pyplot as plt

Fs = 20E3
f = 1E6
sample = Fs/f
print(sample)
x = np.arange(sample)

y = 100*np.sin(2 * np.pi * f * x / Fs)

plt.plot(x, y)
plt.show()
