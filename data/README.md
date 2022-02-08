# Carpeta con los datos necesarios para el taller 

En esta carpeta hay dos tipos de datos repartidos en 21 ficheros.

Por un lado se tiene el fichero *grid_school_v2_8420_8785_003899999999998727.pkl* que contiene un objeto del tipo *pandas.DataFrame*. Este fichero contiene la malla de simulaciones para el entrenamiento de la red neuronal. Algunos de los parámetros con los que se simularon los espectros son Teff, logg y m_h que hacen referencia a la temperatura efectiva, el logaritmo de la gravedad y la metalicidad ([M/H]) respectivamente, se encuentran como columnas. Hay otra columna llamada *spectrum* que almacena el espectro simulado. 

Por otro lado, los ficheros *input_spectra_x.pkl* con x=0,...,19 son un subconjunto de espectros medidos con [RAVE](https://www.rave-survey.org/) que se utilizan como datos de entrada a la red neuronal entrenada y de los que se quiere inferir sus parámetros astrofísicos.

Nota: para las simulaciones se han usado los modelos atmosféricos de [MARCS](https://marcs.astro.uu.se/) y [Turbospectrum](https://ui.adsabs.harvard.edu/abs/2012ascl.soft05004P/abstract) como código de síntesis. El software utilizado para la generación ha sido [iSpec](https://www.blancocuaresma.com/s/iSpec).
