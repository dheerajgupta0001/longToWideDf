# longToWideDf

df_long.pivot_table(index=["student", "school"], 
                    columns='class', 
                    values='grade')
pd.pivot_table pivots/splits a column into three separate columns
Long to wide: values in grade are split/pivoted into three separate columns (run code here)

#test
'''#print(maxDemandDf)
                testDf=maxDemandDf
                testDf = testDf.pivot_table(index=["TIME_STAMP"],
                                    columns='ENTITY_FULL_NAME', values='MAX_DEMAND')
                print(testDf)'''

 TIME_STAMP    MAX_DEMAND               ENTITY_TAG    ENTITY_FULL_NAME
0 2020-10-02    293.859985  WRLDCMP.SCADA1.A0046948           DAMAN DIU
1 2020-10-02  44848.601562  WRLDCMP.SCADA1.A0047000            WR-TOTAL
2 2020-10-02  14196.740234  WRLDCMP.SCADA1.A0046957              GUJRAT
3 2020-10-02  16018.950195  WRLDCMP.SCADA1.A0046980          MAHARASTRA
4 2020-10-02    704.049988  WRLDCMP.SCADA1.A0046953  DADAR NAGAR HAWELI
5 2020-10-02   9127.059570  WRLDCMP.SCADA1.A0046978      MADHYA PRADESH
6 2020-10-02    377.160004  WRLDCMP.SCADA1.A0046962                 GOA
7 2020-10-02   3779.620117  WRLDCMP.SCADA1.A0046945         CHATTISGARH
closed db connection after daily max demand data fetching
  time_stamp  MADHYA PRADESH  CHATTISGARH      WR-TOTAL  ...        GUJRAT         GOA   DAMAN DIU  DADAR NAGAR HAWELI
0 2020-10-02     9127.059570  3779.620117  44848.601562  ...  14196.740234  377.160004  293.859985          704.049988
