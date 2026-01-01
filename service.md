apiVersion: v1     #גרסה
kind: Service      #סוג יאמל
metadata:
  name: map-service
spec:
  selector:
    app: map        #לפי איזה תגית הוא יהיה מחובר אליו
  ports:
  - protocol: TCP
    port: 8080       #הפורט הפנימי
    targetPort: 8080     #הפורט החיצוני