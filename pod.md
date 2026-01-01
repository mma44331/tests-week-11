apiVersion: v1  #איזה גרסה
kind: Pod #סןג יאמל
metadata:
  name: map
  labels:
    app: map   #תגית שלפי יתקשרו איתו

spec:
  containers:    #קונטיינרים
  - name: map
    image: my-app:latest       #ירוץ עם ה image שלי החדש
    ports:
    - containerPort: 8080