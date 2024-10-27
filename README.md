# Configuração de Rede Local Básica no Windows 10

Este projeto guia o usuário na configuração de uma rede local (LAN) básica no Windows 10, permitindo o compartilhamento de arquivos e dispositivos (como impressoras) entre computadores na mesma rede.

## Pré-requisitos

- Computadores com Windows 10 conectados à mesma rede (roteador ou switch), seja por Wi-Fi ou cabo Ethernet.
- Permissões de administrador no sistema para realizar as configurações.

## Passo a Passo

### 1. Configurar a Rede no Windows 10

1. **Definir a Rede como Privada**:
   - Vá para **Configurações > Rede e Internet > Status.
   - Clique em **Propriedades da Conexão** e selecione **Rede Particular**. Isso permite que os dispositivos na mesma rede sejam detectados.

2. **Ativar a Descoberta de Rede e o Compartilhamento de Arquivos**:
   - Acesse **Configurações > Rede e Internet > Status > Central de Rede e Compartilhamento**.
   - Clique em **Alterar as configurações de compartilhamento avançadas**.
     - Em **Particular(perfil atual)**, selecione **Ativar descoberta de rede** e **Ativar o compartilhamento de arquivos e impressoras**.
     - Em **Todas as redes**, selecione **Desativar compartilhamento protegido por senha** (opcional, para facilitar o acesso de todos na rede).
     - E clique em "Salvar alterações".

### 2. Compartilhar Pastas na Rede

1. Abra o **Explorador de Arquivos** e vá até a pasta que deseja compartilhar, ou crie uma para testes com algum documento vazio.
2. Clique com o botão direito na pasta, selecione **Propriedades** e vá para a aba **Compartilhamento**.
3. Clique em **Compartilhar** e escolha **Todos** para compartilhar com qualquer dispositivo na rede.
4. Defina o nível de permissão:
   - **Leitura**: Permite visualizar arquivos.
   - **Leitura/Gravação**: Permite visualizar e modificar arquivos.
5. Clique em **Compartilhar** e depois em **Concluído**.

### 3. Acessar Pastas Compartilhadas em Outro Computador

Existem duas formas para acessar a pasta compartilhada a partir de outro dispositivo Windows na mesma rede:

1ª Forma:

    - Abra o **Explorador de Arquivos** e clique em **Rede** na barra lateral para ver os dispositivos conectados na LAN.
    - Clique no nome do computador onde a pasta foi compartilhada para ver as pastas e arquivos disponíveis.

2ª Forma:

    - Pressione os atalhos de teclado Windows + R, para abrir a janela do "Executar".
    - Digite o ip do computador para acessar a pasta compartilhada e dê Enter. Ex: "\\192.168.1.1"
    Obs: Sem usar as aspas, informando o ip da máquina.

### Solução de Problemas

- **Dispositivo não aparece na rede**:
  - Certifique-se de que a rede está configurada como **Privada**.
  - Verifique se a **descoberta de rede** e o **compartilhamento de arquivos** estão ativados.

- **Erro ao acessar pastas compartilhadas**:
  - Verifique as permissões de compartilhamento e o nível de acesso configurado.
  - Caso tenha desativado o **compartilhamento protegido por senha**, isso pode ajudar a evitar problemas de permissão.

## Autor

Este projeto foi desenvolvido como um guia para configurar uma rede local básica no Windows 10.

## Licença

Este projeto está licenciado sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.
