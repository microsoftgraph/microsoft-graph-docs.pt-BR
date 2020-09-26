---
title: Permitir que o Applicatiosn acesse reuniões online em nome de um usuário
description: Descubra como configurar aplicativos para acessar reuniões online em nome de um usuário.
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: fc96bd7958fd2729c9222bdb88b50fb04608732a
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289460"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a>Permitir que os aplicativos acessem reuniões online em nome de um usuário

Em alguns casos, como nos serviços em segundo plano ou em aplicativos de daemon executados em um servidor sem a presença de um usuário conectado, é apropriado para um aplicativo chamar o Microsoft Graph para executar ações em nome de um usuário. Por exemplo, um aplicativo pode precisar chamar o Microsoft Graph para agendar várias reuniões com base em agendas publicadas (como cursos) ou em ferramentas de agendamento externas. Nesses casos, o usuário que o aplicativo atua em nome do é identificado como organizador da reunião.

Os administradores que desejam permitir que um aplicativo acesse recursos de reunião online em nome de um usuário podem usar os cmdlets **New-CsApplicationAccessPolicy** e **Grant-CsApplicationAccessPolicy** do PowerShell para configurar o controle de acesso. Este artigo aborda as etapas básicas para configurar uma política de acesso a aplicativos.

Estas etapas são específicas para reuniões online e não se aplicam a outros recursos do Microsoft Graph.

## <a name="configure-application-access-policy"></a>Configurar a política de acesso do aplicativo

Para configurar uma política de acesso de aplicativo e permitir que os aplicativos acessem reuniões online com permissões de aplicativo:

1. Identifique a ID do applcation (cliente) do aplicativo e as IDs de usuário dos usuários em nome do qual o aplicativo será autorizado a acessar reuniões online.

    - Identifique o ID do aplicativo (cliente) do aplicativo no [portal de registro de aplicativos do Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).
    - Identificar a ID de usuário (objeto) do usuário no [portal de gerenciamento de usuários do Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)

2. Conecte-se ao Skype for Business PowerShell com a conta Adminitrator. Para obter detalhes, consulte [gerenciar o Skype for Business online com o PowerShell](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell).

3. Crie uma política de acesso de aplicativo contendo uma lista de IDs de aplicativos.

    Execute o cmdlet a seguir, substituindo os argumentos **identidade**, **APPIDs**e **Description** (opcional).

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. Conceda a política ao usuário para permitir que as IDs de aplicativo contidas na política acessem reuniões online em nome do usuário concedido. 

   Execute o cmdlet a seguir, substituindo os argumentos **PolicyName** e **Identity** .

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "ddb80e06-92f3-4978-bc22-a0eee85e6a9e"
   ```

> **Observação** 
> 
> - _Identity_ se refere ao nome da política ao criar a política, mas a ID de usuário ao conceder a política.
> - As alterações nas políticas de acesso de aplicativos podem levar até 30 minutos para entrar em vigor nas chamadas da API REST do Microsoft Graph.

## <a name="supported-permissions-and-additional-resources"></a>Permissões compatíveis e recursos adicionais

Os administradores podem usar cmdlets do ApplicationAccessPolicy para controlar o acesso de caixa de correio de um aplicativo que recebeu qualquer uma das seguintes permissões de aplicativo:

- OnlineMeetings.Read.All
- OnlineMeetings.ReadWrite.All

Para obter mais informações sobre como configurar a política de acesso a aplicativos, consulte a [referência de cmdlet do PowerShell para New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).

## <a name="errors"></a>Erros

Você pode encontrar o seguinte erro quando uma chamada à API tem acesso negado devido a um aplicativo tentando acessar uma reunião online quando a política de acesso ao aplicativo não é configurada.

```json
{
    "error": {
        "code": "Unauthorized",
        "message": "App <app_ID_redacted> is not authorized to Create meeting on behalf of user <user_ID_redacted>",
        "innerError": {
            "date": "<date_redacted>",
            "request-id": "599d9cb0-56ac-4dc5-b6f8-1456a1414609"
        }
    }
}
```

Siga as etapas neste artigo para criar e/ou conceder uma política de acesso de aplicativo que contenha a ID de aplicativo para a ID de usuário.

## <a name="see-also"></a>Confira também

- [Referência de permissões](permissions-reference.md)
- [New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy)
- [Grant-ApplicationAccessPolicy](/powershell/module/skype/grant-csapplicationaccesspolicy)
- [Get-ApplicationAccessPolicy](/powershell/module/skype/get-csapplicationaccesspolicy)
- [Set-ApplicationAccessPolicy](/powershell/module/skype/set-csapplicationaccesspolicy)
- [Remove-ApplicationAccessPolicy](/powershell/module/skype/remove-csapplicationaccesspolicy)