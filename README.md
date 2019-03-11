# vision
Codes & papers about vision






s = glob.glob("./hima/*00.png")

for f in s:
    i = (re.findall('_\d+', f))
    f[44:52]
    print(f[48:50])
    print(i)

# ch09,14의 폴더를 복사하고 각각의 폴더에서 아래의 코드를 이용해 필요한 사진만 
import os
import glob
import re
s = glob.glob("./hima/*00.png")
for f in s:
    i = (re.findall('_\d+', f))
    if  ('19'or'20'or'21'or'22'or'23'or'00'or'01'or'02'or'03'or'04'or'05') in f[48:50]:
        os.remove(f)
        print("file name[" + f + "]")
