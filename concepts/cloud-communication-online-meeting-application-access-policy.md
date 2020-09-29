---
title: Permitir que os aplicativos acessem reuniões online em nome de um usuário
description: Descubra como configurar aplicativos para acessar reuniões online em nome de um usuário.
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: a0a0d264e8898d8524f104d3fe5dafeb1b151f5f
ms.sourcegitcommit: 6eadb95e21b2e7eb5d6b081b91999cb91070f397
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2020
ms.locfileid: "48299267"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a><span data-ttu-id="30cb0-103">Permitir que os aplicativos acessem reuniões online em nome de um usuário</span><span class="sxs-lookup"><span data-stu-id="30cb0-103">Allow applications to access online meetings on behalf of a user</span></span>

<span data-ttu-id="30cb0-104">Em alguns casos, como nos serviços em segundo plano ou em aplicativos de daemon executados em um servidor sem a presença de um usuário conectado, é apropriado para um aplicativo chamar o Microsoft Graph para executar ações em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="30cb0-104">In some cases, such as for background services or daemon apps that run on a server without the presence of a signed-in user, it is appropriate for an app to call Microsoft Graph to take actions on behalf of a user.</span></span> <span data-ttu-id="30cb0-105">Por exemplo, um aplicativo pode precisar chamar o Microsoft Graph para agendar várias reuniões com base em agendas publicadas (como cursos) ou em ferramentas de agendamento externas.</span><span class="sxs-lookup"><span data-stu-id="30cb0-105">For example, an app might need to call Microsoft Graph to schedule multiple meetings based on published schedules (such as courses) or external scheduling tools.</span></span> <span data-ttu-id="30cb0-106">Nesses casos, o usuário que o aplicativo atua em nome do é identificado como organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="30cb0-106">In these cases, the user that the application acts on behalf of is identified as the meeting organizer.</span></span>

<span data-ttu-id="30cb0-107">Os administradores que desejam permitir que um aplicativo acesse recursos de reunião online em nome de um usuário podem usar os cmdlets **New-CsApplicationAccessPolicy** e **Grant-CsApplicationAccessPolicy** do PowerShell para configurar o controle de acesso.</span><span class="sxs-lookup"><span data-stu-id="30cb0-107">Administrators who want to allow an application to access online meeting resources on behalf of a user can use **New-CsApplicationAccessPolicy** and **Grant-CsApplicationAccessPolicy** PowerShell cmdlets to configure access control.</span></span> <span data-ttu-id="30cb0-108">Este artigo aborda as etapas básicas para configurar uma política de acesso a aplicativos.</span><span class="sxs-lookup"><span data-stu-id="30cb0-108">This article covers the basic steps to configure an application access policy.</span></span>

<span data-ttu-id="30cb0-109">Estas etapas são específicas para reuniões online e não se aplicam a outros recursos do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="30cb0-109">These steps are specific to online meetings and do not apply to other Microsoft Graph resources.</span></span>

## <a name="configure-application-access-policy"></a><span data-ttu-id="30cb0-110">Configurar a política de acesso do aplicativo</span><span class="sxs-lookup"><span data-stu-id="30cb0-110">Configure application access policy</span></span>

<span data-ttu-id="30cb0-111">Para configurar uma política de acesso de aplicativo e permitir que os aplicativos acessem reuniões online com permissões de aplicativo:</span><span class="sxs-lookup"><span data-stu-id="30cb0-111">To configure an application access policy and allow applications to access online meetings with application permissions:</span></span>

1. <span data-ttu-id="30cb0-112">Identifique a ID do applcation (cliente) do aplicativo e as IDs de usuário dos usuários em nome do qual o aplicativo será autorizado a acessar reuniões online.</span><span class="sxs-lookup"><span data-stu-id="30cb0-112">Identify the app’s applcation (client) ID and the user IDs of the users on behalf of which the app will be authorized to access online meetings.</span></span>

    - <span data-ttu-id="30cb0-113">Identifique o ID do aplicativo (cliente) do aplicativo no [portal de registro de aplicativos do Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span><span class="sxs-lookup"><span data-stu-id="30cb0-113">Identify the app’s application (client) ID in the [Azure app registration portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
    - <span data-ttu-id="30cb0-114">Identificar a ID de usuário (objeto) do usuário no [portal de gerenciamento de usuários do Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="30cb0-114">Identify the user's user (object) ID in the [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span></span>

2. <span data-ttu-id="30cb0-115">Conecte-se ao Skype for Business PowerShell com a conta Adminitrator.</span><span class="sxs-lookup"><span data-stu-id="30cb0-115">Connect to Skype for Business PowerShell with adminitrator account.</span></span> <span data-ttu-id="30cb0-116">Para obter detalhes, consulte [gerenciar o Skype for Business online com o PowerShell](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="30cb0-116">For details, see [Manage Skype for Business Online with PowerShell](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell).</span></span>

3. <span data-ttu-id="30cb0-117">Crie uma política de acesso de aplicativo contendo uma lista de IDs de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="30cb0-117">Create an application access policy containing a list of app IDs.</span></span>

    <span data-ttu-id="30cb0-118">Execute o cmdlet a seguir, substituindo os argumentos **identidade**, **APPIDs**e **Description** (opcional).</span><span class="sxs-lookup"><span data-stu-id="30cb0-118">Run the following cmdlet, replacing the **Identity**, **AppIds**, and **Description** (optional) arguments.</span></span>

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. <span data-ttu-id="30cb0-119">Conceda a política ao usuário para permitir que as IDs de aplicativo contidas na política acessem reuniões online em nome do usuário concedido.</span><span class="sxs-lookup"><span data-stu-id="30cb0-119">Grant the policy to the user to allow the app IDs contained in the policy to access online meetings on behalf of the granted user.</span></span> 

   <span data-ttu-id="30cb0-120">Execute o cmdlet a seguir, substituindo os argumentos **PolicyName** e **Identity** .</span><span class="sxs-lookup"><span data-stu-id="30cb0-120">Run the following cmdlet, replacing the **PolicyName** and **Identity** arguments.</span></span>

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "ddb80e06-92f3-4978-bc22-a0eee85e6a9e"
   ```

> <span data-ttu-id="30cb0-121">**Observação**</span><span class="sxs-lookup"><span data-stu-id="30cb0-121">**Note**</span></span> 
> 
> - <span data-ttu-id="30cb0-122">_Identity_ se refere ao nome da política ao criar a política, mas a ID de usuário ao conceder a política.</span><span class="sxs-lookup"><span data-stu-id="30cb0-122">_Identity_ refers to the policy name when creating the policy, but the user ID when granting the policy.</span></span>
> - <span data-ttu-id="30cb0-123">As alterações nas políticas de acesso de aplicativos podem levar até 30 minutos para entrar em vigor nas chamadas da API REST do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="30cb0-123">Changes to application access policies can take up to 30 minutes to take effect in Microsoft Graph REST API calls.</span></span>

## <a name="supported-permissions-and-additional-resources"></a><span data-ttu-id="30cb0-124">Permissões compatíveis e recursos adicionais</span><span class="sxs-lookup"><span data-stu-id="30cb0-124">Supported permissions and additional resources</span></span>

<span data-ttu-id="30cb0-125">Os administradores podem usar cmdlets do ApplicationAccessPolicy para controlar o acesso de caixa de correio de um aplicativo que recebeu qualquer uma das seguintes permissões de aplicativo:</span><span class="sxs-lookup"><span data-stu-id="30cb0-125">Administrators can use ApplicationAccessPolicy cmdlets to control mailbox access for an app that has been granted any of the following application permissions:</span></span>

- <span data-ttu-id="30cb0-126">OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="30cb0-126">OnlineMeetings.Read.All</span></span>
- <span data-ttu-id="30cb0-127">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30cb0-127">OnlineMeetings.ReadWrite.All</span></span>

<span data-ttu-id="30cb0-128">Para obter mais informações sobre como configurar a política de acesso a aplicativos, consulte a [referência de cmdlet do PowerShell para New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).</span><span class="sxs-lookup"><span data-stu-id="30cb0-128">For more information about configuring application access policy, see the [PowerShell cmdlet reference for New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).</span></span>

## <a name="errors"></a><span data-ttu-id="30cb0-129">Erros</span><span class="sxs-lookup"><span data-stu-id="30cb0-129">Errors</span></span>

<span data-ttu-id="30cb0-130">Você pode encontrar o seguinte erro quando uma chamada à API tem acesso negado devido a um aplicativo tentando acessar uma reunião online quando a política de acesso ao aplicativo não é configurada.</span><span class="sxs-lookup"><span data-stu-id="30cb0-130">You might encounter the following error when an API call is denied access due to an app trying to access an online meeting when application access policy is not configured.</span></span>

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

<span data-ttu-id="30cb0-131">Siga as etapas neste artigo para criar e/ou conceder uma política de acesso de aplicativo que contenha a ID de aplicativo para a ID de usuário.</span><span class="sxs-lookup"><span data-stu-id="30cb0-131">Follow the steps in this article to create and/or grant an application access policy that contains the app ID to the user ID.</span></span>

## <a name="see-also"></a><span data-ttu-id="30cb0-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="30cb0-132">See also</span></span>

- [<span data-ttu-id="30cb0-133">Referência de permissões</span><span class="sxs-lookup"><span data-stu-id="30cb0-133">Permissions reference</span></span>](permissions-reference.md)
- [<span data-ttu-id="30cb0-134">New-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="30cb0-134">New-ApplicationAccessPolicy</span></span>](/powershell/module/skype/new-csapplicationaccesspolicy)
- [<span data-ttu-id="30cb0-135">Grant-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="30cb0-135">Grant-ApplicationAccessPolicy</span></span>](/powershell/module/skype/grant-csapplicationaccesspolicy)
- [<span data-ttu-id="30cb0-136">Get-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="30cb0-136">Get-ApplicationAccessPolicy</span></span>](/powershell/module/skype/get-csapplicationaccesspolicy)
- [<span data-ttu-id="30cb0-137">Set-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="30cb0-137">Set-ApplicationAccessPolicy</span></span>](/powershell/module/skype/set-csapplicationaccesspolicy)
- [<span data-ttu-id="30cb0-138">Remove-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="30cb0-138">Remove-ApplicationAccessPolicy</span></span>](/powershell/module/skype/remove-csapplicationaccesspolicy)
