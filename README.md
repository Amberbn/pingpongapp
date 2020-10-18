1. Clone repository
git clone https://github.com/Amberbn/pingpongapp.git

2. Masuk ke directory 
cd pingpongapp

3. Jalankan perintah
kubectl create namespace dev
kubectl apply -f pingpong-deploy.yaml
kubectl apply -f pingpong-svc.yaml

4. Lihat status pod dan svc
kubectl get pods,svc -n dev 
#tunggu sampai status running
#untuk melihat aplikasi berjalan di port berapa bisa dilihat pada svc

5. Akses aplikasi di browser
http://ipserver:port/ping
