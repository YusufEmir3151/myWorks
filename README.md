/*-TABLO OLUŞTURMA-*/
CREATE TABLE kisiler (
  kisi_sira INT,
  kisi_adi VARCHAR(20),
  kisi_soyadi VARCHAR(30),
  kisi_eposta VARCHAR(50)
);



/*-KİŞİLER TABLOSUNDAN kişi_adi SATIRINDA Y İLE BAŞLAYAN SATIR-*/
select * from kisiler k  where kisi_adi  like 'Y%'

/*-KİŞİLER TABLOSUNDAN kisi_adi ve kisi-soyadi SÜTUNLARINI ÇEK-*/
select kisi_adi , kisi_soyadi  from kisiler k 

/*-TABLODAN VERİ SİLME-*/
delete from kisiler where kisi_sira= 1

/*-VERİ GÜNCELLEME-*/
update kisiler set kisi_adi='Yusuf Emir'  where kisi_adi='YusufEmir'  

/*-TABLOYU GÖSTERME-*/
select * from kisiler k  

/*-TABLOYA VERİ GİRİŞİ-*/
insert into kisiler values (2,'Abdullah','Sağlam', 'Abdullahsalam223@gmail.com')
