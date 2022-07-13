---
ms.localizationpriority: medium
ms.openlocfilehash: 3c4731d0d1b8f6f7015387fee6a59e3a3d8f1883
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768189"
---
<!-- markdownlint-disable MD002 MD041 -->

Um administrador do Microsoft 365 tem a capacidade de aprovar ou negar solicitações de consentimento. Isso pode ser feito por meio do Administração Microsoft 365 Center ou programaticamente por meio do PowerShell.

## <a name="approve-consent-requests"></a>Aprovar solicitações de consentimento

# <a name="microsoft-365-admin-center"></a>[Administração Microsoft 365 Central](#tab/Microsoft365)

1. Abra um navegador e vá para o [Administração Microsoft 365 Portal](https://admin.microsoft.com).

1. Para aprovar ou negar solicitações de consentimento, vá para [Acesso Privilegiado](https://portal.office.com/adminportal/home#/Settings/PrivilegedAccess).

1. Selecione uma solicitação de **acesso a dados pendente**.

1. Na chamada **solicitação de acesso** a dados, selecione o **botão** Aprovar.

    ![Uma captura de tela mostrando uma solicitação de acesso a dados com aprovação de consentimento pendente no Centro de administração do Microsoft 365.](../concepts/images/data-connect-m365-approve.png)

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

1. Abra o PowerShell do Windows.
1. Verifique se a sessão do PowerShell habilitou scripts assinados remotamente.

    ```powershell
    Set-ExecutionPolicy RemoteSigned
    ```

1. Conecte-se Exchange Online.

    1. Obtenha uma credencial de entrada executando o PowerShell a seguir. Entre usando um usuário diferente do que criou e iniciou o pipeline do Azure Data Factory, que tem **a função Administrador global** aplicada, que é membro do grupo que tem direitos para aprovar solicitações de dados no Microsoft 365 e tem a autenticação multifator habilitada.

        ```powershell
        $UserCredential = Get-Credential
        ```

    1. Crie uma nova sessão Exchange Online PowerShell e carregue -a (importe).

        ```powershell
        $Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://ps.protection.outlook.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection
        Import-PSSession $Session -DisableNameChecking
        ```

        > [!IMPORTANT]
        > Depois de concluir esta sessão, desconecte-se da sessão usando o comando do PowerShell `Remove-PSSession $Session`. Exchange Online permite apenas três sessões remotas abertas do PowerShell para proteção contra ataques de Negação de Serviço (DoS). Se você simplesmente fechar a janela do PowerShell, ela deixará a conexão aberta.

1. Obtenha uma lista de todas as solicitações de dados pendentes da conexão de dados do Microsoft Graph executando o PowerShell a seguir.

    ```powershell
    Get-ElevatedAccessRequest | where {$_.RequestStatus -eq 'Pending'} | select RequestorUPN, Service, Identity, RequestedAccess | fl
    ```

    - Examine a lista de solicitações de acesso a dados retornadas. Na imagem a seguir, observe que há duas solicitações pendentes.

        ![Uma captura de tela mostrando uma lista de solicitações pendentes formatadas como uma lista em um console do PowerShell.](../concepts/images/data-connect-ps-pending-requests.png)

1. Aprove um acesso a dados retornado na etapa anterior copiando o GUID de identidade de uma solicitação executando o PowerShell a seguir.

    > [!NOTE]
    > Substitua o GUID no snippet de código a seguir pelo GUID dos resultados da etapa anterior.

    ```powershell
    Approve-ElevatedAccessRequest -RequestId fa041379-0000-0000-0000-7cd5691484bd -Comment 'approval request granted'
    ```

1. Após alguns instantes, você deverá ver a página de status da atualização de execução de atividade para mostrar que agora está _extraindo dados_.

    ![Uma captura de tela mostrando portal do Azure interface do usuário do serviço Data Factory em que o status da carga agora é exibido como "Extraindo dados".](../concepts/images/data-connect-adf-extraction-approved.png)

1. Esse processo de extração dos dados pode levar algum tempo, dependendo do tamanho do locatário do Microsoft 365.

---

## <a name="verify-extracted-data-from-microsoft-365-to-azure-storage-blob"></a>Verificar dados extraídos do Microsoft 365 para o Blob de Armazenamento do Azure

1. Abra um navegador e vá para o [Portal do Azure](https://portal.azure.com/).

1. Entre usando uma conta com direitos **Administrador global** seus locatários do Azure e do Microsoft 365.

1. Na navegação da barra lateral, selecione o item **de menu Todos os** recursos.

1. Na lista de recursos, selecione a conta **de Armazenamento do Azure** criada anteriormente neste tutorial.

1. No menu de navegação da barra lateral, selecione **Blobs** na folha **da conta de Armazenamento do Azure** .

1. Selecione o **contêiner** criado anteriormente neste tutorial que você configurou o pipeline Azure Data Factory como o coletor para os dados extraídos. Você deve ver os dados neste contêiner agora.

    ![Uma captura de tela mostrando a portal do Azure interface do usuário do serviço de conta de armazenamento. Ele está mostrando o contêiner onde os dados extraídos estão sendo armazenados.](../concepts/images/data-connect-adf-extracted-data-in-blob.png)
