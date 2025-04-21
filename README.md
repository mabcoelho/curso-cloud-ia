# Criar uma Máquina Virtual Windows no Azure
Passos Principais:
Acessar o Portal do Azure

Entre no Portal do Azure.

Crie uma conta gratuita se não tiver assinatura.

Criar a Máquina Virtual (VM)

Pesquise por "Máquinas Virtuais" e selecione "Criar" → "Máquina Virtual do Azure".

Configure:

Nome da VM: myVM.

Imagem: Windows Server 2022 Datacenter.

Credenciais: Defina um usuário (ex: azureuser) e senha complexa.

Portas de entrada: Libere RDP (3389) e HTTP (80).

Valide e clique em "Criar".

Conectar-se à VM via RDP

Na página da VM, selecione "Conectar" → RDP.

Baixe o arquivo RDP e faça login com as credenciais definidas.

Instalar Servidor Web (IIS)

Abra o PowerShell na VM e execute:

powershell
Install-WindowsFeature -name Web-Server -IncludeManagementTools
Acesse o IP público da VM no navegador para ver a página padrão do IIS.

Gerenciar Recursos

Exclua o grupo de recursos se não for mais necessário.

Configure desligamento automático para economizar custos.
