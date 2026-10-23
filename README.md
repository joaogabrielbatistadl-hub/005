# exemplo-git-parte2
| comandos git-da-silva | descrição |
| --- | --- |
 | git remote -v | aparece o histórico e a origem do repositório ou algo do tipo. | 
| git remote remove origin | altera a origem do git. |
git remote add origin (link do repositório novo) | substitui a origem do repositório pela a que você escolher.
git config --global user.name "SEU nick do git"  | Serve para não mostrar os dados de login do seu computador local quando você der commit (isso acontece mesmo com você logado no VScode).
git config --global user.email "SEU email do git" | A mesma coisa só que por e-mail da maquina.
Remove-Item -Recurse -Force .git | Apaga o histórico do repositório clonado de uma forma mais "elegante" e ariscada (ele pode deletar até as .git que n devem ser deletadas).
git init | Inicia um .git novo na pasta desejada.
git branch -M main | Renomeia o "master" que o git init cria para "main" não ficar 2 brachs criadas.
git remote add origin (link do repositório) | Adiciona uma origem para a nova pasta .git que tu deletou.
git push -f origin main | Ignora o que está na nuvem e força a substituição do arquivo (não recomendado para estagiários).
git checkout -b (nome da branch) | Cria uma nova branch (usando o -b) e troca pra ela (não colocar acento, espaço e caracteres especiais no nome). Para mudar para outro branch é só colocar o nome dele E REMOVER o -b
git push origin (nome da branch) | Atualiza a branch selecionada.
git merge (nome da branch) | Junta a branch atual com a branch selecionada.

OBS:
Se você entrar na pasta clonada, clicar em visualizar, mostrar e depois em itens ocultos: você consegue ver todos os commits do repositório.

Mesmo depois de você substituir a origem do repositório para a origem que você escolher, quando você upar o arquivo para o seu repositório do Github, o criador original do repositório vai aparecer como contribuidor. Você precisa alterar os arquivos na pasta do repositório do seu computador (usando a explicação acima) e remover o criador original dos arquivos da pasta para ele não aparecer como contribuidor.

Para apagar o histórico de uma de negocio clonado é só deletar a pasta .git usando os coisas acima.

Caso você não use o -b no comando, ele tentará selecionar uma branch que não foi criada
