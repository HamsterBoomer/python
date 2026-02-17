# Python
Remove Image Background using Python

# Code
pip install rembg pillow

from rembg import remove
from PIL import Image

input_path = 'pk.png'
output_path = 'pkjsp.png'

inp = Image.open(input_path)
output = remove(inp)
output.save(output_path)
Image.open(output_path).show()  # If you want to display it
