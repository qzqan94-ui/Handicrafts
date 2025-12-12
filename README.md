<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
 <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">

<title>استمارة الحرف اليدوية</title>
<style>
  body {
    font-family: "Tahoma", sans-serif;
    margin: 0;
    padding: 20px;
    background: #fff;
}


  .form-container {
    width: 98%;
    margin: 10px auto;
    border: 1px solid #999;
    padding: 10px;
  }

  table {
    width: 100%;
    border-collapse: collapse;
    text-align: center;
    font-size: 14px;
  }

  td, th {
    border: 1px solid #999;
    padding: 6px;
  }

  .header-logo {
    width: 140px;
  }

  .section-title {
    background: #eee;
    font-weight: bold;
  }

  .side-title {
    background: #e5e5e5;
    min-width: 20px;
    font-weight: bold;
  }

  .no-border {
    border: none !important;
  }
  body {
    display: flex;
    justify-content: flex-start; /* يجعل المحتوى على اليسار */
    align-items: flex-start;     /* من الأعلى */
    padding: 20px;
  }
  table {
    border-collapse: collapse;
  }
  td {
    padding: 5px 0; /* مسافة بين الصفوف */
  }
  input {
    width: 150px; /* عرض صندوق النص */
  }
/* إجبار جدول معلومات أساسية على التصغير مع الشاشة */
.basic-info-table {
  width: 100%;
  table-layout: fixed;   /* يسمح للجدول بالتصغير */
}

.basic-info-table td,
.basic-info-table th {
  white-space: nowrap;   /* يمنع تكسير النص */
  overflow: hidden;
  text-overflow: ellipsis;
}

.basic-info-table input {
  width: 100%;           /* يجعل الحقول تتقلص تلقائياً */
  box-sizing: border-box;
}
/* تصغير الخط للجوال فقط */
@media (max-width: 768px) {
  .basic-info-table td,
  .basic-info-table th {
    font-size: 7px;   /* حجم أصغر */
    padding: 4px;      /* تقليل المسافات */
  }

  .basic-info-table input {
    font-size: 12px;
    padding: 4px;
  }
}

/* تصغير أكبر للشاشات الصغيرة جدًا */
@media (max-width: 480px) {
  .basic-info-table td,
  .basic-info-table th {
    font-size: 11px;
    padding: 3px;
  }

  .basic-info-table input {
    font-size: 11px;
    padding: 3px;
  }
}
.compact {
  float: left;
  margin-top: 5px; /* احتفظ بالمسافة العلوية */
}
.compact {
  display: block;
  width: auto;
  margin-inline-start: 0;   /* بداية السطر (في RTL هذه هي اليمين) */
  margin-inline-end: auto;  /* يجعل العنصر يلصق بداية المحور */
  margin-top: 9px;
    font-size: 7px;  /* صغّر الرقم حسب رغبتك */

}
.basic-info-table .header-row td {
  background-color: #e5e5e5; /* رمادي رصاصي */
  font-weight: bold;          /* اختياري */
  color: #000;                /* لون النص */
}

.vertical-header{writing-mode:vertical-rl;}
input[type="checkbox"] {
    margin:0;
    padding:0;
}
td input[type="checkbox"] {
    float: right;
    margin-left: 4px;
}
td {
  position: relative;
  padding-right: 0 !important; /* إزالة المسافة من اليمين */
}

td input[type="checkbox"] {
  position: absolute;
  right: -65px;                /* الصندوق يلتصق تمامًا باليمين */
  top: 50%;
  transform: translateY(-50%);
  margin: 0;
}
.craft-wrapper {
  width: 100%;
  overflow-x: auto;   /* يسمح بتمرير أفقي */
}

.craft-table {
  width: 100%;
  border-collapse: collapse;
}

.craft-table td,
.craft-table th {
  white-space: nowrap;   /* يمنع تكسر النص */
  padding: 5px;
  font-size: 14px;
}

/* للجوال */
@media (max-width: 768px) {
  .craft-table td,
  .craft-table th {
    font-size: 10px;
    padding: 3px;
  }
}

</style>
</head>
<body>

<div class="form-container">

  <!-- رأس الاستمارة -->
  <table>
    <tr>
      <td rowspan="2" style="border:none; width:130px;">
    <img src="Logo.jpg" alt="Logo" style="width:200px; height:auto;">
</td>

      <td class="no-border" style="font-size:20px; font-weight:bold;">استمارة الحرف اليدوية</td>
      <td rowspan="2" class="no-border" style="width:130px;"></td>
    </tr>
    <tr></tr>
  </table>
  <hr style="margin:12px 0; border-color:#ddd;">

  <!-- مثال لجدول صغير مدمج (يُصغر حسب المحتوى) -->
  <table class="compact" style="margin-top:8px;">
    <tr class="side-title">
      <td>التاريخ</td>
    
      <td><input type="text"></td>
    </tr>
    <tr class="side-title">
      <td>رقم الزيارة</td>

      <td><input type="text"></td>
    </tr>
  </table>


  <!-- العنوان الجانبي + البيانات الأساسية -->
  <div>
  <table class="basic-info-table">

   <tr class="header-row">
  <td rowspan="4" class= vertical-header>معلومات أساسية</td>
  <td>اسم منفذ البيع</td>
  <td>اسم المالك</td>
  <td> السجل المدني</td>
  <td>السجل التجاري</td>
  <td>رقم الهاتف</td>
</tr>

    <tr>
      <td><input type="text"></td>
      <td><input type="text"></td>
      <td><input type="text"></td>
      <td><input type="text"></td>
      <td><input type="text"></td>
    </tr>
    <tr class="header-row"></trclass>
        <td>اسم السوق </td>
         <td>المحافظة</td>
         <td>المنطقة</td>
         <td>الفرع</td>
      <td>رقم رخصة حرفي</td>
    </tr>
    <tr>
      <td><input type="text"></td>
      <td><input type="text"></td>
      <td><input type="text"></td>
      <td><input type="text"></td>
      <td><input type="text"></td>
    </tr>
  </table>
<!-- جدول الحرف اليدوية -->
<h3 style="margin-top:25px; text-align:center;">الحرف اليدوية</h3>
<div class="craft-wrapper">
<table class="craft-table">
    ...

       <th rowspan="20" class="vertical-header" style="background:#e5e5e5; color:#000;">
    الحرفة
</th>

               
        <th style="background:#e5e5e5; color:#000; font-weight:bold;">
    الحرفة
</th>

        
     <td><input type="checkbox" style="margin:0 2px 0 0;">النقش والرسومات</td>

        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>
<th rowspan="2" style="background:#e5e5e5; color:#000; font-weight:bold;">
    الحرفة
</th>

        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>

        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
<td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>  
  <th rowspan="2" style="background:#e5e5e5; color:#000; font-weight:bold;">
    الحرفة
</th>

        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>لرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>

        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>
        
        
        <th rowspan="2" style="background:#e5e5e5; color:#000; font-weight:bold;">
    الحرفة
</th>

        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>

        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>
     <th rowspan="2" style="background:#e5e5e5; color:#000; font-weight:bold;">
    الحرفة
</th>

        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>

        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>     
        
     <th rowspan="2" style="background:#e5e5e5; color:#000; font-weight:bold;">
    الحرفة
</th>

        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>

        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>        
        <th style="background:#e5e5e5; color:#000; font-weight:bold;">
    الحرفة
</th>
        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>
 <th style="background:#e5e5e5; color:#000; font-weight:bold;">
    الحرفة
</th>
        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>
        
        
        <th style="background:#e5e5e5; color:#000; font-weight:bold;">
    الحرفة
</th>
        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>
        
        <th style="background:#e5e5e5; color:#000; font-weight:bold;">
    الحرفة
</th>
        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>
 <th style="background:#e5e5e5; color:#000; font-weight:bold;">
    الحرفة
</th>
        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>
        
        
      
       <th rowspan="2" style="background:#e5e5e5; color:#000; font-weight:bold;">
    الحرفة
</th>

        
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>
        
        

 <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
        <td>النقش والرسومات
        <input type="checkbox"></td>
         <td>النقش والرسومات
        <input type="checkbox"></td>
    </tr>

</table>


</div>
</div>
</div>

<script>
// مساحة للسكربت إن احتجت
</script>

</body>
</html>
