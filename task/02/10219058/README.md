# 10219058
Isep Robi Awaludin


## materi sebelumnya
+ Rekursif
+ Metode Euler
+ Metode Runge-Kutta orde 4
+ Penyelesaian persamaan ODE
+ Predator Prey
+ Heat difussion model
+ Osilasi Harmonis Sederhana
+ Osilasi Teredam 
+ Osilasi Terkopel
+ monte carlo
+ Fourier transform



## materi paling menarik
+ Rekursif. dapat membuat bentuk fisis dari suatu benda seperti snowflek. menarik karena dapat membuat snowflake yang lumayan rumit


## materi paling membosankan
+ Heat diffusion. karena untuk pembuatan code nya menggunakan penulisan matriks yang cukup melelahkan


## materi yang sudah dipami
+ dari semua materi yang disampaikan, saya lebih memahami metode euler dan runge kutta orde 4, serta penerapannya seperti pada fenomena osilasi bandul


## materi yang belum dipahami
+ cara menerapkan metode monte carlo


## contoh program
+ Buat suatu contoh program dalam Python dan sertakan di sini dengan hasil keluarnnya.

```python
# contoh program python
import math 
import numpy as np
import matplotlib.pyplot as plt

#Deklarasi fungsi

#Deklarasi variabel
r=1
l=10
c=10


#set parameter
n=10000
dt=0.01

#bikin array
t=[0 for i in range(1,n+1)]
v=[10 for i in range(1,n+1)]
u=[0.5 for i in range(1,n+1)]

#main code
for i in range(1,n-1):
    t[i+1]=t[i]+dt
    v[i+1]=v[i]+dt*u[i]-0.5*(dt**2)*((r/l)*u[i]+(1/l*c)*v[i])
    u[i+1]=u[i]-dt*((r/l)*u[i]+(1/l*c)*v[i])+0.5*(dt**2)*((r**2/l**2)*u[i]+(r/(c*l**2))*v[i]-(1/l*c)*u[i])

#linear space
T=np.linspace(0,99.98,10000)
V=10*np.exp(-2*T)+5*np.exp(-2*T)


#plot
plt.plot(T,V,t,v)
plt.show()
```

Hasilnya adalah

<a href="https://ibb.co/h1mhpCt"><img src="https://i.ibb.co/dJ51n7z/Hasil.jpg" alt="Hasil" border="0"></a>


## cara perkuliahan
+ Menurut saya perkuliahan sebaiknya selalu dilakukan di labcom, supaya mahasiswa bisa secara langsung melakukan simulasi materi yang disampaikan. 


## topik sistem fisis
+ reaksi fisi nuklir dalam reaktor nuklir generasi IV. Untuk melakukan pengembangan reaktor dengan metode simulasi. dengan cara tersebut tidak memerlukan banyak biaya yang keluar


## simulasi dan visualisasi
+ Saya tertarik, karena saya selaku mahasiswa fisika banyak menggunakan simulasi dan visualisasi dalam melakukan berbagai hal penelitian. sehingga dapat mendukung proses penelitian
