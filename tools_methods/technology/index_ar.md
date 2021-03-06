---
layout: contentwithsiblings.html
title: "التقنيات"
date: 2017-11-27
desc: "أدوات ومصادر مفتوحة المصدر للتحقيقات"
image: /assets/technology/technologyyy.jpg
---

يُحدّد الأرشيف السوري، يجمع، ويحافظ على المحتوى الرقمي في صيغ متنوّعة من مصادر ومنصات مُتعدّدة. يُخزّن المحتوى في قاعدة بيانات مركزية بحيث يتم الوصول إليه من قبل أدواتنا مفتوحة المصدر لإجراء عمليات البحث، الاستقصاء، التحقّق، التصنيف والتوسّع. وبدلًا من تطوير حلول تقنية جاهزة على التحديات المتعلّقة بالمحتوى والتي يواجهها فريق الأرشيف السوري، فإننا اتخذنا نهجًا مُتمركز حول المستخدم لتطوير أو المساهمة في حلول مُخصّصة مفتوحة المصدر (على سبيل المثال [Sugarcube](https://gitlab.com/sucarcube)) بما يسمح لفريقنا من المُحقّقين العمل بشكل متعاون على مسار البيانات لدينا.

## نظرة عامة

![tech diagram](/assets/technology/techdiagram.jpg)

### المصادر والجمع

تُجمع قاعدة بياناتنا من قائمة مصادر تُغطّي أنواع عديدة من المنصات. نحن نجمع البيانات والمنشورات بشكل يومي من هذه المصادر. أنواع المصادر تشمل قنوات الشبكات الاجتماعية (تويتر، فيس بوك، يوتيوب)، الملفات المُحمّلة (فيديوهات، ملفات pdf)، ومجموعات البيانات التي أُرسلت لنا في سياق التعاون. كما يتم تعقّب التغييرات التي تتطرأ على هذه المصادر، بما يعني أن جميع النُسخ المُعدّلة من موادها محفوظة لدينا.

### عمليات التجيهز / مسار البيانات

كل وحدة Unit من البيانات في قاعدة البيانات لدينا تمر من خلال "مسار أنابيب البيانات" لدينا، في هذا المسار نقوم بتحديد اللغة، نُوحّد صيغة البيانات (مع الاحتفاظ على الصيغة الأصلية كذلك)، بالإضافة إلى إجراء عمليات أخرى بغرض تجهيز البيانات. كما نقوم بالتقاط وتنزيل صفحة الويب التي تلقينا المعلومات منها.

### الختم الزمني

نقوم بتوليد قيم التجزئة (الهاش) وفق خوارزميتي `md5` & `sha256` لجميع الملفات في قاعدة البيانات لدينا. بالإضافة إلى ختم زمني من خلال الأداة [Enigio Time](https://www.enigio.com/).


### أدوات التحقّق

نستخدم مجموعة متنوعة من الأدوات للتحقّق من الوحدات التي حصلنا عليها. وباعتبار أنه لا يُمكن للبيانات أن تُفقد، يمكننا استخدام مجموعة متنوعة من الأدوات لإضافة أو تحرير حقول جديدة من المعلومات على تلك البيانات ثم دمجهم ثانيةَ مع قاعدة بياناتنا المركزية.

حاليًا، نقوم باستخدام مزيج من  [Google Sheets](https://gitlab.com/sugarcube/sugarcube/tree/master/packages/plugin-googlesheets/) وَ [Check](https://meedan.com/en/check/).

## حزمة التطوير

نعتمد التقنيات التالية في حزمتنا للتطوير:

debian / nodejs / sugarcube / python / mongodb / nginx / react

موقعنا هو عبارة عن ملفات html صرفة. استخدمنا react لقاعدة البيانات، ونقوم بالاستدعاء من خلال API.

## روابط

[الأرشيف السوري على غيتهاب](https://github.com/syrianarchive)

[Sugarcube - خط البيانات](https://gitlab.com/sugarcube)

## تواصل معنا

[تواصل معنا](mailto:niko@syrianarchive.org) لنرى كيف يمكننا مساعدتك في العمل على مشروعك.
