## SORT
 # Insertion Sort Örneği:
    # [22,27,16,2,18,6] dizisini;
    # 1.yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
    # 2.Big O Notation gösterimini yazınız.
    # 3.Time Complexity:Average Case:Aradığımız sayının ortada olması
                        Worst Case:Aradığımız sayının sonunda olması
                        Best Case:Aradığımız sayınının başında olması
    # 4.Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.
 
 # Çözümü:
    # 1.
    ## 1.AŞAMA:
     İlk önce sayı dizisinde en küçük elemanı bulup ilk baştaki elemanla yer değişikliği yapıyoruz.
        [22,27,16,2,18,6] => [2,27,16,22,18,6]
    ## 2.AŞAMA:
      Daha sonra en son düzenlediğimiz diziden tekrar en küçük elemanı bulup bu sefer 2. elemanla yer değişikliği yapıyoruz.
         [2,27,16,22,18,6] => [2,6,16,22,18,27]
    ## 3.AŞAMA:
      Tekrar en son düzenlediğimiz dizide en küçük elemanı bulup 3. elemanla yer değişikliği yapıyoruz.
         [2,6,16,22,18,27] => [2,6,16,22,18,27]   En küçük eleman 16 ve 3. sırada yer aldığı için yer değişikliği yapılmıyor.
    ## 4.AŞAMA:
      En son düzenlediğimiz diziye baktığımızda en küçük elemanı bulup bu seferde 4.elemanla yer değişikliği yapıyoruz.
         [2,6,16,22,18,27] => [2,6,16,18,22,27]
      Böylelikle dizimizi küçükten büyüğe doğru sıralamış olduk.
    # 2.
     # [2,27,16,22,18,6]      n => n-1 => n-2 => .... => 1 şeklinde ilerlediği için
       [2,6,16,22,18,27]         n+(n-1)+(n-2)+...+1= n(n+1)/2 den formülü n^2+1/2 oluyor.
       [2,6,16,22,18,27]            Big O Notation gösterimi O(n^2) oluyor.
       [2,6,16,18,22,27]      
    # 3.
     #Time Complexity= O(n^2)
    # 4.
      #[2,6,16,18,22,27]  18 sayısı sıralanmış dizide ortada olduğu için Average Case kapsamına giriyor.
 
 # 2.Örnek:
   # [7,3,5,8,2,9,4,15,6] dizisinin insertion Sort göre ilk 4 adımını yazınız.
    ## 1.Adım:
      dizideki en küçük sayı 2 dir. 1.sıradaki elemanla yer değişikliği yapıyoruz.
          [7,3,5,8,2,9,4,15,6] => [2,3,5,8,7,9,4,15,6]
    ## 2.Adım:
       En küçük sayı 3'tür. 2.sırada yer aldığı için yer değişikliği yapmıyoruz.
           [2,3,5,8,7,9,4,15,6]
    ## 3.Adım:
        En küçük sayı 4 tür. 3.sıradaki elemanla yer değişikliği yapıyoruz.
           [2,3,5,8,7,9,4,15,6] => [2,3,4,8,7,9,5,15,6]
    ## 4.Adım:
        En küçük sayı 5'tir. 4. sıradaki elemala yer değişiklği yapıyoruz.
           [2,3,4,8,7,9,5,15,6] => [2,3,4,5,7,9,8,15,6]
         
