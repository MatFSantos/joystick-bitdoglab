# Instruções de uso

Para uso do software, siga os seguintes passos:

- **1°:** clone o repositório para o seu computador.

    - Ao abrir o projeto com o **VSCode**, a extensão do **CMake** irá criar a pasta ``build`` para você com os arquivos de compilação.

    - Caso não seja gerada a pasta, crie uma pasta com nome `build` e execute o seguinte comando dentro da pasta criada:
        
        ``cmake ..``

        O comando acima irá criar os arquivos de compilação.
        
        > Você pode também seguir para o passo 2 sem executar o passo anterior

- **2°:** execute a compilação do firmware usando a extensão do ***Raspberry Pi Pico*** do ***VSCode***.

A partir daqui, seu firmware já está compilado e pronto para uso, e só depende de onde será usado.

## Execução na *BitDogLab*

Siga os passos a seguir para poder executar seu firmware na placa *BitDogLab*:

- **1°:** coloque o seu ***Raspberry*** em modo de ***bootsel***, clicando no botão branco na placa e reiniciando a mesma.

- **2°:** copie o arquivo `.uf2` que foi gerado na pasta `build` para o seu ***Raspberry*** (ele aparecerá como um armazenamento externo, um Pen-Drive com nome de RPI-RP2).

    - Após isso, o seu código já vai está rodando na sua plaquinha ***BitDogLab***.

- **3°:** Está pronto, dê os comandos para executar as funcionalidades clicando nas teclas do seu teclado.

## Instruções para uso do firmware

O firmware que o código gera, faz uso do botão A e o botão do **Joystick** da placa de desenvolvimento, presentes nos pinos 5 e 22 do **Raspberry Pi Pico W**,além do display **SSD1306** que faz uso do canal de comunicação I2C, presente nos pinos 14 (*SDA*) e 15 (*SCL*). Também faz uso do LED RGB, presentes nos pinos 11, 12 e 13, e dos potenciômetros conectados ao **Joystick**, ligados aos pinos 27 (eixo X) e 26 (eixo Y).

Ao mover o **Joystick** no eixo X, poderá ser observado o LED vermelho aumentando sua intensidade a medida que se afasta do centro. O mesmo acontece com o LED azul, caso o eixo Y seja movimentado. Em união com esse comportamento, é possível ver um quadrado no **Display** que segue o movimento do **Joystick**.

O **botão A** habilita e desabilita os LEDs azul e vermelho, já o botão do **Joystick** altera o estado do LED verde, além de modificar a borda que é apresentada no **Display**.

## Vídeo Ensaio

Clique em ***[link do video](https://drive.google.com/file/d/1b43aFzuZxrxSeato3uNGRyhxHl_tkZRX/view?usp=sharing)*** para visualizar o vídeo ensaio do projeto.
