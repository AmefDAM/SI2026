# UD1. Sistemas microinformáticos
## Avaliación e identificación dos compoñentes dun sistema informático 

**Módulo:** Sistemas informáticos

**Ciclo:** Desenvolvemento de Aplicacións Multiplataforma (DAM) 
 
## RA1. Avalía sistemas informáticos, identificando os seus compoñentes e as súas características 

---

# 1. CA1.1. Recoñecéronse os compoñentes físicos dun sistema informático e os seus mecanismos de interconexión.

## 1.1. Que é un sistema informático?

Un sistema informático é un conxunto de elementos relacionados que permite introducir, procesar, almacenar, transmitir e presentar información.

Nunha visión ampla intervén:

- **Hardware:** parte física do sistema.
- **Software:** instrucións e datos que controlan e utilizan o hardware.
- **Persoas:** utilizan, administran, manteñen ou desenvolven o sistema.

| Elemento | Función | Exemplos |
|---|---|---|
| Hardware | Parte física | CPU, RAM, placa base, SSD, monitor, teclado |
| Software | Instrucións e datos | Firmware, sistema operativo, aplicacións |
| Persoas | Uso e administración | Persoa usuaria, persoal técnico, administración |

## 1.2. Modelo funcional dun computador vs compoñentes actuais

O modelo de programa almacenado asociado á arquitectura de von Neumann continúa sendo útil como modelo conceptual. As instrucións e os datos se almacenan en memoria e o procesador execútanos seguindo unha secuencia controlada.

Podemos distinguir:

- **CPU:** procesa instrucións e datos.
- **Memoria principal:** mantén os programas e datos que están sendo utilizados.
- **Entrada/saída:** permite a comunicación co exterior.
- **Almacenamento persistente:** conserva datos e programas cando o equipo está apagado.
- **Interconexión:** permite que os diferentes elementos intercambien información.

Os computadores actuais son máis complexos que este modelo: existen varios niveis de cache, controladores integrados no procesador, enlaces punto a punto e numerosos dispositivos especializados. O modelo funcional segue sendo útil para comprender o papel de cada elemento.

Na actualidade un sistema informático está formado por diferentes compoñentes físicos que traballan de maneira coordinada, dos que os fundamentais son os seguintes:

| Compoñente | Función principal | Exemplos |
|---|---|---|
| Placa base | Interconectar os principais compoñentes | ATX, microATX, Mini-ITX |
| CPU | Executar instrucións e procesar datos | Intel Core, AMD Ryzen |
| RAM | Manter temporalmente datos e programas en uso | DDR4, DDR5 |
| Almacenamento | Conservar información de forma persistente | HDD, SSD SATA, SSD NVMe |
| Fonte de alimentación | Subministrar enerxía aos compoñentes | PSU ATX |
| GPU | Procesar gráficos e tarefas paralelizables | Integrada ou dedicada |
| Tarxeta de expansión | Engadir funcións ao sistema | Rede, audio, captura |
| Chasis | Soportar e protexer os compoñentes | ATX, microATX, SFF |

## 1.3. Chasis e factor de forma

O chasis proporciona soporte mecánico, protección, circulación de aire e espazo para os compoñentes.

O **factor de forma** determina entre outros aspectos, as dimensións da placa e a súa compatibilidade mecánica co chasis:

- dimensións da placa;
- posición dos puntos de fixación;
- disposición dos compoñentes;
- compatibilidade mecánica co chasis;
- determinados requisitos de alimentación.

Os formatos máis relevantes para esta unidade son:

| Factor de forma | Características |
|---|---|
| ATX | Formato de sobremesa moi estendido, con varias posibilidades de expansión |
| microATX | Máis pequeno, mantendo boa parte da infraestrutura ATX |
| Mini-ITX | Formato compacto, habitualmente 170 × 170 mm |
| E-ATX e formatos de estación/servidor | Maiores dimensións e posibilidades de expansión |
| Propietario | Deseñado por un fabricante concreto; pode limitar substitucións |

![Comparación visual de diversos factores de forma de placa base](imaxes/factorFormaPlacaBase.png)


Ao seleccionar unha placa e un chasis non abonda con que ambos sexan compatibles nominalmente. Tamén hai que comprobar:

- altura máxima do disipador;
- lonxitude máxima da GPU;
- formato da fonte;
- espazo para unidades;
- posición dos conectores;
- posibilidades de cableado;
- ventilación.

## 1.4. Fonte de alimentación

A **fonte de alimentación (PSU)** converte a enerxía eléctrica da rede nas tensións de corrente continua necesarias para os compoñentes.

Unha fonte debe proporcionar:

- potencia suficiente;
- tensións estables;
- proteccións eléctricas;
- conectores adecuados;
- formato compatible;
- refrixeración suficiente.

Ao seleccionar unha fonte hai que considerar:

1. Consumo previsto de CPU e GPU.
2. Consumo das unidades e demais dispositivos.
3. Marxe suficiente para picos de consumo.
4. Calidade e eficiencia.
5. Conectores necesarios.
6. Compatibilidade co chasis.

Nos equipos modernos é habitual atopar:

- conector principal da placa base;
- conector adicional para alimentación da CPU;
- conectores para unidades SATA;
- conectores adicionais para GPU, cando sexan necesarios.

**Importante:** non se debe conectar un cable simplemente porque encaixe fisicamente. Débese utilizar o cableado previsto polo fabricante da fonte e do dispositivo.

## 1.5. Placa base

A **placa base** é o circuíto impreso que proporciona os elementos mecánicos e eléctricos necesarios para conectar CPU, memoria, almacenamento, tarxetas de expansión, periféricos e alimentación.

Cómpre saber localizar:

- socket do procesador;
- slots de memoria;
- slots PCI Express;
- conectores M.2;
- portos SATA;
- conectores de alimentación;
- cabeceiros de ventiladores;
- cabeceiros USB internos;
- conectores do panel frontal;
- audio;
- rede;
- outros controladores integrados.

### O chipset

Nos PCs antigos era habitual describir a placa mediante **Northbridge** e **Southbridge**. Esta explicación é útil como contexto histórico, pero non debe empregarse como modelo principal dos equipos actuais.

Nas plataformas modernas moitas funcións tradicionalmente asociadas ao Northbridge están integradas no procesador, como parte do controlador de memoria e determinadas interconexións. A placa dispón ademais dun controlador/chipset da plataforma que xestiona outras funcións de entrada/saída.

O importante desde o punto de vista práctico é saber:

- que dispositivos soporta a plataforma;
- que interfaces proporciona;
- que CPU e memoria son compatibles;
- cantos slots e conectores existen;
- como se distribúen os carrís (*lanes*) PCIe;
- que funcións están integradas.

## 1.6. Socket, CPU e compatibilidade

O **socket** proporciona a conexión eléctrica e mecánica entre o procesador e a placa base.

Para saber se unha CPU é compatible hai que comprobar:

- socket;
- plataforma/chipset;
- versión mínima do firmware, cando proceda;
- consumo e solución térmica;
- compatibilidade da memoria.

Existen diferentes tipos de encapsulado:

- **LGA:** os contactos están no socket e o procesador presenta superficies de contacto.
- **PGA:** o procesador dispón de pines.
- **BGA:** o compoñente está soldado á placa e non está pensado para a substitución.

A CPU executa instrucións. Conceptualmente podemos distinguir:

- unidades de cálculo;
- unidades de control;
- rexistros;
- memoria cache.

Nas CPU actuais tamén son relevantes:

- número de núcleos;
- número de fíos;
- frecuencia;
- caches;
- consumo;
- arquitectura;
- aceleradores especializados.

A frecuencia por si soa non determina o rendemento dun procesador.

## 1.7. Almacenamento

O almacenamento persistente conserva a información sen alimentación.

| Tipo | Características | Uso |
|---|---|---|
| HDD | Discos magnéticos con partes móbiles | Gran capacidade, copias e almacenamento masivo |
| SSD SATA | Memoria flash, sen partes móbiles, interface SATA | Equipos e actualizacións |
| SSD NVMe | Memoria flash, normalmente sobre PCIe e protocolo NVMe | Sistemas que precisan baixa latencia e alto rendemento |
| Almacenamento USB | Dispositivo externo | Transporte, copias e almacenamento |

### M.2 non é NVMe

Este é un concepto fundamental:

- **M.2** é un formato físico/conector.
- **SATA** é unha interface.
- **PCIe** é unha interconexión.
- **NVMe** é un protocolo para almacenamento non volátil.

Un SSD M.2 pode utilizar SATA ou PCIe/NVMe, segundo o modelo e o slot.

Antes de instalar un SSD M.2 hai que consultar o manual da placa para saber:

- que tamaños admite;
- que tipo de interface admite;
- se comparte recursos con determinados portos SATA ou PCIe;
- se precisa disipador.

## 1.8. GPU e tarxetas de expansión

A GPU pode estar integrada no procesador/plataforma ou formar parte dunha tarxeta dedicada.

Unha GPU dedicada dispón habitualmente de:

- procesador gráfico;
- memoria gráfica;
- sistema de alimentación;
- sistema de refrixeración;
- interface PCI Express.

As tarxetas de expansión poden proporcionar:

- rede;
- audio;
- captura de vídeo;
- controladoras de almacenamento;
- adquisición de datos;
- interfaces adicionais.

## 1.9. Buses, interfaces, conectores e protocolos

Estes termos non son sinónimos.

| Concepto | Significado | Exemplo |
|---|---|---|
| Bus/interconexión | Mecanismo polo que se comunican elementos | PCI Express |
| Interface | Forma normalizada de comunicación | SATA, USB |
| Protocolo | Regras para intercambiar información | NVMe |
| Conector | Elemento físico que permite a conexión | USB-C |
| Porto | Punto de conexión accesible | Porto USB dun portátil |

**PCI Express (PCIe)** é unha interconexión de alta velocidade para expansión. Pode utilizar diferentes cantidades de carrís (*lanes*), como x1, x4, x8 ou x16.

**SATA** utilízase principalmente para dispositivos de almacenamento.

**USB** permite conectar numerosos periféricos. USB-C identifica o conector físico, pero non determina por si só a velocidade ou todas as funcións dispoñibles.

### Ancho de banda

O ancho de banda expresa a cantidade máxima de datos que pode transferirse por unidade de tempo.

É necesario distinguir:

- **b** = bit;
- **B** = byte;
- **b/s** = bits por segundo;
- **B/s** = bytes por segundo.

Como 1 byte = 8 bits:

> 800 Mb/s = 100 MB/s, sen considerar sobrecargas do protocolo.

Na práctica, o rendemento real adoita ser inferior ao máximo teórico por sobrecargas, latencia, limitacións dos dispositivos e condicións do sistema.

### Unidades decimais e binarias

No Sistema Internacional (en base 10):

- 1 kB = 1.000 bytes
- 1 MB = 1.000.000 bytes
- 1 GB = 1.000.000.000 bytes
- 1 TB = 1.000.000.000.000 bytes

Nas unidades binarias (en base 2), definidas pola IEC (Comisión Electrotécnica Internacional):

- 1 KiB = 1.024 bytes
- 1 MiB = 1.024 KiB
- 1 GiB = 1.024 MiB
- 1 TiB = 1.024 GiB

Non deben confundirse GB con GiB.

![Unidades IEC / Unidades SI](imaxes/IECvsSI.png)

A mestura de ambas unidades explica porqué o tamaño dos dispositivos de almacenamento indicado polos fabricantes, na práctica é inferior á capacidade real de almacenamento:

![Exemplo de como calcula-la capacidade de almacenamento real dun disco](imaxes/exemploCapacidadeDisco.png)

Para pasar do que di a caixa dun disco (unidades ***SI***) ó tamaño real que verás no ordenador (unidades ***IEC***), hai que facer dous pasos:
- Paso 1 (partindo da capacidade anunciada polo fabricante): converte-la capacidade comercial (GB ou TB) a bytes puros, multiplicando por potencias de 1.000.
- Paso 2 (obtención da capacidade real recoñecida polo sistema operativo): convertes eses bytes puros á unidade binaria real (GiB ou TiB), dividindo por potencias de 1.024.

![Método para calcula-la capacidade de almacenamento real dos dispositivos de almacenamento](imaxes/calculoCapacidadeReal.png)

Cando nos referimos ao ancho de banda das transferencias internas (como PCI Express, SATA ou NVMe), as unidades utilízanse habitualmente segundo o Sistema Internacional (SI), é dicir, en base 10 (decimais), e mídense en bytes por segundo (B/s, MB/s, GB/s) ou bits por segundo (b/s, Gb/s).

Hai que ter en conta varios detalles para evitar confusións comúns:

**1. Velocidade do bus e interface (Sistema Internacional - Base 10)**
Os fabricantes e as especificacións oficiais sempre anuncian o ancho de banda teórico usando as potencias de 10:

* SATA III: ten un ancho de banda máximo de 6 Gb/s (Gigabits por segundo), que tras a codificación dos datos tradúcese nuns 600 MB/s (Megabytes por segundo) reais de transferencia.
* NVMe (PCIe 4.0 x4): ten un ancho de banda teórico de ata 8 GB/s (Gigabytes por segundo).
* ***Nota:*** neste contexto, 1 GB/s son exactamente 1.000 MB/s, e 1 MB/s son 1.000 KB/s.

**2. A confusión co sistema IEC (Base 2)**
Aínda que a velocidade da canle se mida co Sistema Internacional, o software (especialmente sistemas operativos como Windows) adoita calcular as taxas de transferencia e o tamaño dos ficheiros en base 2 (unidades IEC como MiB/s ou GiB/s, aínda que Windows use erroneamente as siglas MB/s e GB/s).
A diferenza de cálculo amósase na seguinte táboa:

| Tipo de Unidade | Base | Exemplo de cálculo | Onde se usa habitualmente |
|---|---|---|---|
| SI (Decimal) | $10^3 = 1.000$ | 1 GB = 1.000 MB | Especificacións de hardware (PCIe, SATA, NVMe), publicidade de fabricantes. |
| IEC (Binario) | $2^{10} = 1.024$ | 1 GiB = 1.024 MiB | Medicións reais de movemento de ficheiros dentro de Linux ou Windows. |

Por esta razón, cando copias un ficheiro nun NVMe que sobre o papel (SI) vai a 7.000 MB/s, Windows pode mostrarche unha velocidade máxima de arredor de 6.519 MiB/s (indicado como MB/s), simplemente porque o sistema operativo divide entre 1.024 en lugar de entre 1.000.

Iso si, aos fabricantes valles moi ben esta discrepancia porque comercialmente un número decimal sempre vai ser máis alto e vistoso que un binario. Benefícianse dun lio de estándares que Windows non quere corrixir para non romper a compatibilidade con programas antigos.

**3. Velocidades de transferencia por rede -Internet, Ethernet, Wi-Fi, etc.- (Sistema Internacional)**
A diferenza principal co hardware interno é que en redes a unidade de medida estándar **non é o byte, senón o **bit** por segundo (b/s).**

A maior confusión en redes non vén polo sistema SI vs IEC, senón por mesturar bits (velocidade da liña) con bytes (tamaño dos ficheiros):

* Un Byte son 8 bits.
* Se tes unha conexión de 100 Mbps (Megabits), para saber a velocidade máxima teórica de descarga en Megabytes (MB) tes que dividir entre 8:
$$\frac{100 \text{ Mbps}}{8} = 12,5 \text{ MB/s}$$

Por tanto, se contratas 1.000 Megas (1 Gbps) de fibra, o teu navegador (que mide en IEC) amosará unha descarga máxima teórica de arredor de 119,2 MiB/s (indicado habitualmente como 119,2 MB/s), debido á conversión de bits a bytes (/8) e despois de decimal a binario (/1.024), sen contar a perda por tráfico de control (overhead).

## 1.10. PCI Express

**PCI Express (PCIe)** é a principal interconexión de expansión de alta velocidade dos PCs actuais.

Utiliza enlaces punto a punto e pode combinar carrís (*lanes*):

- x1;
- x2;
- x4;
- x8;
- x16;
- etc.

A notación x16 significa que o enlace dispón de ata 16 carrís, non que todos os slots físicos x16 teñan necesariamente 16 carrís activos.

Un dispositivo pode funcionar nun enlace con menos carrís cando a plataforma o permite.

As diferentes xeracións de PCIe aumentan a taxa de transferencia por carril. A especificación continúa evolucionando, polo que non ten sentido memorizar todas as velocidades históricas. O importante é comprender:

1. xeración;
2. número de carrís;
3. compatibilidade;
4. ancho de banda;
5. función do dispositivo.

## 1.11. SATA

SATA é unha interface utilizada principalmente para unidades de almacenamento.

Nunha unidade SATA de sobremesa adoitan existir:

- un conector de datos SATA;
- un conector de alimentación SATA.

A unidade debe estar conectada correctamente á placa base e á fonte.

A antiga interface **IDE/PATA**, baseada en cables paralelos e configuración mestre/escravo, debe tratarse como tecnoloxía histórica e de compatibilidade con equipos antigos.

## 1.12. USB e USB-C

USB é unha familia de tecnoloxías para conectar periféricos e outros dispositivos.

**USB-C é un tipo de conector físico**, non unha velocidade concreta.

Un porto USB-C pode ofrecer, segundo o equipamento:

- datos;
- alimentación;
- vídeo mediante modos alternativos;
- USB4;
- outras tecnoloxías.

Por iso, dous portos USB-C visualmente idénticos poden ter capacidades moi diferentes.

Para coñecer as capacidades reais débese consultar:

- símbolos do fabricante;
- manual;
- especificacións do equipo;
- documentación do porto.

## 1.13. Vídeo

As interfaces máis relevantes son:

- HDMI;
- DisplayPort.

Tamén poden atoparse VGA ou DVI en equipamentos antigos.

Para comprobar a compatibilidade dunha conexión de vídeo débese verificar:

- tipo de conector;
- versión da interface;
- resolución;
- frecuencia de refresco;
- capacidades da GPU;
- capacidades do monitor;
- adaptadores utilizados.

## 1.14. Rede

Os equipos poden conectarse mediante:

- **Ethernet:** rede cableada;
- **Wi-Fi:** rede sen fíos;
- **Bluetooth:** comunicación de curto alcance con periféricos e outros dispositivos.

Un adaptador de rede pode estar integrado na placa base ou instalarse como dispositivo adicional.

## 1.15. Periféricos

Os periféricos poden clasificarse como:

| Categoría | Exemplos |
|---|---|
| Entrada | Teclado, rato, cámara, micrófono, escáner |
| Saída | Monitor, impresora, proxector, altofalantes |
| Entrada/saída | Pantalla táctil, almacenamento externo |
| Comunicación | Ethernet, Wi-Fi, Bluetooth |
| Almacenamento | SSD externo, disco externo, memoria USB |

A clasificación debe entenderse como funcional: un mesmo dispositivo pode cumprir varias funcións.

## 1.16. Interfaces

| Interface | Exemplos de uso | Que comprobar |
|---|---|---|
| USB-A / USB-C | Teclado, rato, discos, cámaras | Versión, velocidade, alimentación e funcións |
| HDMI | Monitores e televisores | Versión, resolución e frecuencia |
| DisplayPort | Monitores | Versión, resolución e frecuencia |
| Ethernet | Rede cableada | Velocidade e controlador |
| Wi-Fi | Rede sen fíos | Estándar e banda |
| Bluetooth | Periféricos | Emparellamento e compatibilidade |
| Audio | Micrófono, auriculares | Entrada/saída e configuración |

## 1.17. Instalación dun periférico

Procedemento xeral:

1. Identificar o dispositivo.
2. Identificar a interface.
3. Comprobar compatibilidade.
4. Conectar.
5. Comprobar alimentación.
6. Verificar detección.
7. Instalar controlador se é necesario.
8. Configurar.
9. Probar.
10. Documentar.

### Exemplo: monitor

1. Comprobar saída da GPU.
2. Comprobar entrada do monitor.
3. Seleccionar cable compatible.
4. Conectar.
5. Acender.
6. Seleccionar a entrada correcta.
7. Comprobar detección.
8. Seleccionar resolución adecuada.
9. Seleccionar frecuencia soportada.
10. Verificar estabilidade da imaxe.

### Exemplo: impresora

1. Identificar interface.
2. Conectar ou configurar a rede.
3. Instalar controlador ou utilizar o soporte do sistema.
4. Engadir a impresora.
5. Configurar preferencias.
6. Imprimir unha páxina de proba.
7. Comprobar cola e estado.

## Actividade A1.1 — Identificación dun sistema informático

**Obxectivo:** identifica-los principais compoñentes físicos e explicar como se interconectan.

1. Selecciona un PC físico ou unha configuración documentada polo fabricante.
2. Identifica placa base, CPU, RAM, almacenamento, fonte e GPU.
3. Localiza os conectores e interfaces principais.
4. Identifica polo menos unha conexión PCIe, unha SATA e unha USB.
5. Explica a función de cada conexión.
6. Indica se o almacenamento utilizado é SATA ou NVMe.
7. Elabora unha ficha técnica.

**Entrega:**

| Elemento | Modelo/tipo | Interface ou conexión | Función |
|---|---|---|---|
| CPU | | | |
| RAM | | | |
| Almacenamento | | | |
| GPU | | | |
| Rede | | | |

**Evidencia:** ficha técnica + esquema ou fotografía anotada.

---
# 2. CA1.2. Clasificáronse os tipos de memorias, sinalando as súas características e identificando as súas prestacións e a función que desenvolven no conxunto do sistema.

## 2.1. Memoria RAM

A **RAM (Random Access Memory)** é a memoria principal de traballo. É normalmente volátil: o seu contido pérdese ao interromperse a alimentación.

A RAM contén temporalmente:

- partes do sistema operativo;
- programas en execución;
- datos que estes programas están utilizando.

Ao seleccionar memoria hai que comprobar:

- tipo de memoria
- xeración
- capacidade
- capacidade máxima admitida
- número de módulos
- velocidade/taxa de transferencia
- formato
- compatibilidade eléctrica
- número e configuración de canles
- ECC, se a plataforma o admite

### DDR e xeracións

A memoria DDR realiza transferencias de datos nas transicións do sinal de reloxo. Ao longo do tempo evolucionou desde DDR ata DDR2, DDR3, DDR4 e DDR5.

Para unha unidade actual interesa especialmente distinguir **DDR4 e DDR5**, sen necesidade de memorizar táboas históricas de pines e tensións de todas as xeracións.

Un módulo DDR non pode instalarse indistintamente nun slot doutra xeración: a muesca, o número de contactos e as características eléctricas impiden a compatibilidade directa.

### DIMM e SO-DIMM

- **DIMM:** formato habitual en sobremesas.
- **SO-DIMM:** formato compacto frecuente en portátiles e equipos pequenos.

### Canles de memoria, tecnoloxía multicanle

As plataformas poden utilizar dous ou máis canles para aumentar o ancho de banda dispoñible.

A configuración correcta depende da placa. Por iso, para instalar dous módulos non se debe aplicar unha regra universal como "sempre nos slots 1 e 2": débese consultar o manual, que indicará os slots recomendados.

Unha das arquitecturas fundamentais para mellorar o acceso á memoria RAM é o **sistema multicanle**. Esta tecnoloxía permite que o procesador se comunique con varios módulos de memoria de forma simultánea a través de canles independentes, multiplicando así o ancho de banda dispoñible e mellorando notablemente as prestacións do sistema.

**Dobre canle (Dual Channel)**

Permite acceder a dous módulos ou subcanles de memoria simultaneamente para incrementar a taxa de transferencia de datos.

Esta tecnoloxía é especialmente efectiva con controladoras de vídeo integradas no procesador (iGPU). Como estas gráficas non teñen memoria VRAM dedicada, utilizan a RAM do sistema; ao duplicar o ancho de banda mediante o Dual Channel, o rendemento gráfico aumenta de forma drástica.

![Dual Channel](imaxes/dualChannel.png)

O funcionamento varía segundo a xeración de memoria:

* En memorias DDR4 (e anteriores): agrúpanse dúas canles físicas de 64 bits para realizar transferencias en bloques de 128 bits. Para practicalo, precísanse dous módulos de memoria instalados nos zócalos axeitados da placa base.
* En memorias DDR5: o propio estándar revolucionou esta arquitectura. Un único módulo DDR5 xa funciona internamente en dobre canle, dividindo o bus de datos en dúas canles independentes de 32 bits (máis 8 bits de corrección de erros ECC). Se instalamos dous módulos DDR5, o sistema pasa a operar nunha configuración equivalente a cuádruple canle virtual.

As condicións para activar o multicanle óptimo son:

* Ter o controlador de memoria integrado no propio procesador (CPU) compatible coa tecnoloxía (estándar en todos os procesadores modernos).
* Utilizar módulos de memoria instalados nos zócalos recomendados polo fabricante da placa base (habitualmente identificados por cores alternas ou especificados no manual).
* Para evitar perdas de rendemento ou incompatibilidades, recoméndase que os módulos sexan do mesmo tipo (DDR4 ou DDR5), capacidade, velocidade e latencia (preferiblemente adquiridos xuntos nun mesmo kit).

![Combinacións dual channel nunha placa segundo o seu fabricante](imaxes/colocacionModulosDualChannel.png)


**Cuádruple canle (Quad Channel)**

Permite acceder de forma simultánea a catro canles de memoria independentes. Hoxe en día a canle cuádrupla nativa quedou relegada case en exclusiva a contornas profesionais onde o manexo de inmensos volumes de datos xustifica o seu custo.

### SPD

Os módulos de memoria incorporan información **SPD (Serial Presence Detect)** que permite ao firmware identificar características do módulo e seleccionar parámetros adecuados.

En Linux pódense consultar datos mediante ferramentas como:

```bash
sudo dmidecode --type memory
```

Segundo o hardware tamén pode ser posible consultar información SPD con ferramentas específicas.

## Actividade A1.2 — Identificación e comparación de memoria

**Obxectivo:** identificar a memoria dun equipo e relacionar as súas características coa plataforma.

1. Executa:

```bash
sudo dmidecode --type memory
```

2. Identifica tipo, capacidade, velocidade e formato.
3. Indica cantos módulos están instalados.
4. Consulta o manual da placa ou do equipo.
5. Determina a configuración de canles recomendada.
6. Explica se sería posible ampliar a memoria e ata que capacidade.

**Entrega:**

| Parámetro | Valor detectado | Interpretación |
|---|---|---|
| Tipo | | |
| Capacidade total | | |
| Capacidade por módulo | | |
| Velocidade | | |
| Formato | | |
| Slots ocupados | | |
| Slots dispoñibles | | |
| Configuración de canles | | |

---

# 3. CA1.2. Verificouse o proceso de posta en marcha dun equipamento

## 3.1. Secuencia xeral

Ao premer o botón de acendido non se inicia inmediatamente o sistema operativo. Primeiro debe prepararse o hardware.

A secuencia simplificada é:

1. Iníciase a alimentación.
2. Comeza a execución da CPU.
3. Iníciase o firmware.
4. Inicialízanse os compoñentes.
5. Realízase o **POST**.
6. Detéctanse os dispositivos necesarios.
7. Aplícase a configuración do firmware.
8. Selecciónase unha entrada de arranque.
9. Execútase o Boot Manager.
10. Cárgase o sistema operativo.

A secuencia exacta depende da plataforma.

## 3.2. POST

O **POST (Power-On Self-Test)** é a fase inicial de comprobación realizada polo firmware.

Pode comprobar:

- memoria
- procesador
- dispositivos fundamentais
- controladoras
- outros elementos necesarios para continuar

Un problema pode producir:

- pantalla sen sinal
- mensaxe de erro
- código LED
- código no display da placa
- sinais acústicos
- reinicio continuo
- imposibilidade de atopar o dispositivo de arranque

Os métodos de diagnose dependen da placa e deben consultarse no manual.

## 3.3. BIOS legado e UEFI

**BIOS** designa o modelo tradicional de firmware dos PCs. **UEFI** define un modelo máis moderno de interface entre o firmware da plataforma e o cargador do sistema operativo.

Nun sistema UEFI é habitual traballar con:

- entradas de arranque;
- Boot Manager;
- EFI System Partition;
- controladores e aplicacións de prearranque;
- Secure Boot.

Non é correcto afirmar que UEFI só permite **sistemas operativos de 64 bits**. Tampouco se debe identificar UEFI con ***Secure Boot***: Secure Boot é unha función de seguridade que pode utilizarse dentro do modelo UEFI.

## 3.4. EFI System Partition

A **EFI System Partition (ESP)** é unha partición utilizada habitualmente nos sistemas UEFI para almacenar ficheiros de arranque.

Unha secuencia simplificada pode ser:

**Firmware UEFI → entrada de arranque → Boot Manager → cargador do SO → núcleo do SO**

Isto permite comprender por que o modelo:

**BIOS → MBR → código de arranque**

debe tratarse como un modelo de arranque legado, non como a descrición xeral dos PCs actuais.

## 3.5. Secure Boot

Secure Boot permite verificar os compoñentes autorizados da cadea de arranque antes de executalos.

O obxectivo é dificultar a execución de software non autorizado ou modificado durante o arranque.

Se se modifica esta opción:

1. debe coñecerse o estado inicial
2. débese comprobar a compatibilidade co sistema operativo
3. hai que saber como restaurar a configuración
4. deben seguirse as indicacións do fabricante do equipamento

## 3.6. Configuración básica do UEFI

Entre as opcións que poden aparecer están:

- data e hora
- orde de arranque
- dispositivos de almacenamento
- memoria
- CPU
- virtualización
- ventiladores
- dispositivos integrados
- Secure Boot
- TPM
- actualización do firmware
- restauración de valores por defecto

Non se debe memorizar a localización dunha opción concreta: as interfaces cambian entre fabricantes.

A competencia importante é **saber localizar e interpretar a opción necesaria utilizando o manual**.

### Orde de arranque

Determina que entradas ou dispositivos se intentarán utilizar para iniciar o sistema.

### Memoria

Pode permitir seleccionar perfís ou parámetros compatibles coa memoria instalada.

### Virtualización

As plataformas actuais dispoñen habitualmente de extensións de virtualización. Deben activarse se son necesarias para utilizar determinadas plataformas de máquinas virtuais.

### Ventiladores

Pódense configurar curvas de funcionamento para equilibrar:

- temperatura;
- ruído;
- consumo.

### Dispositivos integrados

Pódense activar ou desactivar determinadas interfaces, como:

- audio;
- rede;
- controladoras;
- determinados portos.

### TPM e Secure Boot

Son relevantes para a seguridade da plataforma e para determinados sistemas operativos.

### Actualización do firmware

Procedemento:

1. Identificar modelo e revisión exacta.
2. Consultar o soporte oficial.
3. Ler as notas da versión.
4. Comprobar requisitos.
5. Anotar a configuración actual.
6. Utilizar o método recomendado.
7. Non interromper a alimentación.
8. Comprobar a versión tras actualizar.

Unha actualización incorrecta pode inutilizar o equipamento, polo que non debe facerse sen verificar previamente o modelo.


## 3.7. Diagnose dun equipo que non arranca

Ante un equipo que non arranca, seguir unha secuencia:

1. Comprobar alimentación eléctrica.
2. Comprobar interruptor da fonte, se existe.
3. Comprobar alimentación da placa e CPU.
4. Comprobar RAM.
5. Comprobar GPU e conexión do monitor.
6. Observar LEDs/códigos de diagnóstico.
7. Consultar o manual.
8. Probar unha configuración mínima.
9. Eliminar variables innecesarias.
10. Repetir a proba e documentar o resultado.

## Actividade A1.3 — Verificación do arranque

1. Inicia un equipamento.
2. Accede ao UEFI.
3. Identifica:
   - modelo da placa;
   - CPU;
   - memoria;
   - dispositivos de almacenamento;
   - modo de arranque;
   - entradas de arranque.
4. Identifica a entrada utilizada para iniciar o sistema.
5. Localiza, se é posible, a configuración de Secure Boot.
6. Documenta a secuencia observada.

**Entrega:** captura ou fotografía das pantallas relevantes + descrición paso a paso.

### Exercicio de diagnóse

Un equipo acende pero non mostra imaxe.

Ordena unha primeira secuencia de comprobacións entre:

- monitor;
- cable;
- entrada seleccionada no monitor;
- GPU;
- alimentación da GPU;
- RAM;
- indicadores de diagnóstico;
- manual da placa.

Xustifica a orde escollida.

---

# 4. CA1.4. Clasificáronse, instaláronse e configuráronse diferentes tipos de dispositivos periféricos.

## 4.1. Clasificación funcional

| Tipo | Exemplos |
|---|---|
| Entrada | Teclado, rato, cámara, micrófono, escáner |
| Saída | Monitor, impresora, proxector, altofalantes |
| Entrada/saída | Pantalla táctil, almacenamento externo, multifunción |
| Comunicación | Ethernet, Wi-Fi, Bluetooth |
| Almacenamento | SSD externo, disco externo, memoria USB |

A clasificación é funcional: un mesmo dispositivo pode cumprir varias funcións.

## 4.2. Interfaces habituais

| Interface | Exemplos de uso | Que comprobar |
|---|---|---|
| USB-A / USB-C | Teclado, rato, almacenamento | Versión, velocidade, alimentación |
| HDMI | Monitor/TV | Versión, resolución, frecuencia |
| DisplayPort | Monitor | Versión, resolución, frecuencia |
| Ethernet | Rede cableada | Velocidade e controlador |
| Wi-Fi | Rede sen fíos | Estándar e banda |
| Bluetooth | Periféricos | Compatibilidade e emparellamento |
| Audio | Micrófono/auriculares | Entrada ou saída |

## 4.3. Procedemento de instalación

1. Identificar o dispositivo.
2. Identificar a interface.
3. Comprobar compatibilidade.
4. Conectar ou emparellar.
5. Comprobar alimentación.
6. Verificar detección.
7. Instalar controlador se é necesario.
8. Configurar.
9. Realizar unha proba.
10. Documentar o resultado.

## Actividade A1.4 — Instalación e configuración de periféricos

Instala e verifica, cando estean dispoñibles, polo menos:

- teclado ou rato;
- monitor;
- dispositivo de audio;
- almacenamento externo;
- dispositivo Bluetooth ou Wi-Fi.

Para cada un:

| Dispositivo | Función | Interface | Detectado | Controlador | Configuración | Proba |
|---|---|---|---|---|---|---|
| | | | | | | |

---

# CA1.5. Identificáronse os tipos de redes e de sistemas de comunicación.

## 5.1. Características das redes

Unha rede permite intercambiar información e compartir recursos entre dispositivos.

Ao describila pódense considerar:

- alcance;
- medio de transmisión;
- velocidade;
- topoloxía;
- tecnoloxía utilizada;
- finalidade.

## 5.2. Tipos de rede segundo o alcance

- **PAN:** rede de ámbito persoal.
- **LAN:** rede de área local.
- **WLAN:** LAN baseada en comunicación sen fíos.
- **MAN:** rede de ámbito metropolitano.
- **WAN:** rede de grande extensión xeográfica.

## 5.3. Sistemas de comunicación

Segundo o medio poden distinguirse:

- comunicación cableada;
- comunicación sen fíos.

Entre as tecnoloxías habituais están:

- Ethernet;
- Wi-Fi;
- Bluetooth;
- fibra óptica.

## Actividade A1.5 — Clasificación de redes

Para cada escenario indica o tipo de rede e o medio de comunicación máis axeitado:

1. Teclado conectado por Bluetooth.
2. Rede dunha aula con 25 equipos.
3. Rede Wi-Fi dunha vivenda.
4. Conexión entre sedes situadas en cidades diferentes.
5. Comunicación entre teléfono e auriculares.

Xustifica cada resposta.

---

# CA1.6. Identificáronse os compoñentes dunha rede informática.

## 6.1. Elementos básicos

Unha rede pode incluír:

- dispositivos finais
- adaptadores de rede
- medios de transmisión
- conmutadores (*switches*)
- enrutadores (*routers*)
- puntos de acceso (*access points*)
- cableado e conectores

## 6.2. Adaptadores de rede

Un adaptador proporciona a interface necesaria para conectar un dispositivo á rede.

Pode ser:

- integrado na placa base
- unha tarxeta de expansión
- un adaptador USB
- un adaptador sen fíos

## 6.3. Cableado e conectores

Nas redes cableadas pódense atopar diferentes tipos de cable e conectores. En Ethernet sobre par trenzado é habitual o conector **RJ-45**.

Cómpre distinguir o medio físico do protocolo ou tecnoloxía de comunicación que utiliza.

## 6.4. Dispositivos de interconexión

- **Switch:** interconecta dispositivos dunha rede local.
- **Router:** interconecta redes diferentes e realiza funcións de enrutamento.
- **Access Point:** proporciona acceso sen fíos á rede.
- **Repetidor:** amplía ou rexenera un sinal segundo a tecnoloxía empregada.

## Actividade A1.6 — Inventario dunha rede local

Observa a rede dunha aula, laboratorio ou domicilio e identifica:

| Elemento | Modelo | Función | Conexión |
|---|---|---|---|
| Router | | | |
| Switch | | | |
| Access Point | | | |
| Adaptador de rede | | | |
| Cableado | | | |

Debuxa un esquema sinxelo indicando como están conectados os elementos.

---

# CA1.7. Interpretáronse mapas físicos e lóxicos dunha rede informática.

## 7.1. Mapa físico

Representa a disposición real dos elementos:

- equipos;
- racks;
- switches;
- puntos de acceso;
- cableado;
- localizacións.

Responde principalmente á pregunta:

> **Onde está cada elemento e como está conectado fisicamente?**

## 7.2. Mapa lóxico

Representa a organización da comunicación:

- redes;
- subredes;
- enderezos IP;
- gateways;
- VLAN, cando existan;
- relacións entre dispositivos.

Responde principalmente á pregunta:

> **Como se organiza a comunicación entre os dispositivos?**

## Actividade A1.7 — Interpretación dun mapa de rede

A partir dun mapa de rede proporcionado pola persoa docente:

1. Identifica os dispositivos.
2. Distingue os elementos finais dos elementos de interconexión.
3. Indica que elementos pertencen ao mapa físico.
4. Identifica no mapa lóxico as redes e enderezos que aparezan.
5. Explica o percorrido dunha comunicación entre dous equipos.
6. Detecta posibles incoherencias entre os mapas físico e lóxico.

**Entrega:** mapa anotado + explicación das conexións.

### Exercicio

Dado o seguinte escenario:

```text
Internet
   |
 Router
   |
 Switch
 /   \
PC1  PC2
 |
AP
 |
Wi-Fi
```

Indica:

1. Que elementos son dispositivos finais.
2. Que elementos son dispositivos de interconexión.
3. Que conexións son cableadas.
4. Que conexión é sen fíos.
5. Que parte do esquema representa principalmente a topoloxía física.
6. Que información adicional necesitarías para elaborar o mapa lóxico.

---

# CA1.8. Recoñecéronse as normas de seguridade e de prevención de riscos laborais no uso dos sistemas informáticos.

## 8.1. Seguridade na manipulación do hardware

Antes de manipular un equipamento:

- apagalo correctamente
- desconectalo da alimentación cando proceda
- descargar ou controlar electricidade estática
- evitar manipular compoñentes baixo tensión
- utilizar ferramentas adecuadas
  gardar parafusos e pezas pequenas
- evitar líquidos
- manter o posto ordenado
- manipular as placas polos bordos
- evitar tocar innecesariamente contactos eléctricos
- evitar forzar conectores

Ao utilizar aire comprimido, hai que evitar que os ventiladores xiren libremente a gran velocidade.

## 8.2. Electricidade estática

A electricidade estática pode danar determinados compoñentes electrónicos.

Medidas preventivas:

- utilizar os medios antiestáticos dispoñibles;
- evitar acumular cargas por fricción innecesaria;
- manipular os compoñentes de maneira adecuada;
- conservar as placas nas súas bolsas antiestáticas cando non estean instaladas.

## 8.3. Ergonomía e seguridade do posto

Tamén deben considerarse:

- postura de traballo;
- iluminación;
- organización dos cables;
- estabilidade dos equipamentos;
- ventilación;
- manipulación segura de ferramentas;
- orde e limpeza.

## Actividade A1.8 — Auditoría de seguridade dun posto

Realiza unha inspección dun posto informático.

Marca cada elemento como:

- **Correcto**
- **Cómpre mellorar**
- **Incorrecto**

| Aspecto | Estado | Medida correctora |
|---|---|---|
| Alimentación eléctrica | | |
| Cableado | | |
| Electricidade estática | | |
| Ferramentas | | |
| Postura/ergonomía | | |
| Ventilación | | |
| Orde e limpeza | | |
| Manipulación de compoñentes | | |

Finaliza cunha lista de medidas correctoras.

---

# 9. Práctica integradora do RA1

A partir dun equipamento real ou dun escenario documentado:

1. Identifica os compoñentes físicos.
2. Identifica as interfaces e mecanismos de interconexión.
3. Identifica e analiza a memoria instalada.
4. Verifica o proceso de posta en marcha.
5. Identifica e configura os periféricos dispoñibles.
6. Identifica os tipos de redes e comunicacións presentes.
7. Identifica os compoñentes da rede local.
8. Interpreta ou elabora un mapa físico e un mapa lóxico.
9. Realiza unha revisión básica das condicións de seguridade do posto.
10. Documenta os resultados.

## Informe

O informe debe conter:

1. **Inventario hardware**
2. **Memoria**
3. **Proceso de arranque**
4. **Periféricos**
5. **Rede e comunicacións**
6. **Compoñentes de rede**
7. **Mapa físico**
8. **Mapa lóxico**
9. **Seguridade e PRL**
10. **Incidencias detectadas**
11. **Medidas correctoras**


# 10. Práctica EXTRA do proceso de montaxe dun equipo (FÓRA DE PROGRAMACIÓN)

## 10.1 Documentación técnica

Antes de montar hai que consultar:

- manual da placa base;
- manual do chasis;
- documentación da CPU e disipador;
- especificacións da RAM;
- documentación da fonte;
- manuais dos SSD;
- manuais das tarxetas;
- páxinas de soporte dos fabricantes.

A documentación pode incluír:

- guía técnica;
- guía de instalación;
- manual de uso;
- esquemas de conectores;
- táboas de compatibilidade;
- procedementos de actualización;
- códigos de diagnóstico.

## 10.2. Preparación da montaxe

Antes de comezar:

1. Identificar todos os compoñentes.
2. Comprobar compatibilidade.
3. Consultar os manuais.
4. Preparar ferramentas.
5. Preparar o posto.
6. Comprobar que os separadores do chasis coinciden coa placa.
7. Determinar a orde de montaxe.

## 10.3. Instalación da CPU

1. Localizar o socket.
2. Abrir o mecanismo de retención.
3. Identificar a marca de orientación.
4. Colocar a CPU sen forza.
5. Pechar o mecanismo.
6. Comprobar visualmente.

**Nunca se debe forzar o procesador.** Se non encaixa, débese revisar a orientación e a compatibilidade.

## 10.4. Sistema de refrixeración

A CPU xera calor e necesita un sistema que a transfira ao ambiente.

Un sistema típico combina:

- superficie de contacto;
- pasta térmica;
- disipador;
- ventilador.

Procedemento:

1. Consultar o sistema de ancoraxe.
2. Preparar a superficie.
3. Aplicar a pasta térmica cando corresponda.
4. Fixar o disipador uniformemente.
5. Conectar o ventilador ao cabeceiro indicado, normalmente CPU_FAN.
6. Comprobar que ningún cable pode entrar en contacto coas aspas.

O chasis tamén debe dispoñer dun fluxo de aire adecuado:

- entrada de aire fresco;
- circulación interior;
- extracción de aire quente.

A posición exacta dos ventiladores depende do deseño do chasis.

## 10.5. Instalación da RAM

1. Consultar o manual.
2. Localizar os slots recomendados.
3. Abrir as pestanas.
4. Aliñar a muesca.
5. Inserir o módulo de maneira uniforme.
6. Comprobar que as pestanas quedan pechadas.

Para activar dual channel ou outras configuracións de canles débese seguir a disposición indicada polo fabricante.

Non se debe asumir que todos os módulos deben ser idénticos nin que calquera combinación funcionará: a compatibilidade depende da plataforma.

## 10.6. Instalación da placa base

1. Preparar os separadores.
2. Colocar o panel de E/S segundo o modelo.
3. Introducir a placa.
4. Aliñar os orificios.
5. Fixar cos parafusos adecuados.
6. Non apertar excesivamente.
7. Comprobar que non hai contacto metálico indebido.

## 10.7. Instalación da fonte

1. Colocar a fonte na orientación indicada polo chasis.
2. Fixala cos parafusos.
3. Identificar os cables necesarios.
4. Separar os cables para evitar erros.
5. Non conectar aínda os cables se a secuencia do procedemento indica facelo posteriormente.

## 10.8. Instalación de almacenamento

### SATA

Unha unidade SATA precisa habitualmente:

- cable de datos SATA;
- cable de alimentación SATA.

O procedemento é:

1. Fixar a unidade.
2. Conectar alimentación.
3. Conectar datos á unidade.
4. Conectar datos á placa.
5. Comprobar no UEFI que é detectada.

### M.2

1. Comprobar a compatibilidade do slot.
2. Introducir o módulo no ángulo indicado.
3. Baixalo.
4. Fixalo co parafuso ou mecanismo correspondente.
5. Instalar o disipador do slot se existe e procede.
6. Comprobar a detección no UEFI.

## 10.9. Tarxetas de expansión

1. Seleccionar o slot adecuado.
2. Retirar a tapa correspondente do chasis.
3. Inserir a tarxeta.
4. Fixala mecanicamente.
5. Conectar alimentación adicional se é necesaria.
6. Comprobar que non interfire con outros compoñentes.

## 10.11. Cableado do panel frontal

O panel frontal pode incluír:

- Power SW;
- Reset SW;
- Power LED;
- actividade do almacenamento;
- USB;
- audio.

O manual da placa indica a posición exacta dos cabeceiros.

Os interruptores non adoitan ter polaridade; os LEDs si.

## 10.12. Conexión da alimentación

Antes do primeiro acendido hai que comprobar:

- alimentación principal da placa;
- alimentación adicional da CPU;
- alimentación da GPU, se procede;
- alimentación das unidades SATA;
- outros conectores específicos.

Nunca se debe confiar só na forma física do conector: debe comprobarse a súa función.

## 10.13. Lista de comprobación antes do primeiro acendido

- [ ] CPU correctamente instalada.
- [ ] Disipador correctamente fixado.
- [ ] Ventilador da CPU conectado.
- [ ] RAM completamente inserida.
- [ ] Placa base correctamente fixada.
- [ ] Fonte correctamente instalada.
- [ ] Alimentación principal conectada.
- [ ] Alimentación da CPU conectada.
- [ ] Almacenamento correctamente instalado.
- [ ] GPU/tarxetas correctamente fixadas.
- [ ] Alimentación adicional da GPU conectada, se procede.
- [ ] Panel frontal correctamente conectado.
- [ ] USB/audio frontal correctamente conectado.
- [ ] Ningún cable interfire cos ventiladores.
- [ ] Non hai parafusos ou pezas soltas.
- [ ] Monitor e teclado dispoñibles.

## 10.14. Primeiro acendido

1. Conectar monitor e teclado.
2. Conectar alimentación.
3. Acender o equipamento.
4. Observar ventiladores e indicadores.
5. Acceder ao UEFI.
6. Comprobar CPU.
7. Comprobar RAM.
8. Comprobar almacenamento.
9. Comprobar temperaturas.
10. Comprobar ventiladores.
11. Continuar co arranque.

É recomendable facer esta proba antes de pechar definitivamente o chasis.

## 10.15. Inventario de hardware en Linux

Ferramentas útiles:

```bash
lscpu
lsblk
lspci
lsusb
lshw
sudo dmidecode
sudo dmidecode --type memory
```

### `lscpu`

Informa sobre:

- arquitectura;
- CPU;
- núcleos;
- fíos;
- modos de funcionamento.

### `lsblk`

Permite identificar:

- discos;
- particións;
- dispositivos de bloques.

### `lspci`

Mostra dispositivos PCI/PCI Express:

- GPU;
- controladoras;
- rede;
- audio;
- etc.

### `lsusb`

Mostra dispositivos USB detectados.

### `lshw`

Proporciona un inventario detallado do hardware.

### `dmidecode`

Permite consultar información proporcionada polas estruturas DMI/SMBIOS.


## 10.16. Diagnose da memoria

Os problemas de RAM poden provocar:

- bloqueos;
- reinicios;
- erros de aplicación;
- erros do sistema operativo;
- imposibilidade de iniciar.

Pódense utilizar ferramentas de diagnose específicas que realizan probas sobre a memoria.

A diagnose debe facerse, cando sexa necesario, fóra do sistema operativo para evitar que o propio sistema interfira na proba.

## 10.17. Metodoloxía xeral de diagnóstico

1. Definir o síntoma.
2. Determinar cando aparece.
3. Identificar cambios recentes.
4. Comprobar alimentación e conexións.
5. Consultar UEFI e indicadores.
6. Obter información do sistema operativo.
7. Formular unha hipótese.
8. Realizar unha proba.
9. Modificar unha variable.
10. Repetir a proba.
11. Documentar o resultado.

**Principio fundamental:** non se deben substituír compoñentes ao azar. Unha boa proba debe servir para distinguir hipóteses.

---


# 11. Práctica EXTRA de Identificación e inventario dun PC (FÓRA DE PROGRAMACIÓN)

## 11.1. Actividade A. Inventario dun PC

1. Abrir o chasis aplicando as medidas de seguridade.
2. Identificar placa base.
3. Identificar CPU.
4. Identificar RAM.
5. Identificar almacenamento.
6. Identificar fonte.
7. Identificar GPU.
8. Localizar SATA.
9. Localizar M.2.
10. Localizar PCIe.
11. Localizar conectores de alimentación.
12. Identificar portos externos.
13. Elaborar unha ficha técnica.

**Resultado:** esquema/fotografía anotada + inventario.

## 11.2. Actividade B. Interpretación dun manual

Localizar no manual:

- CPU compatibles;
- RAM compatible;
- capacidade máxima;
- slots recomendados;
- M.2;
- SATA;
- PCIe;
- alimentación;
- CPU_FAN;
- CHA_FAN;
- panel frontal;
- USB;
- audio;
- procedemento de actualización do firmware;
- indicadores de diagnóstico.

**Resultado:** ficha técnica indicando onde se atopa cada dato.

## 11.3. Actividade C. Montaxe completa

1. Preparar posto.
2. Consultar manuais.
3. Montar CPU.
4. Montar refrixeración.
5. Montar RAM.
6. Montar placa.
7. Montar fonte.
8. Montar almacenamento.
9. Montar GPU/tarxetas.
10. Conectar cableado.
11. Completar checklist.
12. Realizar primeiro acendido.
13. Acceder ao UEFI.
14. Comprobar detección.
15. Documentar incidencias.

## 11.4. Actividade D. Inventario en Linux

Executar:

```bash
lscpu
lsblk
lspci
lsusb
sudo lshw -short
sudo dmidecode --type system
sudo dmidecode --type memory
```

Elaborar unha táboa:

| Elemento | Información |
|---|---|
| CPU | Modelo, arquitectura, núcleos/fíos |
| RAM | Capacidade, módulos, velocidade |
| Placa | Fabricante, modelo, firmware |
| Almacenamento | Modelo, interface, capacidade |
| GPU | Modelo e interface |
| Rede | Adaptadores |
| USB | Dispositivos detectados |

## 11.5. Actividade E. Diagnose

**Situación:** o equipo acende pero non aparece imaxe.

Seguir unha secuencia:

1. Comprobar monitor.
2. Comprobar entrada seleccionada.
3. Comprobar cable.
4. Comprobar onde está conectado o monitor.
5. Comprobar GPU.
6. Comprobar alimentación da GPU.
7. Comprobar RAM.
8. Observar indicadores da placa.
9. Consultar manual.
10. Probar configuración mínima.
11. Documentar hipótese, proba e resultado.

## 11.6. Actividade F. Instalación de periféricos

Instalar e verificar varios dispositivos:

- teclado USB
- rato USB
- monitor
- audio
- rede
- almacenamento externo
- Bluetooth/Wi-Fi, cando estea dispoñible

Para cada dispositivo documentar:

- función
- interface
- conexión
- detección
- controlador
- configuración
- proba
- resultado


---

# 12. Conceptos que deben quedar claros

1. Hardware é a parte física; software son instrucións e datos.
2. A placa base interconecta os principais compoñentes.
3. A CPU executa; a RAM mantén temporalmente datos e instrucións en uso.
4. RAM é volátil; o almacenamento persistente non.
5. M.2 é un formato/conector; NVMe é un protocolo.
6. PCIe é unha interconexión baseada en enlaces e carrís.
7. USB-C é un conector físico e non define por si só a velocidade.
8. UEFI é firmware.
9. Secure Boot é unha función de seguridade da cadea de arranque.
10. O POST forma parte da inicialización, non do sistema operativo.
11. A documentación do fabricante é parte do procedemento técnico.
12. Un diagnóstico debe partir de síntomas e probas.

---


## Checklist final

- [ ] Identifico CPU, placa base, RAM, almacenamento, fonte e GPU.
- [ ] Identifico PCIe, SATA, USB e outras interfaces relevantes.
- [ ] Sei diferenciar M.2 e NVMe.
- [ ] Sei identificar o tipo e as características básicas da RAM.
- [ ] Sei explicar a secuencia básica de posta en marcha.
- [ ] Sei interpretar o papel do POST e do UEFI.
- [ ] Sei clasificar e instalar periféricos.
- [ ] Sei distinguir LAN, WLAN, PAN, MAN e WAN.
- [ ] Sei identificar switch, router, access point e adaptadores de rede.
- [ ] Sei distinguir un mapa físico dun mapa lóxico.
- [ ] Sei interpretar un esquema básico de rede.
- [ ] Aplico normas básicas de seguridade e PRL.
- [ ] Sei documentar as comprobacións e os resultados realizados.

