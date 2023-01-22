from scipy import misc
import matplotlib.pyplot as plt
ascent=misc.ascent()
plt.imshow(ascent)
print('\nOriginal image')
plt.show()

from scipy import misc
ascent=misc.ascent()
import matplotlib.pyplot as plt
plt.axis("off") #removes the axis and the ticks
plt.gray()
plt.imshow(ascent)
print('\nAfter convert the image to gray scale')
plt.show()



import numpy as np
from scipy import misc
import matplotlib.pyplot as plt
pic=misc.face() #reading an image from misc in scipy
plt.imshow(pic) #displaying the image using imshow() function in matplot
print('\nOriginal image')
plt.show()

import numpy as np
from scipy import misc
import matplotlib.pyplot as plt
pic=misc.face(gray=True) # getting the image in grayscale format
type(pic)
l=int(len(pic)/4)
crop_pic=pic[l:3*l,2*l:4*l] #taking only some values of the matrix pic
print('\nAfter crop and convert the image to gray scale')
plt.imshow(crop_pic,cmap='gray')


import numpy as np
from scipy import misc
import matplotlib.pyplot as plt
pic=misc.face() #reading an image from misc in scipy
plt.imshow(pic) #displaying the image using imshow() function in matplot
print('\nOriginal image')
plt.show()

from scipy import ndimage
rot_pic=ndimage.rotate(pic,45)
print('\nAfter rotate the image')
plt.imshow(rot_pic)


import numpy as np
from scipy import misc
import matplotlib.pyplot as plt
pic=misc.face() #reading an image from misc in scipy
plt.imshow(pic) #displaying the image using imshow() function in matplot
print('\nOriginal image')
plt.show()

import numpy as np
from scipy import ndimage
from scipy import misc
import matplotlib.pyplot as plt
pic=misc.face() #reading an image from misc in scipy
flip_pic=np.flipud(pic)
print('\nAfter flip the image')
plt.imshow(flip_pic)


import matplotlib.image as img
import matplotlib.pyplot as plt
img=img.imread(r'C:\Users\Likhith\Downloads\Chaplin.jpg')
plt.imshow(img)
print('\nOriginal image')
plt.show()

import matplotlib.image as img
import matplotlib.pyplot as plt
img=img.imread(r'C:\Users\Likhith\Downloads\Chaplin.jpg')
plt.imshow(img)
plt.axis("off") #removes the axis and the ticks
print('\nAfter removing the scale')
plt.show()