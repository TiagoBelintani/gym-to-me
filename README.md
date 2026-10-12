# Gym To Me — aplicativo Android (PWA)

Aplicativo estático que registra os treinos ABCDE, peso e repetições de cada série, conclusão, histórico e gráfico de evolução. Os dados ficam em `localStorage` no aparelho. Não requer login, backend nem cobrança.

## Como instalar no Android com GitHub Pages

1. Crie um repositório GitHub, por exemplo `gym-to-me` (pode ser público; **não inclua registros pessoais** nele).
2. Envie **os arquivos desta pasta** para a raiz do repositório (não envie só o ZIP).
3. Em **Settings → Pages → Build and deployment**, selecione **Deploy from a branch**, **main**, **/(root)** e salve.
4. Abra no Chrome do Android o link fornecido pelo GitHub Pages: `https://SEU-USUARIO.github.io/gym-to-me/`.
5. Menu **⋮ → Adicionar à tela inicial → Instalar**, conforme as opções disponíveis no Chrome.
6. Abra uma vez com internet para fazer cache dos arquivos; o app funcionará offline depois disso.

Para testar no computador, sirva a pasta com `python3 -m http.server 8000` e abra `http://localhost:8000`. O Chrome pode registrar service worker no localhost.

## Limitações e segurança

- Os dados **não** sincronizam entre aparelhos: faça backup JSON regularmente em **Ajustes → Exportar backup**.
- Limpar dados do Chrome, desinstalar o PWA ou mudar de navegador pode apagar o histórico.
- Carga em kg: decida uma convenção para exercícios com dois halteres (peso por halter ou total) e mantenha-a para comparação.
- Prancha: use a coluna repetições para segundos; campo kg pode ficar vazio.
- O aplicativo **não prescreve** alterações de treino e não substitui supervisão profissional.
