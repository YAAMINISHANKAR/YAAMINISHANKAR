import numpy as np
y = np.random.randint(1,20,(1,15))
print("Original Array:")
print(y)
y=np.reshape(y,(3,5))
print("Reshaped Array:\n",y)
for i in y:
  i[np.where(i==i.max())]=0
print("Maximum value replaced by 0 in each row are:\n",y)
