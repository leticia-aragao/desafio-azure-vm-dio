# Desafio Azure VM - DIO

## 📌 Descrição
Este projeto faz parte do desafio prático proposto no bootcamp da DIO, com o objetivo de consolidar conhecimentos sobre máquinas virtuais no Microsoft Azure.

## 📝 Etapas
1. No portal do Azure, digite “Máquinas Virtuais” e clique no resultado. Clique em "Criar" e "Máquina Virtual".
   
2. Na aba "Básico", definimos as configurações básicas da VM:
   - Assinatura: selecione qual plano de assinatura será usado (pago ou gratuito, por exemplo).
   - Grupo de Recursos: criar um novo para agrupar os recursos do projeto.
   - Nome da VM: criar um nome para identificar sua máquina.
   - Região: onde a VM será hospedada. escolha a mais próxima ou com disponibilidade gratuita.
   - Opções de disponibilidade: define o nível de alta disponibilidade da sua VM.
   - Opções de zona: especificar se deseja usar zonas de disponibilidade escolhidas por você ou pela Azure.
   - Zona de disponibilidade: define quais zonas físicas da região serão usadas.
   - Tipo de segurança: define o nível de segurança da sua VM.
   - Imagem: escolher o sistema operacional (Windows Server 2022, Ubuntu 20.04, etc).
   - Tamanho: tipo de hardware virtual. Determina fatores como capacidade de processamento, memória e capacidade de armazenamento.
   - Tipo de Autenticação: escolha se usará o nome de usuário/senha ou chaves SSH para a autenticação.
   - Usuário e senha/chave SSH: Define as credenciais para acessar a máquina (Windows usa senha; Linux geralmente usa chave SSH).
   - Portas de entrada públicas: Selecione quais portas de rede da máquina virtual podem ser acessadas pela internet pública.

3. Na aba "Discos", definimos o tipo e a performance do disco rígido virtual:
   - Tipo de disco de SO: Pode ser SSD (rápido, mas mais caro) ou HDD (mais barato, porém mais lento).
   - Discos de dados: pode adicionar e configurar discos de dados adicionais para a VM ou anexar discos existentes.

4. Na aba "Rede", permite que a VM se conecte à internet:
   - O Azure cria uma rede virtual (VNet) automaticamente.
   - Selecione as portas de entrada: Windows: habilite a porta 3389 (RDP). Linux: habilite a porta 22 (SSH).

5. Na aba "Gerenciamento", permite definir como a VM será monitorada e protegida:
   - Você pode ativar ou desativar recursos como: monitoramento de desempenho, atualizações automáticas e backup.
   - Se estiver apenas testando, pode deixar tudo padrão ou desativar para reduzir consumo de recursos.

6. Na aba "Monitoramento", permite ativar serviços que acompanham o desempenho da VM:
   - Diagnóstico de inicialização: Útil para solucionar problemas de falha de inicialização de imagens personalizadas ou de plataforma.
   - Diagnóstico de convidado do SO: obter métricas para sua máquina virtual a cada minuto.
   - Para testes ou laboratórios simples, pode deixar desativado para economizar recursos.

7. Na aba "Avançado", permite configurar scripts de inicialização, extensões e outras opções avançadas:
   - Para uso iniciante/teste, pode ignorar e seguir para a próxima aba.

8. Na aba "Marcas", são pares de nome/valor que permitem classificar recursos:
   - Útil em empresas com muitos recursos.
   - Opcional, mas boa prática incluir no projeto.

9. Na aba “Revisar + Criar”, confirma se tudo está certo antes de criar a máquina:
   - O Azure vai validar as configurações.
   - Se estiver tudo OK, clique em “Criar”.
  
10. Acessar a VM:
    - Clique em “Ir para o recurso” depois da criação.
    - Clique em “Conectar”:
        - Para Windows, escolher RDP, baixe o arquivo e abrir no seu computador.
        - Para Linux, usar o comando SSH sugerido no terminal.
