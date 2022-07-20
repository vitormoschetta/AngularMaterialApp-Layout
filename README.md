### Créditos / Referência / Tutorial:

<https://devdactic.com/angular-material-app-capacitor/>

### Resumo de comandos do tutorial acima

De posse de um App Angular pronto, seguir:

#### Instalar `capacitor/cli` e `capacitor/core`:
  npm install @capacitor/cli @capacitor/core

#### Inicializar configurações:
  npx cap init

O comando acima criar um arquivo `capacitor.config.ts`

#### Instalar pacotes `ios` e `android`:
  npm install @capacitor/ios @capacitor/android

#### Inicializar um projeto Android:
O projeto Android deve ser criado já com os arquivos Angular como base, para isso precisamos buildar o Angular App:
  ng build

O comando acima gera uma pasta `dist/<nome-do-app`. É importante atualizar o arquivo `capacitor.config.ts`, na linha `webDir: 'dist/<nome-do-app'`, 
para que o capacitor pegue os arquivos na pasta correta.

Na sequência, gerar o projeto android:
  npx cap add android

O comando acima cria uma pasta `android` já com o seu aplicativo Angular.

Se for necessário atualiar o App Angular, faça um novo `ng build` e execute um `npx cap sync`.

Com o Android Studio instalado, agora abra o projeto com o seguinte comando: `npx cap open android`. Se não tiver o Android Studio, o próximo bloco tem uma referencia para a instalação.


### Instalação do Android Studio:

<https://balta.io/>

Se cadastrar e pegar videos de configurações iniciais do curso gratuito de Flutter. Ele ensina como instalar o Android Studio e criar uma VM para um dispositivo móvel.


### Como gerar uma APK pelo Android Studio para publicar na Play Store 

<https://www.youtube.com/watch?v=_6a_nPFu05E>


###  Como publicar o seu aplicativo na PlayStore

<https://www.youtube.com/watch?v=RVv9CbmNnE0>


### Rebuildar e publicar nova versão

Atualiar `versionCode` e  `versionName` no arquivo `build.gradle`     


### Para mais detalhes sobre Capacitor e Ionic:

<https://capacitorjs.com/solution/angular>
<https://ionicframework.com/docs/>
