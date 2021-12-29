### Terminal_Tips
This repository contain tips and tricks for Linux terminal 

## Tip 1: 
  اذا كان عندك ملف فاستا يحتوي على اكثر من سيكونس وتحتاج تعرف كم طول كل واحد منهم، استخدم هذا الامر من في التيرمينال 

```
  awk 'BEGIN{FS="[>]"} /^>/{val=$2;next} {print val,length($0)}' input.fasta > output.length.txt
```

## Tip 2:
  اذا كنت بحاجة إلى كتابة امر في عدة أسطر، استخدم علامة \ واذا كنت تحتاج تنفذ اكثر من امر استخدم علامة && او علامة ;
 
  Example: 
  ```

  mkdir /home/data/Experment && \
  cd /home/data/Experment ; \
  touch notes.txt"
  ```

  
## Tip 3: 
  الأمر touch يستخدم لتحديث تاريخ الملف (من اسمه)، ولكن لو تم استخدامه على ملف غير موجود، راح ينشئ ملف جديد:
  ```
   touch /home/notes.txt
  ```
