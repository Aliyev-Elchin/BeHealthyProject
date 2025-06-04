# 🥦 BeHealthy

## 📌 Layihə haqqında / About the Project

**AZ:**  
**BeHealthy** layihəsinin məqsədi istifadəçilərlə (user) dietoloqları bir platformada birləşdirmək, onların kalori və su ehtiyaclarını izləmək və onlara fərdi diet planları təqdim etməkdir. Platformada **Admin**, **İstifadəçi (User)** və **Dietoloq** olmaqla 3 əsas rol mövcuddur.

**EN:**  
**BeHealthy** is a web platform that connects users with dietitians, helps track daily calorie and water needs, and provides access to personalized diet plans. The system includes three main roles: **Admin**, **User**, and **Dietitian**.

---

## 🧑‍💼 Rol Sistemi / Role System

### 🔐 Admin
**AZ:**  
- Qeydiyyatdan keçən dietoloqları yoxlayır.  
- Onları təsdiqləyir və ya rədd edir.  

**EN:**  
- Reviews newly registered dietitians.  
- Approves or rejects their access to the system.

---

### 👤 İstifadəçi / User
**AZ:**  
- Qeydiyyatdan keçir, yaş, boy, çəki məlumatlarını daxil edir.  
- Gündəlik kalori və su ehtiyacını öyrənir.  
- Ninja Food API ilə qidaların kalorisini izləyir.  
- Dietoloqları izləyə və onlara abunə ola bilər.  
- Abunə olduqda planlara baxır və chat vasitəsilə ünsiyyət qurur.

**EN:**  
- Registers, enters age, height, and weight.  
- Learns daily calorie and water needs.  
- Tracks food calories using Ninja Food API.  
- Follows dietitians and can subscribe to them.  
- Gets access to diet plans and chat after subscription.

---

### 👩‍⚕️ Dietoloq / Dietitian
**AZ:**  
- Qeydiyyatdan keçəndə sertifikatlarını, təcrübə illərini və plan qiymətini daxil edir.  
- Admin təsdiqini gözləyir.  
- Təsdiqləndikdən sonra diet plan(lar)ı əlavə etməlidir.  
- Abunə olan istifadəçiləri görür və onlarla yazışa bilir.

**EN:**  
- Provides certificate info, years of experience, and plan pricing during registration.  
- Waits for admin approval.  
- After approval, must add at least one diet plan.  
- Can view and chat with subscribed users.

---

## 🛠 Texnologiyalar / Technologies

| Layer       | Texnologiya / Technology           |
|-------------|-------------------------------------|
| Frontend    | React.js                           |
| Backend     | ASP.NET Core Web API               |
| Verilənlər Bazası / Database | Microsoft SQL Server              |
| API         | [Ninja Food API](https://api-ninjas.com/api/nutrition) |
| Real-time Chat | SignalR                          |
| Arxitektura | Monolit (Monolithic Architecture)  |

---

## 🚀 Qurulum / Setup

### 📥 Layihəni klonla / Clone the repository
```bash
git clone https://github.com/Aliyev-Elchin/BeHealthyProject.git

1. `DataAccessLayer` layihəsini seç və terminaldan bu əmri icra et:
   cd DataAccessLayer
   dotnet ef database update

1. Select the `DataAccessLayer` project and run the following:
   cd DataAccessLayer
   dotnet ef database update

2. Backend işlək vəziyyətdə olmalıdır (dotnet run və ya Visual Studio ilə).

3. Swagger və ya Postman vasitəsilə bu endpoint-ə POST sorğusu göndər:
   /api/seed-foods

2. Backend must be running (via `dotnet run` or Visual Studio).

3. Send a POST request to the following endpoint via Swagger or Postman:
   /api/seed-foods

4. Frontend qovluğuna keç:
   cd client

5. Lazımi paketləri quraşdır:
   npm install

6. React tətbiqini işə sal:
   npm start

4. Navigate to the frontend folder:
   cd client

5. Install dependencies:
   npm install

6. Start the React app:
   npm start


