# QueryBDPV

﻿select * from cardex where fecmov between '2015/10/01 00:00:01' and '2015/10/31 23:59:59';

select * from cardex car
inner join catpro pro on
car.carpro=pro.codpro
