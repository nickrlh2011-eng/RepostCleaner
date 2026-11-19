# Repost Cleaner – protótipo Android

Projeto Android nativo em Kotlin. Inclui uma interface inicial e um serviço de acessibilidade experimental que só procura rótulos conhecidos de “Remover republicação” no TikTok e exige confirmação antes do toque.

## Gerar o APK usando apenas o celular
1. Crie uma conta no GitHub, se ainda não tiver.
2. Crie um repositório novo e envie todos os arquivos desta pasta (incluindo a pasta oculta `.github/workflows`).
3. Abra a aba **Actions** do repositório.
4. Se solicitado, habilite GitHub Actions.
5. Execute **Build Repost Cleaner APK** em **Run workflow**, ou aguarde o build após enviar os arquivos.
6. Quando terminar, abra a execução e baixe o artefato `repost-cleaner-debug-apk`.
7. Extraia o ZIP do artefato para obter `app-debug.apk` e instale-o no Android.

## Uso
1. Abra Repost Cleaner.
2. Toque em “Ativar acessibilidade” e ative o serviço nas configurações do Android.
3. Volte ao app e abra o TikTok.
4. Navegue até suas republicações.
5. Se o serviço reconhecer a opção de remover, ele mostrará uma confirmação. Confirme apenas se o texto e o vídeo estiverem corretos.

## Limitações
- É um protótipo; a interface/idioma do TikTok pode mudar e impedir a detecção.
- Não percorre automaticamente toda a lista nem garante exclusão em massa.
- Não pede senha, não tem permissão de internet e não envia dados.
- A permissão de acessibilidade é sensível. Revise o código e desative o serviço quando não estiver usando.
- O APK gerado pelo fluxo é de depuração, não uma versão publicada/assinada para distribuição.
