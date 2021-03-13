---
title: Permissões de escopo de aplicativo para caixas de correio específicas do Exchange Online
description: Para definir o escopo das permissões de aplicativo de um aplicativo para caixas de correio específicas do Exchange Online, você precisará criar políticas de acesso a aplicativos.
author: abheek-das
localization_priority: Priority
ms.prod: applications
ms.openlocfilehash: 56b05834f85c0b4a3f4480855cd0bffc8415b628
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760739"
---
# <a name="scoping-application-permissions-to-specific-exchange-online-mailboxes"></a>Permissões de escopo de aplicativo para caixas de correio específicas do Exchange Online 

Alguns aplicativos chamam o Microsoft Graph usando sua própria identidade e não em nome de um usuário. Geralmente, são serviços de segundo plano ou aplicativos daemon executados em um servidor sem a presença de um usuário conectado. Esses aplicativos usam o [fluxo de concessão de credenciais do cliente OAuth 2.0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) para autenticar e são configurados com permissões de aplicativo, que permitem que esses aplicativos acessem todas as caixas de correio de uma organização no Exchange Online. Por exemplo, a permissão de aplicativo Mail.Read permite que os aplicativos leiam emails em todas as caixas de correio sem um usuário conectado. 

Os administradores que desejem limitar o acesso ao aplicativo a um conjunto específico de caixas de correio podem usar o cmdlet **New-ApplicationAccessPolicy** do PowerShell para configurar o controle de acesso. Este artigo aborda as etapas básicas para configurar uma política de acesso a aplicativos.

Estas etapas são específicas aos recursos do Exchange Online e não se aplicam a outras cargas de trabalho do Microsoft Graph. 

## <a name="configure-applicationaccesspolicy"></a>Configurar ApplicationAccessPolicy

Para configurar uma política de acesso a aplicativos e limitar o escopo das permissões de aplicativos:
1.  Conecte-se ao PowerShell do Exchange Online. Para detalhes, consulte [Conectar-se ao PowerShell do Exchange Online](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps).

2.  Identifique o ID do cliente do aplicativo e um grupo de segurança habilitado para email para restringir o acesso do aplicativo.

    - Identifique o ID do aplicativo (cliente) do aplicativo no [portal de registro de aplicativos do Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).
    - Crie um novo grupo de segurança habilitado para email ou use um existente e identifique o endereço de email do grupo. 

3.  Crie uma política de acesso a aplicativos. 

    Execute o seguinte comando, substituindo os argumentos **AppId**, **PolicyScopeGroupId** e **Description**.
    ```sh 
    New-ApplicationAccessPolicy -AppId e7e4dbfc-046f-4074-9b3b-2ae8f144f59b -PolicyScopeGroupId EvenUsers@contoso.com -AccessRight RestrictAccess -Description "Restrict this app to members of distribution group EvenUsers."
    ```
4.  Teste a política de acesso a aplicativos recém-criada.

    Execute o seguinte comando, substituindo os argumentos **AppId** e **Identity**.
    ```sh
    Test-ApplicationAccessPolicy -Identity user1@contoso.com -AppId e7e4dbfc-046-4074-9b3b-2ae8f144f59b 
    ```
    A saída desse comando indicará se o aplicativo tem acesso à caixa de correio do Usuário 1.

Observação: as alterações nas políticas de acesso a aplicativos podem levar até 30 minutos para entrar em vigor nas chamadas da API REST do Microsoft Graph.

## <a name="supported-permissions-and-additional-resources"></a>Permissões compatíveis e recursos adicionais
Os administradores podem usar os cmdlets ApplicationAccessPolicy para controlar o acesso à caixa de correio de um aplicativo que tenha recebido as seguintes permissões de aplicativo: 
- Mail.Read
- Mail.ReadBasic
- Mail.ReadBasic.All
- Mail.ReadWrite
- Mail.Send
- MailboxSettings.Read  
- MailboxSettings.ReadWrite
- Calendars.Read
- Calendars.ReadWrite
- Contacts.Read
- Contacts.ReadWrite

Para obter mais informações sobre como configurar a política de acesso a aplicativos, consulte a [referência de cmdlet do PowerShell para New-ApplicationAccessPolicy](/powershell/module/exchange/organization/new-applicationaccesspolicy). 

## <a name="handling-api-errors"></a>Como lidar com erros da API
Você poderá encontrar o seguinte erro quando uma chamada de API for negada devido a uma política de acesso de aplicativo configurada. 
```json
{
    "error": {
        "code": "ErrorAccessDenied",
        "message": "Access to OData is disabled.",
        "innerError": {
            "request-id": "2f038156-cf40-403d-8e46-831fe42a8229",
            "date": "2019-05-24T10:16:21"
        }
    }
}
```
Se as chamadas da API do Microsoft Graph de seu aplicativo retornarem esse erro, trabalhe com o administrador do Exchange Online da organização para garantir que seu aplicativo tenha permissão para acessar o recurso de caixa de correio.



## <a name="see-also"></a>Confira também

- [Referência de permissões](permissions-reference.md)
- [New-ApplicationAccessPolicy](/powershell/module/exchange/organization/new-applicationaccesspolicy)
- [Get-ApplicationAccessPolicy](/powershell/module/exchange/organization/get-applicationaccesspolicy)
- [Remove-ApplicationAccessPolicy](/powershell/module/exchange/organization/remove-applicationaccesspolicy)
- [Set-ApplicationAccessPolicy](/powershell/module/exchange/organization/set-applicationaccesspolicy)
- [Test-ApplicationAccessPolicy](/powershell/module/exchange/organization/test-applicationaccesspolicy)