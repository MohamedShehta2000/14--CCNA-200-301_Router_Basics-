# 14--CCNA-200-301_Router_Basics
# 1- What is the Router?

**الوظيفة:** عملية ربط بين الشبكات المختلفة.  
الـ **Router** يمنع مرور الـ **broadcast**.  
إذا كنت ترغب في زيادة عدد الواجهات (interfaces)، يمكنك استخدام **WIC**.  
أقل عدد من الواجهات له هو **2**.

## ما هي المكونات الداخلية للـ Router؟

1. **ROM** (Read-Only Memory):  
   - تعليمات لاختبار التشغيل (POST) للتحقق من الأجهزة، و**Bootstrap**، و**Mini-IOS**.

2. **Flash Memory:**  
   - تُحتفظ صور الـ **IOS** هنا.  
   - **Erasable Programmable ROM** (EPROM).  
   - قابل للبرمجة والمسح، والمحتويات تبقى عند إيقاف الطاقة أو إعادة التحميل.

3. **RAM** (Random Access Memory):  
   - **Routing Table**  
   - **Running Configuration**  
   - المحتويات تُفقد عند إعادة التشغيل.

4. **NVRAM** (Non-Volatile RAM):  
   - **Startup Configuration**  
   - المحتويات تُحتفظ بها عند إعادة التحميل.

## Router Power-On/Bootup Sequence

1. **Perform Power-On Self Test (POST):**  
   - **ROM** (check Hardware).
2. **Find the Cisco IOS Software:**  
   - تحديد الـ **IOS**.
3. **Load the Cisco IOS Software:**  
   - من الـ **Flash**، وللعلم يمكنك وضع أكثر من IOS ومن حقك اختيار IOS عند التشغيل.
4. **Find the Configuration:**  
   - هيبص على **NVRAM**.
5. **Load the Configuration.**
6. **Run the Configured Cisco IOS Software.**
