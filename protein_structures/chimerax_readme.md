# general settings
- soft light
- shadows
- no silouette

# PKR  #6dc091
# K3L #786bac
# eIF2a gray

lighting depthCue False
surface resolution 5.5
preset ribbons # not cylinders
graphics silhouettes true
color :4/B #e1e1e1 # color PKR light gray
save file.png width 900 height 900 transparentBackground true supersample 10

---
# positive selection movie
show surface; hide cartoon
color /A #6dc091 surface #pkr
color /A:385,514,259,516,261,6,7,389,265,520,139,394,524,269,270,271,272,275,405,24,538,44,428,49,307,185,314,448,449,322,330,206,462,336,338,86,471,344,351,224,483,486,360,489,488,491,492,493,504,378,496,368,242,506,500,379,502,375,376,505,122,123,380,125,382,255  #E62929 surface # elde/roth pos-sele
color /B #786bac surface #k3
movie record supersample 3; crossfade; transparency /B:6-88 50 surface; wait 30; turn y 2 180; wait 180; crossfade; transparency /B:6-88 0 surface; wait 30; movie encode ~/Desktop/movies/pkr-k3_sele-fade_2.mp4

---
# general pkr-k3l-eif2a coloring
---
# color K3L with custom gradient

rainbow :4/A palette RdPu
rainbow :4/A palette Purples-5
rainbow :4/A palette BuPu
---
# pkr-kinase k3l, warm variant regions

color /A #d9d5d5; color /A:255-278 #ffb000; color /A:371-385 #fe6100; color /A:448-455 #dc267f; color /A:480-506 #7b215a; color /B #7368A7

style /A:466 sphere; show /A:466; color /A:446 #648fff

save /Users/chambersmj/Desktop/pkr-kinase_k3l_cartoon.png width 900 height 900 supersample 10 transparentBackground true
movie record supersample 3; wobble frames 80 cycle 80; wait; movie encode /Users/chambersmj/Desktop/pkr-kinase_k3l_wobble.mp4


---
pkr-kinase_k3l.pdb

preset cylinders
lignting soft

color /A #d9d5d5 cartoon
color /A:255-278 #ffb000 cartoon
color /A:371-385 #fe6100 cartoon
color /A:448-455 #dc267f cartoon
color /A:480-506 #7b215a cartoon
color /A #786bac

color :4/B #d9d5d5
color :4/B:255-278 #ffb000
color :4/B:371-385 #fe6100
color :4/B:448-455 #dc267f
color :4/B:480-506 #7b215a
color :4/A #786bac

color #1/A #d9d5d5
color #1/A:255-278 #ffb000
color #1/A:371-385 #fe6100
color #1/A:448-455 #dc267f
color /A:480-506 #7b215a
color #1/B #7368A7

style /A:466 sphere
show /A:466
color /A:446 #648fff

view name 1
turn y 180
view name 2

save /Users/chambersmj/Desktop/pkr-kinase_k3l_regions.png width 900 height 900 transparentBackground true supersample 4
movie record; wobble frames 80 cycle 80; wait; movie encode /Users/chambersmj/Desktop/wobble.mp4
---
# eif2a - PKR figure
color /B #d9d5d5; color /B:1-23 #ffb000; color /B:104-118 #fe6100; color /B:181-188 #dc267f; color /B:213-239 #785ef0; style /B:179 sphere; show /B:179; color /B:179 #648fff; color /C #7f8281


color /B #d9d5d5
color /B:1-23 #ffb000
color /B:104-118 #fe6100
color /B:181-188 #dc267f
color /B:213-239 #785ef0
style /B:179 sphere
show /B:179
color /B:179 #648fff
---
# make final slide
color /A #d9d5d5
color /A:255-272 #254397
color /A:273-278 #e92a2f
color /A:371-385 #254397
color /A:448-455 #e92a2f
color /A:480-506 #254397
color /B #e92a2f
movie record supersample 3; turn y 2 180; wait 180; movie encode ~/Desktop/pkr-k3l_final_cartoon.mp4 quality highest
---
color :2/B #786bac cartoon
color :2/A #6ec091 cartoon

style /A:466 sphere
show /A:466
color /A:446 #648fff


---

color :2/A #6ec091 surface
color :2/A #6ec091 cartoon
movie record; wobble frames 80 cycle 80; wait; movie encode /Users/chambersmj/Desktop/wobble_pkr_cartoon.mp4
save /Users/chambersmj/Desktop/pkr-full_cartoon.png width 900 height 900 transparentBackground true

hide :2/A surface
hide :2/A cartoon


show :2/B cartoon
color :2/B #786bac cartoon
save /Users/chambersmj/Desktop/k3l_cartoon.png width 900 height 900 transparentBackground true
movie record; wobble frames 80 cycle 80; wait; movie encode /Users/chambersmj/Desktop/wobble_k3l_cartoon.mp4


save /Users/chambersmj/Desktop/k3l_flat.png width 900 height 900 transparentBackground true


style :2/A:6,7,24,44,49,86,122,123,125,139,185,206,224,242,255,259,261,265,275,322,330,336,338,344,351,376,380,462,489,492,496,502,506,516,538 sphere

show :2/A:6,7,24,44,49,86,122,123,125,139,185,206,224,242,255,259,261,265,275,322,330,336,338,344,351,376,380,462,489,492,496,502,506,516,538

color :2/A:6,7,24,44,49,86,122,123,125,139,185,206,224,242,255,259,261,265,275,322,330,336,338,344,351,376,380,462,489,492,496,502,506,516,538 #e92a2f sphere


movie record supersample 3; turn y 2 180; wait 180; movie encode ~/Desktop/turn_pkr_cartoon.mp4 quality highest



6,
7,
24,
44,
49,
86,
122,
123,
125,
139,
185,
206,
224,
242,
255,
259,
261,
265,
275,
322,
330,
336,
338,
344,
351,
376,
380,
462,
489,
492,
496,
502,
506,
516,
538
