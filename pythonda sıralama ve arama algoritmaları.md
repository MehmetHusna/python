# python
// 1- Lineer Search
```python
def lineerSearch(liste,aranan): 
    for i in range(0,len(liste)):
        if(liste[i] == aranan):
            print("Aranan eleman listenin {}. elemanında bulundu".format(i))
        else: 
            pass
liste = [6,5,10,9,25]
lineerSearch(liste,9]
```
```
Ekran Çıktısı : Aranan eleman listenin 3. indisinde bulundu.
```


// 2- Binary Search
```python
def binarySearch(liste,aranan,sayici = 0):
    sayici += 1
    ortanca = len(liste)//2
    if(liste[ortanca] == aranan):
        return {"Adım sayısı":sayici,"Aranan":liste[ortanca]}
     
    elif(liste[ortanca] < aranan):
        liste = liste[ortanca:]
        return binarySearch(liste,aranan,sayici)
    elif(liste[ortanca] > aranan):
        liste = liste[:ortanca]
        return binarySearch(liste,aranan,sayici)
liste = [1,2,4,5,7,9,10,12]
print(binarySearch(liste,9)
 ```     
```
                                                                                   
                  SIRALAMA ALGORİTMALARI                                      
```

// 1- Bubble Sort
```python
def bubbleSort(liste):
    for i in range(0,len(liste)):
        for j in range(0,len(liste)-i-1):
            if(liste[j] > liste[j+1]):
                liste[j] , liste[j+1] = liste[j+1] , liste[j]
                
    return liste
 liste = [16,2,7,98,8]
 print(bubbleSort(liste))
```    
            
 // 2- Selection Sort
 ```python
 def selectionSort(liste): 
      for i in range(0,len(liste)):
           min = i
           for j in range(i+1,len(liste)):
               if(liste[min] > liste[j]):
                  min = j
               liste[min] , liste[j] = liste[j] , liste[min]
      return liste
      
 liste[1,5,9,12,3,54,24,19,2]
 print(selectionSort(liste))
 ```        


// 3- Insertion Sort
```python
def insertionSort(liste):
    for i in range(1,len(liste)):
        while (i>0 and liste[i-1]>liste[i]):
            liste[i-1] , liste[i] = liste[i] , liste[i-1]
            i -= 1
    return liste
liste = [5,6,10,9,67,45,37,18]
print(insertionSort(liste))
```


// 4- Shell Sort
```python
def shellSort(liste):
    atlama_degeri = len(liste)//2
    while(atlama_degeri>0):
        for i in range(atlama_degeri,len(liste)):
            degisken = liste[i]
            j = i 
            while(j >= ara_degisken and liste[j - atlama_degeri] > degisken):
                liste[j] = liste[j-atlama_degeri]
                j = j - atlama_degeri
            liste[j] = degisken
        atlama_degeri = atlama_degeri//2
     return liste
liste = [1,2,34,67,3,4,21,14,5,6,99,12]
print(ShellSort(liste))
```
