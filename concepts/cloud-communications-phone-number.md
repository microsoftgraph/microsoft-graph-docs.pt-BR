---
title: Gerenciar números de telefone para bots
description: Este artigo descreve como criar um bot que é acessível por meio de um número de telefone.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: d6b71d2db1be951137ca33026f243dae6055c93f
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573569"
---
# <a name="manage-phone-numbers-for-bots"></a><span data-ttu-id="da7cf-103">Gerenciar números de telefone para bots</span><span class="sxs-lookup"><span data-stu-id="da7cf-103">Manage phone numbers for bots</span></span> 

<span data-ttu-id="da7cf-104">Este artigo descreve como criar um bot que é acessível por meio de um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="da7cf-104">This article describes how to create a bot that is reachable through a phone number.</span></span> <span data-ttu-id="da7cf-105">À medida que você cria seu bot, será útil estar familiarizado com os seguintes termos:</span><span class="sxs-lookup"><span data-stu-id="da7cf-105">As you create your bot, it will be helpful to be familiar with the following terms:</span></span>

- <span data-ttu-id="da7cf-106">**Aplicativo** – Um aplicativo hospedado no Azure, também conhecido como **bot**.</span><span class="sxs-lookup"><span data-stu-id="da7cf-106">**Application** – An application that is hosted on Azure, also referred to as a **bot**.</span></span>

- <span data-ttu-id="da7cf-107">**Instância do** aplicativo – Um objeto de usuário desabilitado que pode ser atribuído a um número de telefone que pode ser usado por um bot.</span><span class="sxs-lookup"><span data-stu-id="da7cf-107">**Application instance** – A disabled-user object that can be assigned to a phone number that can be used by a bot.</span></span> <span data-ttu-id="da7cf-108">Isso também é conhecido como uma [conta de recurso](/microsoftteams/manage-resource-accounts).</span><span class="sxs-lookup"><span data-stu-id="da7cf-108">This is also known as a [resource account](/microsoftteams/manage-resource-accounts).</span></span> <span data-ttu-id="da7cf-109">Essa é a única maneira de um número de telefone ser atribuído a um bot.</span><span class="sxs-lookup"><span data-stu-id="da7cf-109">This is the only way a phone number can be assigned to a bot.</span></span>

<span data-ttu-id="da7cf-110">Um aplicativo pode ter várias instâncias de aplicativo e cada locatário pode ter várias instâncias de aplicativo, conforme mostrado na imagem a seguir.</span><span class="sxs-lookup"><span data-stu-id="da7cf-110">One application can have multiple application instances, and each tenant can have multiple application instances, as shown in the following image.</span></span>

![Imagem mostrando um número de telefone com locatários com uma ou mais instâncias de aplicativo](images/communications-app-tenant.PNG)

## <a name="prerequisite---register-a-bot"></a><span data-ttu-id="da7cf-112">Pré-requisito - Registrar um bot</span><span class="sxs-lookup"><span data-stu-id="da7cf-112">Prerequisite - Register a bot</span></span>
<span data-ttu-id="da7cf-113">Para começar, siga as instruções para registrar [um bot de chamada](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html).</span><span class="sxs-lookup"><span data-stu-id="da7cf-113">To get started, follow the instructions to [register a calling bot](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html).</span></span> <span data-ttu-id="da7cf-114">Você precisará de valores de configuração, como ID de bot, ID de aplicativo da Microsoft e senha de aplicativo da Microsoft para usar em seu código.</span><span class="sxs-lookup"><span data-stu-id="da7cf-114">You’ll need config values such as bot ID, Microsoft app ID, and Microsoft app password to use in your code.</span></span>

<span data-ttu-id="da7cf-115">Adicione as seguintes permissões ao bot.</span><span class="sxs-lookup"><span data-stu-id="da7cf-115">Add the following permissions to your bot.</span></span> <span data-ttu-id="da7cf-116">Um administrador de locatário também precisa concordar com essas permissões:</span><span class="sxs-lookup"><span data-stu-id="da7cf-116">A tenant admin needs to consent to these permissions as well:</span></span>

- <span data-ttu-id="da7cf-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="da7cf-117">Calls.AccessMedia.All</span></span>
- <span data-ttu-id="da7cf-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="da7cf-118">Calls.Initiate.All</span></span>
- <span data-ttu-id="da7cf-119">Calls.JoinGroupCall.All</span><span class="sxs-lookup"><span data-stu-id="da7cf-119">Calls.JoinGroupCall.All</span></span>
- <span data-ttu-id="da7cf-120">Calls.JoinGroupCallAsGuest.All</span><span class="sxs-lookup"><span data-stu-id="da7cf-120">Calls.JoinGroupCallAsGuest.All</span></span>

<span data-ttu-id="da7cf-121">Para obter mais informações sobre permissões relacionadas a chamada, consulte [a referência Permissões](permissions-reference.md#calls-permissions).</span><span class="sxs-lookup"><span data-stu-id="da7cf-121">For more information about call-related permissions, see the [Permissions reference](permissions-reference.md#calls-permissions).</span></span>


## <a name="assign-a-phone-number-to-your-bot"></a><span data-ttu-id="da7cf-122">Atribuir um número de telefone ao bot</span><span class="sxs-lookup"><span data-stu-id="da7cf-122">Assign a phone number to your bot</span></span>

<span data-ttu-id="da7cf-123">Atribuir um número de telefone ao bot envolve três etapas:</span><span class="sxs-lookup"><span data-stu-id="da7cf-123">Assigning a phone number to your bot involves three steps:</span></span>

1.  <span data-ttu-id="da7cf-124">Crie uma instância de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="da7cf-124">Create an application instance.</span></span>
2.  <span data-ttu-id="da7cf-125">Atribua licenças do Microsoft 365 à instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="da7cf-125">Assign Microsoft 365 licenses to your application instance.</span></span>
3.  <span data-ttu-id="da7cf-126">Atribua um número de telefone à instância do aplicativo (somente administrador de locatário).</span><span class="sxs-lookup"><span data-stu-id="da7cf-126">Assign a phone number to the application instance (only tenant admin).</span></span>

### <a name="create-an-application-instance"></a><span data-ttu-id="da7cf-127">Criar uma instância de aplicativo</span><span class="sxs-lookup"><span data-stu-id="da7cf-127">Create an application instance</span></span>

<span data-ttu-id="da7cf-128">Se ainda não tiver sido instalado, um administrador de locatário precisará instalar o [Módulo do Skype for Business Online](https://www.microsoft.com/download/details.aspx?id=39366) para o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="da7cf-128">If it hasn't been installed already, a tenant admin needs to install the [Skype for Business Online Module](https://www.microsoft.com/download/details.aspx?id=39366) for PowerShell.</span></span> <span data-ttu-id="da7cf-129">O administrador do locatário deve entrar usando suas credenciais antes de executar o cmdlet.</span><span class="sxs-lookup"><span data-stu-id="da7cf-129">The tenant admin must sign in using their credentials before running the cmdlet.</span></span>

<span data-ttu-id="da7cf-130">Para criar uma nova instância de aplicativo, o administrador de locatário executa o cmdlet a seguir.</span><span class="sxs-lookup"><span data-stu-id="da7cf-130">To create a new application instance, the tenant admin runs the following cmdlet.</span></span>

`PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <user@contoso.com> -ApplicationId <app_id> -DisplayName <bot_display_name>`

<span data-ttu-id="da7cf-131">Quando a instância do aplicativo for criada, use o cmdlet de sincronização.</span><span class="sxs-lookup"><span data-stu-id="da7cf-131">When the application instance is created, use the sync cmdlet.</span></span>

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

<span data-ttu-id="da7cf-132">Para obter mais informações, consulte [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="da7cf-132">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>

### <a name="assign-microsoft-365-licenses-to-your-application-instance"></a><span data-ttu-id="da7cf-133">Atribuir licenças do Microsoft 365 à instância do aplicativo</span><span class="sxs-lookup"><span data-stu-id="da7cf-133">Assign Microsoft 365 licenses to your application instance</span></span>

<span data-ttu-id="da7cf-134">Atribua uma licença de usuário virtual à instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="da7cf-134">Assign a virtual user license to your application instance.</span></span> <span data-ttu-id="da7cf-135">Para obter detalhes, consulte [Phone system virtual user license](/microsoftteams/teams-add-on-licensing/virtual-user).</span><span class="sxs-lookup"><span data-stu-id="da7cf-135">For details, see [Phone system virtual user license](/microsoftteams/teams-add-on-licensing/virtual-user).</span></span>

<span data-ttu-id="da7cf-136">Atribua um plano de chamada à instância do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="da7cf-136">Assign a calling plan to your application instance.</span></span> <span data-ttu-id="da7cf-137">Para obter detalhes, consulte [Planos de chamada para o Microsoft 365](/microsoftteams/calling-plans-for-office-365).</span><span class="sxs-lookup"><span data-stu-id="da7cf-137">For details, see [Calling plans for Microsoft 365](/microsoftteams/calling-plans-for-office-365).</span></span>

### <a name="assign-a-phone-number-to-the-application-instance-only-tenant-admin"></a><span data-ttu-id="da7cf-138">Atribuir um número de telefone à instância do aplicativo (somente administrador de locatário)</span><span class="sxs-lookup"><span data-stu-id="da7cf-138">Assign a phone number to the application instance (only tenant admin)</span></span>

<span data-ttu-id="da7cf-139">Antes de poder configurar os usuários em sua organização para fazer e receber chamadas telefônicas, você deve obter números de telefone para eles.</span><span class="sxs-lookup"><span data-stu-id="da7cf-139">Before you can set up users in your organization to make and receive phone calls, you must get phone numbers for them.</span></span> <span data-ttu-id="da7cf-140">Para obter detalhes, consulte [Obter números de telefone para seus usuários](/microsoftteams/getting-phone-numbers-for-your-users#get-new-phone-numbers-for-your-users).</span><span class="sxs-lookup"><span data-stu-id="da7cf-140">For details, see [Getting phone numbers for your users](/microsoftteams/getting-phone-numbers-for-your-users#get-new-phone-numbers-for-your-users).</span></span>

<span data-ttu-id="da7cf-141">Para atribuir o número de telefone à instância do aplicativo, o administrador do locatário:</span><span class="sxs-lookup"><span data-stu-id="da7cf-141">To assign the phone number to the application instance, the tenant admin:</span></span>

1. <span data-ttu-id="da7cf-142">Entre no centro de administração do Teams como administrador de locatário.</span><span class="sxs-lookup"><span data-stu-id="da7cf-142">Signs in to the Teams admin center as a tenant admin.</span></span>
2. <span data-ttu-id="da7cf-143">Vai para o **Centro de Administração do Teams** Números de  >  **Telefone** de  >  **Voz**.</span><span class="sxs-lookup"><span data-stu-id="da7cf-143">Goes to **Teams Admin center** > **Voice** > **Phone Numbers**.</span></span>
3. <span data-ttu-id="da7cf-144">Atribui um número de telefone de serviço (formato+11D) usando o cmdlet a seguir.</span><span class="sxs-lookup"><span data-stu-id="da7cf-144">Assigns a service phone number (+11D format) using the following cmdlet.</span></span>

  `PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <phone_number>`
  
<span data-ttu-id="da7cf-145">Quando o número de telefone de serviço for atribuído, use o cmdlet de sincronização.</span><span class="sxs-lookup"><span data-stu-id="da7cf-145">When the service phone number is assigned, use the sync cmdlet.</span></span>

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

<span data-ttu-id="da7cf-146">Para obter mais informações, consulte [Set-CsOnlineVoiceApplicationInstance](/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) e [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="da7cf-146">For more information, see [Set-CsOnlineVoiceApplicationInstance](/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>

## <a name="unassign-a-bot-phone-number"></a><span data-ttu-id="da7cf-147">Unassign a bot phone number</span><span class="sxs-lookup"><span data-stu-id="da7cf-147">Unassign a bot phone number</span></span>

<span data-ttu-id="da7cf-148">Use o cmdlet a seguir para desemplacar um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="da7cf-148">Use the following cmdlet to unassign a phone number.</span></span>

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber $null`

><span data-ttu-id="da7cf-149">**Observação:** Atualmente, isso só funciona com números online e não números de roteamento direto (DR).</span><span class="sxs-lookup"><span data-stu-id="da7cf-149">**Note:** Currently this only works with online numbers and not direct routing (DR) numbers.</span></span> <span data-ttu-id="da7cf-150">Este é um problema conhecido.</span><span class="sxs-lookup"><span data-stu-id="da7cf-150">This is a known issue.</span></span>

## <a name="update-a-bot-phone-number"></a><span data-ttu-id="da7cf-151">Atualizar um número de telefone bot</span><span class="sxs-lookup"><span data-stu-id="da7cf-151">Update a bot phone number</span></span>

<span data-ttu-id="da7cf-152">Depois de desatribuição do número, você pode atribuir um número diferente ao bot usando o cmdlet a seguir.</span><span class="sxs-lookup"><span data-stu-id="da7cf-152">After unassigning the number, you can assign a different number to the bot by using the following cmdlet.</span></span>

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <new phone_number>`

## <a name="see-also"></a><span data-ttu-id="da7cf-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="da7cf-153">See also</span></span>

- <span data-ttu-id="da7cf-154">[Exemplo de bot de incidente](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot).</span><span class="sxs-lookup"><span data-stu-id="da7cf-154">[Incident bot sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot).</span></span> 
 - <span data-ttu-id="da7cf-155">Para obter detalhes sobre como implantar, consulte [Deploying the sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample).</span><span class="sxs-lookup"><span data-stu-id="da7cf-155">For details about how to deploy, see [Deploying the sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample).</span></span>
