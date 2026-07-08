# doggybag_fonts
In 2019, when I was just starting college, I threw together some handwritten fonts for fun and posted them on Twitter, completely royalty-free. I called them Elegantile and Anglerhand. They were received well on social media, so with the resulting boost in confidence I attempted to make a real, actual sans-serif font called Gunbangs. In 2021, I made an experimental font called LW90 where I used rounded lines to carve negative space out of squares. I still see all of these fonts out in the wild to this day. I've decided to upload my fonts and their respective source files to GitHub to allow people to use them and improve upon them.

## Methodology
I was inspired to make these by [Tom7](http://tom7.org/) and his [large collection of handwritten fonts](http://fonts.tom7.com/). As such I attempted to emulate his [font-making methodology](http://carnage-melon.tom7.org/makefont/) pretty closely.  
My workflow for all of these fonts was as follows:  
1. Design the actual glyphs in Adobe Flash. This wasn't the most ideal piece of software for the job, especially for my attempts at non-handwritten fonts, but it was the one I was most comfortable with.
2. Export all of the glyphs as .svg vector files.
3. Create a new font in FontForge, import the .svg files for each glyph.
4. With a convoluted workflow like this, the coordinates of the points that define the shape of the font would be affected by miniscule rounding errors. This has a pretty big impact on the hinting of the font at smaller scales. This wasn't really a problem for my handwritten fonts, but for something like LW90 where each glyph is created from a consistent base shape, this can be very noticeable.  
   ![image](https://github.com/gatorator/doggybag_fonts/assets/56567229/93f47b79-7c0b-410a-a3ab-5475204c5493)  
   Notice how the I, C, and K appear to be slightly higher than Q and U.  
   I didn't know anything about hinting while making these so I wasn't sure what to do about this at first, but luckily I was able to fix it by rounding every point in each glyph to the nearest hundredth in FontForge.  
   ![image](https://github.com/gatorator/doggybag_fonts/assets/56567229/2d4dbeb9-b996-4839-b7ec-493d76759c01)  
   Each glyph is now level!  
5. After importing, cleaning up, and kerning each glyph, I wrote the metadata and exported the font.  
**Now, you too can make your own fonts very inefficiently!**

## Source files
Each font's respective folder contains these files:
* **Font .fla** - the source Adobe Flash/Animate file for all the glyphs. I can't make any promises about how well-structured these files will be as I haven't touched them in years. 
* **Font .sfd** - the source FontForge file. This is where all the metadata resides.
* **Demo/preview .png** - a graphic I made that demonstrates the font being used.
* **Demo/preview .fla** - the source Adobe Flash/Animate file for the demonstration graphic. 

## Download/Releases
You can download all of the fonts in the releases tab. Each zip file contains the font in OpenType format along with its corresponding preview image.

## Previews
![demo1](https://github.com/gatorator/doggybag_fonts/assets/56567229/07643f26-86d8-4b17-bebb-a23dfe76c3cc)
![demo1 (2)](https://github.com/gatorator/doggybag_fonts/assets/56567229/4bb61eb6-3c19-4da5-a883-7db7c4b1ff68)
![demonstration](https://github.com/gatorator/doggybag_fonts/assets/56567229/3eb85d1e-ce00-40d3-9bac-588fd6a9fbb9)
![demonstration2](https://github.com/gatorator/doggybag_fonts/assets/56567229/3b282e5d-e9b2-442f-8e7d-00b7c07901e9)
