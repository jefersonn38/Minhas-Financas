# Minhas Finanças — como gerar o APK

Você não precisa instalar nada no computador. O GitHub compila o APK de graça.

## Passo a passo
1. Crie uma conta gratuita em https://github.com (se ainda não tiver).
2. Clique em **New repository**, dê um nome (ex.: minhas-financas) e crie.
3. Clique em **uploading an existing file** e envie TODO o conteúdo desta pasta, mantendo as pastas `www` e `.github/workflows`.
   (Dica: se o navegador não enviar a pasta oculta `.github`, crie o arquivo pelo botão **Add file > Create new file**, digitando `.github/workflows/build-apk.yml` e colando o conteúdo do arquivo.)
4. Abra a aba **Actions**. O build começa sozinho (leva uns 5 a 10 minutos). Se não começar, escolha **Gerar APK > Run workflow**.
5. Quando ficar verde, abra a execução e baixe o arquivo **minhas-financas-apk** (vem em .zip, dentro está o `app-debug.apk`).

## Instalar no Android
1. Envie o `app-debug.apk` para o celular (WhatsApp, e-mail, Drive).
2. Toque no arquivo e permita **instalar de fontes desconhecidas** quando o Android pedir.
3. Pronto: o ícone "Minhas Finanças" aparece no celular.

## Distribuir para testadores
Mande o mesmo arquivo `app-debug.apk` para quem vai testar. Cada pessoa tem seus próprios dados, guardados só no aparelho dela.

## Observações
- Este é um APK de teste (assinado com chave de depuração). Serve para instalar e testar, mas não para publicar na Google Play.
- Para publicar na Play Store é preciso gerar um pacote assinado (AAB) com sua própria chave. Posso ajudar nisso depois.
- Ao atualizar o app, troque o arquivo `www/index.html` no GitHub e o APK é gerado de novo.
- Desinstalar o app apaga os dados. Use "Copiar backup" nas configurações antes.
