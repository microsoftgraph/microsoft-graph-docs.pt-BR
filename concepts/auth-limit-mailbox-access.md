---
title: Limitando permissões de escopo de aplicativo para caixas de correio específicas do Exchange Online
description: Para definir o escopo das permissões de aplicativo de um aplicativo para caixas de correio específicas do Exchange Online, você precisará criar políticas de acesso a aplicativos.
author: abheek-das
localization_priority: Priority
ms.prod: applications
ms.openlocfilehash: e9f6b63f64981a49c655208c45ef9754324d5ae4
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456426"
---
# <a name="limiting-application-permissions-to-specific-exchange-online-mailboxes"></a><span data-ttu-id="76b5d-103">Limitando permissões de escopo de aplicativo para caixas de correio específicas do Exchange Online</span><span class="sxs-lookup"><span data-stu-id="76b5d-103">Limiting application permissions to specific Exchange Online mailboxes</span></span> 

<span data-ttu-id="76b5d-104">Os administradores que desejam limitar o acesso do aplicativo a caixas de correio específicas podem criar uma política de acesso de aplicativo usando o cmdlet **New-ApplicationAccessPolicy** do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="76b5d-104">Administrators who want to limit app access to specific mailboxes can create an application access policy by using the **New-ApplicationAccessPolicy** PowerShell cmdlet.</span></span> <span data-ttu-id="76b5d-105">Este artigo aborda as etapas básicas para configurar o controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="76b5d-105">This article covers the basic steps to configure access control.</span></span> <span data-ttu-id="76b5d-106">Estas etapas são específicas aos recursos do Exchange Online e não se aplicam a outras cargas de trabalho do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="76b5d-106">These steps are specific to Exchange Online resources and do not apply to other Microsoft Graph workloads.</span></span> 

## <a name="background"></a><span data-ttu-id="76b5d-107">Histórico</span><span class="sxs-lookup"><span data-stu-id="76b5d-107">Background</span></span>
<span data-ttu-id="76b5d-108">Alguns aplicativos chamam o Microsoft Graph usando sua própria identidade e não em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="76b5d-108">Some apps call Microsoft Graph using their own identity and not on behalf of a user.</span></span> <span data-ttu-id="76b5d-109">Geralmente, são serviços de segundo plano ou aplicativos daemon executados em um servidor sem a presença de um usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="76b5d-109">These are usually background services or daemon apps that run on a server without the presence of a signed-in user.</span></span> <span data-ttu-id="76b5d-110">Esses aplicativos usam o [fluxo de concessão de credenciais do cliente OAuth 2.0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) para autenticar e são configurados com permissões de aplicativo, que por padrão permitem que esses aplicativos acessem _todas_ as caixas de correio de uma organização no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="76b5d-110">These apps make use of [OAuth 2.0 client credentials grant flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) to authenticate and are configured with application permissions, which by default enable such apps to access _all_ mailboxes in a organization on Exchange Online.</span></span> <span data-ttu-id="76b5d-111">Por exemplo, a permissão de aplicativo `Mail.Read` permite que os aplicativos leiam emails em todas as caixas de correio sem um usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="76b5d-111">For example, the `Mail.Read` application permission allows apps to read mail in all mailboxes without a signed-in user.</span></span> 

<span data-ttu-id="76b5d-112">Há cenários em que os administradores podem querer limitar um aplicativo apenas a caixas de correio específicas e _não a todas_ as caixas de correio do Exchange Online na organização.</span><span class="sxs-lookup"><span data-stu-id="76b5d-112">There are scenarios where administrators may want to limit an app to only specific mailboxes and _not all_ Exchange Online mailboxes in the organization.</span></span> <span data-ttu-id="76b5d-113">Os administradores podem identificar o conjunto de caixas de correio para permitir o acesso colocando-as em um grupo de segurança habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="76b5d-113">Administrators can identify the set of mailboxes to permit access by putting them in a mail-enabled security group.</span></span> <span data-ttu-id="76b5d-114">Os administradores podem limitar o acesso de aplicativos de terceiros somente a esse conjunto de caixas de correio criando uma política de acesso de aplicativo para acesso a esse grupo.</span><span class="sxs-lookup"><span data-stu-id="76b5d-114">Administrators can then limit third-party app access to only that set of  mailboxes by creating an application access policy for access to that group.</span></span>

> [!NOTE]
> <span data-ttu-id="76b5d-115">Depois que uma política de acesso a aplicativos é configurada para uma organização, a política se aplica a qualquer aplicativo que usa a API do Microsoft Graph ou os Serviços Web do Exchange para acessar caixas de correio do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="76b5d-115">Once an application access policy is configured for an organization, the policy applies to any app that uses the Microsoft Graph API or Exchange Web Services to access Exchange Online mailboxes.</span></span>

<span data-ttu-id="76b5d-116">Conforme descrito na seção [permissões com suporte e recursos adicionais](#supported-permissions-and-additional-resources) abaixo, a política de acesso ao aplicativo restringe o acesso à caixa de correio para aplicativos que foram concedidos a qualquer um dos escopos de permissão do Microsoft Graph ou dos Serviços Web do Exchange aos quais a política dá suporte.</span><span class="sxs-lookup"><span data-stu-id="76b5d-116">As further described in the [Supported permissions and additional resources](#supported-permissions-and-additional-resources) section below, application access policy restricts mailbox access for apps that have been granted any of the Microsoft Graph or Exchange Web Services permission scopes that the policy supports.</span></span>

## <a name="configure-applicationaccesspolicy"></a><span data-ttu-id="76b5d-117">Configurar ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="76b5d-117">Configure ApplicationAccessPolicy</span></span>

<span data-ttu-id="76b5d-118">Para configurar uma política de acesso a aplicativos e limitar o escopo das permissões de aplicativos:</span><span class="sxs-lookup"><span data-stu-id="76b5d-118">To configure an application access policy and limit the scope of application permissions:</span></span>
1.  <span data-ttu-id="76b5d-119">Conecte-se ao PowerShell do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="76b5d-119">Connect to Exchange Online PowerShell.</span></span> <span data-ttu-id="76b5d-120">Para detalhes, consulte [Conectar-se ao PowerShell do Exchange Online](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="76b5d-120">For details, see [Connect to Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>

2.  <span data-ttu-id="76b5d-121">Identifique o ID do cliente do aplicativo e um grupo de segurança habilitado para email para restringir o acesso do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="76b5d-121">Identify the app’s client ID and a mail-enabled security group to restrict the app’s access to.</span></span>

    - <span data-ttu-id="76b5d-122">Identifique o ID do aplicativo (cliente) do aplicativo no [portal de registro de aplicativos do Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span><span class="sxs-lookup"><span data-stu-id="76b5d-122">Identify the app’s application (client) ID in the [Azure app registration portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
    - <span data-ttu-id="76b5d-123">Crie um novo grupo de segurança habilitado para email ou use um existente e identifique o endereço de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="76b5d-123">Create a new mail-enabled security group or use an existing one and identify the email address for the group.</span></span> 

3.  <span data-ttu-id="76b5d-124">Crie uma política de acesso a aplicativos.</span><span class="sxs-lookup"><span data-stu-id="76b5d-124">Create an application access policy.</span></span> 

    <span data-ttu-id="76b5d-125">Execute o seguinte comando, substituindo os argumentos **AppId**, **PolicyScopeGroupId** e **Description**.</span><span class="sxs-lookup"><span data-stu-id="76b5d-125">Run the following command, replacing the arguments for **AppId**, **PolicyScopeGroupId**, and **Description**.</span></span>
    ```sh 
    New-ApplicationAccessPolicy -AppId e7e4dbfc-046f-4074-9b3b-2ae8f144f59b -PolicyScopeGroupId EvenUsers@contoso.com -AccessRight RestrictAccess -Description "Restrict this app to members of distribution group EvenUsers."
    ```
4.  <span data-ttu-id="76b5d-126">Teste a política de acesso a aplicativos recém-criada.</span><span class="sxs-lookup"><span data-stu-id="76b5d-126">Test the newly created application access policy.</span></span>

    <span data-ttu-id="76b5d-127">Execute o comando a seguir, substituindo os argumentos para **Identity** e **AppId**.</span><span class="sxs-lookup"><span data-stu-id="76b5d-127">Run the following command, replacing the arguments for **Identity** and **AppId**.</span></span>
    ```sh
    Test-ApplicationAccessPolicy -Identity user1@contoso.com -AppId e7e4dbfc-046-4074-9b3b-2ae8f144f59b 
    ```
    <span data-ttu-id="76b5d-128">A saída desse comando indicará se o aplicativo tem acesso à caixa de correio do Usuário 1.</span><span class="sxs-lookup"><span data-stu-id="76b5d-128">The output of this command will indicate whether the app has access to User1’s mailbox.</span></span>

><span data-ttu-id="76b5d-129">**Observação: as alterações nas políticas de acesso ao aplicativo podem levar até 30 minutos para entrar em vigor nas chamadas da API REST do Microsoft Graph.**</span><span class="sxs-lookup"><span data-stu-id="76b5d-129">**Note: Changes to application access policies can take up to 30 minutes to take effect in Microsoft Graph REST API calls.**</span></span>

## <a name="supported-permissions-and-additional-resources"></a><span data-ttu-id="76b5d-130">Permissões compatíveis e recursos adicionais</span><span class="sxs-lookup"><span data-stu-id="76b5d-130">Supported permissions and additional resources</span></span>

<span data-ttu-id="76b5d-131">Os administradores podem usar os cmdlets ApplicationAccessPolicy para controlar o acesso à caixa de correio de um aplicativo que recebeu qualquer uma das seguintes permissões de aplicativo do Microsoft Graph ou permissões de Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="76b5d-131">Administrators can use ApplicationAccessPolicy cmdlets to control mailbox access of an app that has been granted any of the following Microsoft Graph application permissions or Exchange Web Services permissions.</span></span> 

<span data-ttu-id="76b5d-132">Permissões de aplicativos do Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="76b5d-132">Microsoft Graph application permissions:</span></span> 
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

<span data-ttu-id="76b5d-133">Escopo de permissão dos Serviços Web do Exchange: `full_access_as_app`.</span><span class="sxs-lookup"><span data-stu-id="76b5d-133">Exchange Web Services permission scope: `full_access_as_app`.</span></span>

<span data-ttu-id="76b5d-134">Para obter mais informações sobre como configurar a política de acesso a aplicativos, consulte a [referência de cmdlet do PowerShell para New-ApplicationAccessPolicy](/powershell/module/exchange/new-applicationaccesspolicy?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="76b5d-134">For more information about configuring application access policy, see the [PowerShell cmdlet reference for New-ApplicationAccessPolicy](/powershell/module/exchange/new-applicationaccesspolicy?view=exchange-ps&preserve-view=true).</span></span> 


## <a name="handling-api-errors"></a><span data-ttu-id="76b5d-135">Como lidar com erros da API</span><span class="sxs-lookup"><span data-stu-id="76b5d-135">Handling API errors</span></span>
<span data-ttu-id="76b5d-136">Você poderá encontrar o seguinte erro quando uma chamada de API for negada devido a uma política de acesso de aplicativo configurada.</span><span class="sxs-lookup"><span data-stu-id="76b5d-136">You might encounter the following error when an API call is denied access due to a configured application access policy.</span></span> 
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
<span data-ttu-id="76b5d-137">Se as chamadas da API do Microsoft Graph de seu aplicativo retornarem esse erro, trabalhe com o administrador do Exchange Online da organização para garantir que seu aplicativo tenha permissão para acessar o recurso de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="76b5d-137">If the Microsoft Graph API calls from your app return this error, work with the Exchange Online administrator for the organization to ensure that your app has permission to access the mailbox resource.</span></span>



## <a name="see-also"></a><span data-ttu-id="76b5d-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="76b5d-138">See also</span></span>

- [<span data-ttu-id="76b5d-139">Referência de permissões</span><span class="sxs-lookup"><span data-stu-id="76b5d-139">Permissions reference</span></span>](permissions-reference.md)
- [<span data-ttu-id="76b5d-140">New-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="76b5d-140">New-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/new-applicationaccesspolicy)
- [<span data-ttu-id="76b5d-141">Get-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="76b5d-141">Get-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/get-applicationaccesspolicy)
- [<span data-ttu-id="76b5d-142">Remove-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="76b5d-142">Remove-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/remove-applicationaccesspolicy)
- [<span data-ttu-id="76b5d-143">Set-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="76b5d-143">Set-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/set-applicationaccesspolicy)
- [<span data-ttu-id="76b5d-144">Test-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="76b5d-144">Test-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/test-applicationaccesspolicy)
- [<span data-ttu-id="76b5d-145">Suporte à política de acesso a aplicativos no EWS</span><span class="sxs-lookup"><span data-stu-id="76b5d-145">Application Access Policy Support in EWS</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/application-access-policy-support-in-ews/ba-p/2110361)
