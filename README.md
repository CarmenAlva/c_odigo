print 'Que deseas saber?... '
print '1) Velocidad'
print '2) Aceleracion'
opcion = float(raw_input('Elige un numero: '))
 
if opcion == 1:
    print 'Velocidad...'
    print ''
    E = float(raw_input ('Introduce el espacio recorrido en KM ---> '))
    T = float(raw_input ('Introduce el tiempo que se recorrio en Hs --->'))
    print 'La velocidad es %d' % (E/T), 'Km/h'
 
elif opcion == 2:
    print 'Aceleracion...'
    print ''
    Vi = float(raw_input ('Introduce la velocidad inicial---> '))
    Vf = float(raw_input ('Introduce la velocidad final---> ')) 
    T = float(raw_input ('Introduce el tiempo recorrido---> '))
    print 'La aceleracion es %d' % (Vf - Vi / T), 'Mts/seg**2'
