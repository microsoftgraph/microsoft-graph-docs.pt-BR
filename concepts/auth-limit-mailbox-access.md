---
title: Permissões de escopo de aplicativo para caixas de correio específicas do Exchange Online
description: Para definir o escopo das permissões de aplicativo de um aplicativo para caixas de correio específicas do Exchange Online, você precisará criar políticas de acesso a aplicativos.
author: abheek-das
localization_priority: Priority
ms.prod: applications
ms.openlocfilehash: f31f7bfc8ff72c8f3cb9e6f61185187f50bab7fc
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266833"
---
# <a name="scoping-application-permissions-to-specific-exchange-online-mailboxes"></a><span data-ttu-id="ba11d-103">Permissões de escopo de aplicativo para caixas de correio específicas do Exchange Online</span><span class="sxs-lookup"><span data-stu-id="ba11d-103">Scoping application permissions to specific Exchange Online mailboxes</span></span> 

<span data-ttu-id="ba11d-104">Alguns aplicativos chamam o Microsoft Graph usando sua própria identidade e não em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="ba11d-104">Some apps call Microsoft Graph using their own identity and not on behalf of a user.</span></span> <span data-ttu-id="ba11d-105">Geralmente, são serviços de segundo plano ou aplicativos daemon executados em um servidor sem a presença de um usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="ba11d-105">These are usually background services or daemon apps that run on a server without the presence of a signed-in user.</span></span> <span data-ttu-id="ba11d-106">Esses aplicativos usam o [fluxo de concessão de credenciais do cliente OAuth 2.0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) para autenticar e são configurados com permissões de aplicativo, que permitem que esses aplicativos acessem todas as caixas de correio de uma organização no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="ba11d-106">These apps make use of [OAuth 2.0 client credentials grant flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) to authenticate and are configured with application permissions, which enable such apps to access all mailboxes in a organization on Exchange Online.</span></span> <span data-ttu-id="ba11d-107">Por exemplo, a permissão de aplicativo Mail.Read permite que os aplicativos leiam emails em todas as caixas de correio sem um usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="ba11d-107">For example, the Mail.Read application permission allows apps to read mail in all mailboxes without a signed-in user.</span></span> 

<span data-ttu-id="ba11d-108">Os administradores que desejem limitar o acesso ao aplicativo a um conjunto específico de caixas de correio podem usar o cmdlet **New-ApplicationAccessPolicy** do PowerShell para configurar o controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="ba11d-108">Administrators who want to limit the app access to a specific set of mailboxes can use the **New-ApplicationAccessPolicy** PowerShell cmdlet to configure access control.</span></span> <span data-ttu-id="ba11d-109">Este artigo aborda as etapas básicas para configurar uma política de acesso a aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ba11d-109">This article covers the basic steps to configure an application access policy.</span></span>

<span data-ttu-id="ba11d-110">Estas etapas são específicas aos recursos do Exchange Online e não se aplicam a outras cargas de trabalho do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ba11d-110">These steps are specific to Exchange Online resources and do not apply to other Microsoft Graph workloads.</span></span> 

## <a name="configure-applicationaccesspolicy"></a><span data-ttu-id="ba11d-111">Configurar ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ba11d-111">Configure ApplicationAccessPolicy</span></span>

<span data-ttu-id="ba11d-112">Para configurar uma política de acesso a aplicativos e limitar o escopo das permissões de aplicativos:</span><span class="sxs-lookup"><span data-stu-id="ba11d-112">To configure an application access policy and limit the scope of application permissions:</span></span>
1.  <span data-ttu-id="ba11d-113">Conecte-se ao PowerShell do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="ba11d-113">Connect to Exchange Online PowerShell.</span></span> <span data-ttu-id="ba11d-114">Para detalhes, consulte [Conectar-se ao PowerShell do Exchange Online](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ba11d-114">For details, see [Connect to Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps).</span></span>

2.  <span data-ttu-id="ba11d-115">Identifique o ID do cliente do aplicativo e um grupo de segurança habilitado para email para restringir o acesso do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ba11d-115">Identify the app’s client ID and a mail-enabled security group to restrict the app’s access to.</span></span>

    - <span data-ttu-id="ba11d-116">Identifique o ID do aplicativo (cliente) do aplicativo no [portal de registro de aplicativos do Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span><span class="sxs-lookup"><span data-stu-id="ba11d-116">Identify the app’s application (client) ID in the [Azure app registration portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
    - <span data-ttu-id="ba11d-117">Crie um novo grupo de segurança habilitado para email ou use um existente e identifique o endereço de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="ba11d-117">Create a new mail-enabled security group or use an existing one and identify the email address for the group.</span></span> 

3.  <span data-ttu-id="ba11d-118">Crie uma política de acesso a aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ba11d-118">Create an application access policy.</span></span> 

    <span data-ttu-id="ba11d-119">Execute o seguinte comando, substituindo os argumentos **AppId**, **PolicyScopeGroupId** e **Description**.</span><span class="sxs-lookup"><span data-stu-id="ba11d-119">Run the following command, replacing the **AppId**, **PolicyScopeGroupId**, and **Description** arguments.</span></span>
    ```sh 
    New-ApplicationAccessPolicy -AppId e7e4dbfc-046f-4074-9b3b-2ae8f144f59b -PolicyScopeGroupId EvenUsers@contoso.com -AccessRight RestrictAccess -Description "Restrict this app to members of distribution group EvenUsers."
    ```
4.  <span data-ttu-id="ba11d-120">Teste a política de acesso a aplicativos recém-criada.</span><span class="sxs-lookup"><span data-stu-id="ba11d-120">Test the newly created application access policy.</span></span>

    <span data-ttu-id="ba11d-121">Execute o seguinte comando, substituindo os argumentos **AppId** e **Identity**.</span><span class="sxs-lookup"><span data-stu-id="ba11d-121">Run the following command, replacing the **AppId** and **Identity** arguments.</span></span>
    ```sh
    Test-ApplicationAccessPolicy -Identity user1@contoso.com -AppId e7e4dbfc-046-4074-9b3b-2ae8f144f59b 
    ```
    <span data-ttu-id="ba11d-122">A saída desse comando indicará se o aplicativo tem acesso à caixa de correio do Usuário 1.</span><span class="sxs-lookup"><span data-stu-id="ba11d-122">The output of this command will indicate whether the app has access to User1’s mailbox.</span></span>

><span data-ttu-id="ba11d-123">**Observação: as alterações nas políticas de acesso ao aplicativo podem levar até 30 minutos para entrar em vigor nas chamadas da API REST do Microsoft Graph.**</span><span class="sxs-lookup"><span data-stu-id="ba11d-123">**Note: Changes to application access policies can take up to 30 minutes to take effect in Microsoft Graph REST API calls.**</span></span>

## <a name="supported-permissions-and-additional-resources"></a><span data-ttu-id="ba11d-124">Permissões compatíveis e recursos adicionais</span><span class="sxs-lookup"><span data-stu-id="ba11d-124">Supported permissions and additional resources</span></span>
<span data-ttu-id="ba11d-125">Os administradores podem usar os cmdlets ApplicationAccessPolicy para controlar o acesso à caixa de correio de um aplicativo que tenha recebido as seguintes permissões de aplicativo:</span><span class="sxs-lookup"><span data-stu-id="ba11d-125">Administrators can use ApplicationAccessPolicy cmdlets to control mailbox access of an app that has been granted any of the following application permissions:</span></span> 
- <span data-ttu-id="ba11d-126">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="ba11d-126">Mail.Read</span></span>
- <span data-ttu-id="ba11d-127">Mail.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="ba11d-127">Mail.ReadBasic</span></span>
- <span data-ttu-id="ba11d-128">Mail.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="ba11d-128">Mail.ReadBasic.All</span></span>
- <span data-ttu-id="ba11d-129">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba11d-129">Mail.ReadWrite</span></span>
- <span data-ttu-id="ba11d-130">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="ba11d-130">Mail.Send</span></span>
- <span data-ttu-id="ba11d-131">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ba11d-131">MailboxSettings.Read</span></span>  
- <span data-ttu-id="ba11d-132">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba11d-132">MailboxSettings.ReadWrite</span></span>
- <span data-ttu-id="ba11d-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="ba11d-133">Calendars.Read</span></span>
- <span data-ttu-id="ba11d-134">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba11d-134">Calendars.ReadWrite</span></span>
- <span data-ttu-id="ba11d-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ba11d-135">Contacts.Read</span></span>
- <span data-ttu-id="ba11d-136">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba11d-136">Contacts.ReadWrite</span></span>

<span data-ttu-id="ba11d-137">Para obter mais informações sobre como configurar a política de acesso a aplicativos, consulte a [referência de cmdlet do PowerShell para New-ApplicationAccessPolicy](/powershell/module/exchange/organization/new-applicationaccesspolicy).</span><span class="sxs-lookup"><span data-stu-id="ba11d-137">For more information about configuring application access policy, see the [PowerShell cmdlet reference for New-ApplicationAccessPolicy](/powershell/module/exchange/organization/new-applicationaccesspolicy).</span></span> 

## <a name="handling-api-errors"></a><span data-ttu-id="ba11d-138">Como lidar com erros da API</span><span class="sxs-lookup"><span data-stu-id="ba11d-138">Handling API errors</span></span>
<span data-ttu-id="ba11d-139">Você poderá encontrar o seguinte erro quando uma chamada de API for negada devido a uma política de acesso de aplicativo configurada.</span><span class="sxs-lookup"><span data-stu-id="ba11d-139">You might encounter the following error when an API call is denied access due to a configured application access policy.</span></span> 
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
<span data-ttu-id="ba11d-140">Se as chamadas da API do Microsoft Graph de seu aplicativo retornarem esse erro, trabalhe com o administrador do Exchange Online da organização para garantir que seu aplicativo tenha permissão para acessar o recurso de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ba11d-140">If Microsoft Graph API calls from your app return this error, work with the Exchange Online administrator for the organization to ensure that your app has permission to access the mailbox resource.</span></span>



## <a name="see-also"></a><span data-ttu-id="ba11d-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="ba11d-141">See also</span></span>

- [<span data-ttu-id="ba11d-142">Referência de permissões</span><span class="sxs-lookup"><span data-stu-id="ba11d-142">Permissions reference</span></span>](permissions-reference.md)
- [<span data-ttu-id="ba11d-143">New-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ba11d-143">New-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/new-applicationaccesspolicy)
- [<span data-ttu-id="ba11d-144">Get-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ba11d-144">Get-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/get-applicationaccesspolicy)
- [<span data-ttu-id="ba11d-145">Remove-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ba11d-145">Remove-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/remove-applicationaccesspolicy)
- [<span data-ttu-id="ba11d-146">Set-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ba11d-146">Set-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/set-applicationaccesspolicy)
- [<span data-ttu-id="ba11d-147">Test-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="ba11d-147">Test-ApplicationAccessPolicy</span></span>](/powershell/module/exchange/organization/test-applicationaccesspolicy)
