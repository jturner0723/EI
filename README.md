EI
==

Energy Insight Developement

select sa_id, char_type_cd, CHAR_VAL
 from ci_sa_char@ccbprod
 where sa_id in ('1014867265','1283037165','1813740606','1952292059','2086359617',
                 '2141428481','2310096514','2310096650','2342062005','2549937005')
 and char_type_cd in( 'SA-IDEMR','SA-IDIMR')
;

SA_ID      CHAR_TYP CHAR_VAL
---------- -------- ----------------
1283037165 SA-IDIMR
2086359617 SA-IDIMR
2549937005 SA-IDIMR

select sa_id, char_type_cd, CHAR_VAL_FK1
 from ci_sa_char@ccbprod
 where sa_id in ('1014867265','1283037165','1813740606','1952292059','2086359617',
                 '2141428481','2310096514','2310096650','2342062005','2549937005')
 and char_type_cd in( 'SA-IDEMR','SA-IDIMR')
;

SA_ID      CHAR_TYP CHAR_VAL_FK1
---------- -------- -------------------------------
1283037165 SA-IDIMR 1283037460
2086359617 SA-IDIMR 2086359273
2549937005 SA-IDIMR 2549937044


select sa_id, sa_status_flg, acct_id
 from ci_sa
 where sa_id in ('1283037460','2086359273','2549937044','1283037165','2086359617','2549937005')
;
