# sunboxs
scripts of solar data!
## Índice

1. [Escopo do Projeto](#escopo-do-projeto)
2. [Resumo](#resumo)
3. [Motivação](#motivação)
4. [Premissas](#premissas)
5. [Objetivos](#objetivos)
6. [Arquivos e Pastas](#arquivos-e-pastas)
7. [Execução do Algoritmo](#execução-do-algoritmo)
8. [Conclusão](#conclusão)

&nbsp;

## Escopo do Projeto <a id="escopo-do-projeto"></a>

Aplicação prática de detecção de sonolência em tempo real.


## Resumo <a id="resumo"></a>

Este projeto consiste na aplicação prática de detecção de sonolência em tempo real usando visão computacional. A detecção de sonolência é uma técnica consolidada com um impacto significativo em áreas como gestão de frotas, contribuindo para evitar acidentes. O objetivo principal é treinar um modelo personalizado para a detecção de sonolência, aplicando uma metodologia bem definida.
&nbsp;

## Motivação <a id="motivação"></a>

Este projeto tem como objetivo criar uma aplicação prática que possa ser usada em apresentações, visitas e workshops, mostrando a capacidade do Hub em criar soluções úteis. Embora a metodologia seja estabelecida, o foco está no desenvolvimento de um modelo próprio de detecção de sonolência, diferenciando-o dos modelos já disponíveis. A motivação subjacente é impulsionada por uma preocupação fundamental: a segurança e bem-estar das pessoas. A detecção de sonolência em tempo real é um problema de extrema importância, não apenas para motoristas, mas também em diversas outras aplicações. No contexto de motoristas, a sonolência é uma das principais causas de acidentes de trânsito em todo o mundo. Além do trânsito rodoviário, a detecção de sonolência tem aplicações em diversas outras áreas, como a operação de maquinário pesado em setores industriais, e pode contribuir para a saúde individual, alertando sobre distúrbios do sono. Ao demonstrar uma solução tangível, estamos contribuindo para a educação pública e para a promoção de comportamentos mais seguros e saudáveis, tornando esta iniciativa um passo crucial em direção a um ambiente mais seguro e consciente.

&nbsp;

## Premissas <a id="premissas"></a>

* O projeto treina um novo modelo e visa implantá-lo na web.
* O algoritmo de treinamento para detecção de landmarks está disponível em http://dlib.net/train_shape_predictor.py.html.

&nbsp;

## Objetivos <a id="objetivos"></a>

* Aplicar a metodologia de detecção de sonolência.
* Treinar um modelo personalizado para caracterização da sonolência.
* Utilizar um dataset público.
* Parametrizar o modelo e realizar testes.
* Nomear o modelo treinado.

&nbsp;

## Arquivos e Pastas <a id="arquivos-e-pastas"></a>

O diretório do projeto está dividido da seguinte maneira:

* **data**: pasta que deve conter o dataset de treinamento e teste e o arquivo de áudio do sinalizador de sonolência.

* **model**: pasta que contém modelo de landmarks treinado;

* [main.py](main.py): arquivo principal para executar a detecção de sonolência em tempo real.

* [ear.py](ear.py): módulo para calcular o EAR (Eye Aspect Ratio) usado na detecção de sonolência.

* [mar.py](mar.py): módulo para calcular o MAR (Mouth Aspect Ratio) usado na detecção de bocejos.

* [moe.py](moe.py): módulo para calcular o MOE (Mouth Over Eye) usado na detecção de bocejos.

* [landmarks.py](landmarks.py): algoritmo de treinamento do modelo dlib de detecção de landmarks;

* [requirements.txt](requirements.txt): lista de bibliotecas requeridas para execução do projeto;

* [.gitignore](.gitignore): arquivo que contém os nomes dos arquivos e pastas que devem ser ignorados pelo *Git*;

* [README.md](README.md) : arquivo descrevendo detalhes do projeto.

&nbsp;

## Execução do Algoritmo <a id="execução-do-algoritimo"></a>

Para que o programa funcione, é fundamental instalar via pip todas as bibliotecas listadas no arquivo [requirements.txt](requirements.txt). Para isso, basta executar no terminal:

> pip install -r requirements.txt

Em seguida, executar o arquivo 'main.py' para iniciar a detecção de sonolência em tempo real.

&nbsp;

## Conclusão <a id="conclusão"></a>

Este projeto visa aplicar de forma prática a detecção de sonolência em tempo real usando visão computacional. O foco principal é treinar um modelo personalizado para a detecção de sonolência e implementá-lo em uma aplicação web. A detecção de sonolência é um problema importante e a metodologia proposta oferece uma abordagem eficaz para enfrentá-lo.
