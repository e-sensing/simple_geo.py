# TODO list
- Migrar para abordagem get:
    - s = sgeo(...);
    - s.features(filter,within,order,etc).get() : SgeoFeatures : GeoDataFrame
    - s.time_series(...).get(): SgeoTime_Series: GeoDataFrame
    - s.coverage(...).get(): : SgeoCoverage:
    - s.map(...).get()

- Integrar feature com time_series:
    - ts = s.time_series( coverage="rpth",
                        attributes=("temp", "risco"),
                        start_date=sgeo.feature_date(-1),
                        end_date=sgeo.feature_date(2))
     - ft = s.features(filter=, within=, order=, ts=ts).get();
        - Se feature for Point TS ok
        - Se for linha?
        - Se for geometria: precisa associar uma operação reduce: máximo, minimo, média, mediana



- Criar README com pequenos exemplos
- Criar jupyter notebook para cada exemplo (criar link no readme)


- Na integração entre WFS e WTSS
  - Fazer mais testes
  - Integrar data (dia, período, dias para trás, frente e etc)

-Filter
	-  Implementar sgeo.AND e sgeo.OR

- README:
  - Implementrar vários trechos de código simples incremenais
  

- docs
  - Colocar um notebook com os exemplos
  - Se aceito, colocar o artigo como referencia na pagina e incluir o link para o pdf
  

- Implementar Cache (wfs e wtss, no simple_geo)

