---
title: Limitando permissões de escopo de aplicativo para caixas de correio específicas do Exchange Online
description: Para definir o escopo das permissões de aplicativo de um aplicativo para caixas de correio específicas do Exchange Online, você precisará criar políticas de acesso a aplicativos.
author: abheek-das
ms.localizationpriority: high
ms.prod: applications
ms.openlocfilehash: 03a0edde1a3e21455200049bf51bf1867e1a0657
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335889"
---
# <a name="limiting-application-permissions-to-specific-exchange-online-mailboxes"></a>Limitando permissões de escopo de aplicativo para caixas de correio específicas do Exchange Online 

Os administradores que desejam limitar o acesso do aplicativo a caixas de correio específicas podem criar uma política de acesso de aplicativo usando o cmdlet **New-ApplicationAccessPolicy** do PowerShell. Este artigo aborda as etapas básicas para configurar o controle de acesso. Estas etapas são específicas aos recursos do Exchange Online e não se aplicam a outras cargas de trabalho do Microsoft Graph. 

## <a name="background"></a>Histórico
Alguns aplicativos chamam o Microsoft Graph usando sua própria identidade e não em nome de um usuário. Geralmente, são serviços de segundo plano ou aplicativos daemon executados em um servidor sem a presença de um usuário conectado. Esses aplicativos usam o [fluxo de concessão de credenciais do cliente OAuth 2.0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) para autenticar e são configurados com permissões de aplicativo, que por padrão permitem que esses aplicativos acessem _todas_ as caixas de correio de uma organização no Exchange Online. Por exemplo, a permissão de aplicativo `Mail.Read` permite que os aplicativos leiam emails em todas as caixas de correio sem um usuário conectado.

> [!IMPORTANT]
> 
> Por padrão, os aplicativos que receberam permissões de aplicativo para os seguintes conjuntos de dados podem acessar todas as caixas de correio na organização:
> 
> - [Calendários](permissions-reference.md#calendars-permissions)
> - [Contatos](permissions-reference.md#contacts-permissions)
> - [Email](permissions-reference.md#mail-permissions)
> - [Configurações da Caixa de Correio](permissions-reference.md#mail-permissions)
> 
>Os administradores podem configurar a [política de acesso a aplicativos](#configure-applicationaccesspolicy) para limitar o acesso do aplicativo a caixas de correio _específicas_.

Há cenários em que os administradores podem querer limitar um aplicativo apenas a caixas de correio específicas e _não a todas_ as caixas de correio do Exchange Online na organização. Os administradores podem identificar o conjunto de caixas de correio para permitir o acesso colocando-as em um grupo de segurança habilitado para email. Os administradores podem limitar o acesso de aplicativos de terceiros somente a esse conjunto de caixas de correio criando uma política de acesso de aplicativo para acesso a esse grupo.

Conforme descrito na seção [permissões com suporte e recursos adicionais](#supported-permissions-and-additional-resources) abaixo, a política de acesso ao aplicativo restringe o acesso à caixa de correio para aplicativos que foram concedidos a qualquer um dos escopos de permissão do Microsoft Graph ou dos Serviços Web do Exchange aos quais a política dá suporte.

## <a name="configure-applicationaccesspolicy"></a>Configurar ApplicationAccessPolicy

Para configurar uma política de acesso a aplicativos e limitar o escopo das permissões de aplicativos:
1.  Conecte-se ao PowerShell do Exchange Online. Para obter detalhes, consulte [Conectar-se ao PowerShell do Exchange Online](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).

2.  Identifique o ID do cliente do aplicativo e um grupo de segurança habilitado para email para restringir o acesso do aplicativo.

    - Identifique o ID do aplicativo (cliente) do aplicativo no [portal de registro de aplicativos do Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).
    - Crie um novo grupo de segurança habilitado para email ou use um existente e identifique o endereço de email do grupo. 

3.  Crie uma política de acesso a aplicativos. 

    Execute o seguinte comando, substituindo os argumentos **AppId**, **PolicyScopeGroupId** e **Description**.
    ```sh 
    New-ApplicationAccessPolicy -AppId e7e4dbfc-046f-4074-9b3b-2ae8f144f59b -PolicyScopeGroupId EvenUsers@contoso.com -AccessRight RestrictAccess -Description "Restrict this app to members of distribution group EvenUsers."
    ```
4.  Teste a política de acesso a aplicativos recém-criada.

    Execute o comando a seguir, substituindo os argumentos para **Identity** e **AppId**.
    ```sh
    Test-ApplicationAccessPolicy -Identity user1@contoso.com -AppId e7e4dbfc-046-4074-9b3b-2ae8f144f59b 
    ```
    A saída desse comando indicará se o aplicativo tem acesso à caixa de correio do Usuário 1.

>**Observação:** alterações nas políticas de acesso do aplicativo podem levar mais de uma hora para entrar em vigor em chamadas à API REST do Microsoft Graph, mesmo quando `Test-ApplicationAccessPolicy` mostra resultados positivos.

## <a name="supported-permissions-and-additional-resources"></a>Permissões compatíveis e recursos adicionais

Os administradores podem usar os cmdlets ApplicationAccessPolicy para controlar o acesso à caixa de correio de um aplicativo que recebeu qualquer uma das seguintes permissões de aplicativo do Microsoft Graph ou permissões de Serviços Web do Exchange. 

Permissões de aplicativos do Microsoft Graph: 
- `Mail.Read`
- `Mail.ReadBasic`
- `Mail.ReadBasic.All`
- `Mail.ReadWrite`
- `Mail.Send`
- `MailboxSettings.Read`
- `MailboxSettings.ReadWrite`
- `Calendars.Read`
- `Calendars.ReadWrite`
- `Contacts.Read`
- `Contacts.ReadWrite`

Escopo de permissão dos Serviços Web do Exchange: `full_access_as_app`.

Para obter mais informações sobre como configurar a política de acesso a aplicativos, consulte a [referência de cmdlet do PowerShell para New-ApplicationAccessPolicy](/powershell/module/exchange/new-applicationaccesspolicy?view=exchange-ps&preserve-view=true). 


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
- [Suporte à política de acesso a aplicativos no EWS](https://techcommunity.microsoft.com/t5/exchange-team-blog/application-access-policy-support-in-ews/ba-p/2110361)
