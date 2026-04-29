# App Translator - DevOps Project

פרויקט מקיף לבניית מערכת תרגום מבוססת מיקרו-שירותים (Microservices) בסביבת Kubernetes. המערכת מדגימה תהליכי CI/CD, ניהול קונטיינרים (Docker) ותזמור (Orchestration) בעזרת Minikube.

## ארכיטקטורת המערכת
המערכת מורכבת מ-4 שירותים מרכזיים:
1. **Frontend:** אתר סטטי מוגש ע"י Nginx.
2. **Backend:** שרת Node.js המנהל את הלוגיקה.
3. **Database:** מסד נתונים PostgreSQL לשמירת היסטוריית תרגומים.
4. **Translator:** שירות LibreTranslate לתרגום טקסטים.

## טכנולוגיות בשימוש
**Containerization:** Docker & Docker Compose
**Orchestration:** Kubernetes (Minikube)
**Runtime:** Node.js (Alpine)
**Database:** PostgreSQL (with Persistent Storage/PVC)
**Networking:** Nginx Ingress Controller

## הוראות הרצה (Kubernetes)
1. **הקמת הקלאסטר:** minikube start --nodes 3
2. **פריסת המערכת:** 
bash
   kubectl apply -f k8s/
