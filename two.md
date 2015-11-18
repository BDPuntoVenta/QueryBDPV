# QueryBDPV
#Listar los productos ingresados en ultimo mes
select * from cardex where fecmov between '2015/10/01 00:00:01' and '2015/10/31 23:59:59';

#Lista los 10 productos con mas salida
select codpro,despro,prov.nomprov,sum(cantpro) from cardex car

inner join catpro pro on
car.carpro=pro.codpro


join catprov prov on 
pro.codprov=prov.codprov
group by codpro,despro,prov.nomprov

limit 10 
