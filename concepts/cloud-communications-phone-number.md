---
title: Gerenciar números de telefone para bots
description: Este artigo descreve como criar um bot alcançável por meio de um número de telefone.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 679ee5ac5da1a8754d7517dfb9f35bd9e0a071db
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289369"
---
# <a name="manage-phone-numbers-for-bots"></a><span data-ttu-id="c41e1-103">Gerenciar números de telefone para bots</span><span class="sxs-lookup"><span data-stu-id="c41e1-103">Manage phone numbers for bots</span></span> 

<span data-ttu-id="c41e1-104">Este artigo descreve como criar um bot alcançável por meio de um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="c41e1-104">This article describes how to create a bot that is reachable through a phone number.</span></span> <span data-ttu-id="c41e1-105">Ao criar o bot, será útil estar familiarizado com os seguintes termos:</span><span class="sxs-lookup"><span data-stu-id="c41e1-105">As you create your bot, it will be helpful to be familiar with the following terms:</span></span>

- <span data-ttu-id="c41e1-106">**Aplicativo** – um aplicativo hospedado no Azure, também chamado de **bot**.</span><span class="sxs-lookup"><span data-stu-id="c41e1-106">**Application** – An application that is hosted on Azure, also referred to as a **bot**.</span></span>

- <span data-ttu-id="c41e1-107">**Instância de aplicativo** – um objeto de usuário desabilitado que pode ser atribuído a um número de telefone que pode ser usado por um bot.</span><span class="sxs-lookup"><span data-stu-id="c41e1-107">**Application instance** – A disabled-user object that can be assigned to a phone number that can be used by a bot.</span></span> <span data-ttu-id="c41e1-108">Isso também é conhecido como uma [conta de recurso](/microsoftteams/manage-resource-accounts).</span><span class="sxs-lookup"><span data-stu-id="c41e1-108">This is also known as a [resource account](/microsoftteams/manage-resource-accounts).</span></span> <span data-ttu-id="c41e1-109">Essa é a única maneira de atribuir um número de telefone a um bot.</span><span class="sxs-lookup"><span data-stu-id="c41e1-109">This is the only way a phone number can be assigned to a bot.</span></span>

<span data-ttu-id="c41e1-110">Um aplicativo pode ter várias instâncias de aplicativo, e cada locatário pode ter várias instâncias de aplicativo, conforme mostrado na imagem a seguir.</span><span class="sxs-lookup"><span data-stu-id="c41e1-110">One application can have multiple application instances, and each tenant can have multiple application instances, as shown in the following image.</span></span>

![Imagem mostrando um número de telefone com locatários com uma ou mais instâncias de aplicativo](images/communications-app-tenant.PNG)

## <a name="prerequisite---register-a-bot"></a><span data-ttu-id="c41e1-112">Pré-requisitos-registrar um bot</span><span class="sxs-lookup"><span data-stu-id="c41e1-112">Prerequisite - Register a bot</span></span>
<span data-ttu-id="c41e1-113">Para começar, siga as instruções para [registrar um bot de chamada](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html).</span><span class="sxs-lookup"><span data-stu-id="c41e1-113">To get started, follow the instructions to [register a calling bot](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html).</span></span> <span data-ttu-id="c41e1-114">Você precisará de valores de configuração como ID do bot, ID do aplicativo da Microsoft e senha do Microsoft App para usar no seu código.</span><span class="sxs-lookup"><span data-stu-id="c41e1-114">You’ll need config values such as bot ID, Microsoft app ID, and Microsoft app password to use in your code.</span></span>

<span data-ttu-id="c41e1-115">Adicione as seguintes permissões ao bot.</span><span class="sxs-lookup"><span data-stu-id="c41e1-115">Add the following permissions to your bot.</span></span> <span data-ttu-id="c41e1-116">Um administrador de locatários também precisa concordar com essas permissões:</span><span class="sxs-lookup"><span data-stu-id="c41e1-116">A tenant admin needs to consent to these permissions as well:</span></span>

- <span data-ttu-id="c41e1-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="c41e1-117">Calls.AccessMedia.All</span></span>
- <span data-ttu-id="c41e1-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="c41e1-118">Calls.Initiate.All</span></span>
- <span data-ttu-id="c41e1-119">Calls.JoinGroupCall.All</span><span class="sxs-lookup"><span data-stu-id="c41e1-119">Calls.JoinGroupCall.All</span></span>
- <span data-ttu-id="c41e1-120">Calls. JoinGroupCallAsGuest. All</span><span class="sxs-lookup"><span data-stu-id="c41e1-120">Calls.JoinGroupCallAsGuest.All</span></span>

<span data-ttu-id="c41e1-121">Para obter mais informações sobre permissões relacionadas a chamadas, consulte a [referência de permissões](permissions-reference.md#calls-permissions).</span><span class="sxs-lookup"><span data-stu-id="c41e1-121">For more information about call-related permissions, see the [Permissions reference](permissions-reference.md#calls-permissions).</span></span>


## <a name="assign-a-phone-number-to-your-bot"></a><span data-ttu-id="c41e1-122">Atribuir um número de telefone ao bot</span><span class="sxs-lookup"><span data-stu-id="c41e1-122">Assign a phone number to your bot</span></span>

<span data-ttu-id="c41e1-123">Atribuir um número de telefone ao bot envolve três etapas:</span><span class="sxs-lookup"><span data-stu-id="c41e1-123">Assigning a phone number to your bot involves three steps:</span></span>

1.  <span data-ttu-id="c41e1-124">Criar uma instância de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c41e1-124">Create an application instance.</span></span>
2.  <span data-ttu-id="c41e1-125">Atribua uma licença de usuário virtual à sua instância de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c41e1-125">Assign a virtual user license to your application instance.</span></span>
3.  <span data-ttu-id="c41e1-126">Atribuir um número de telefone à instância do aplicativo (somente administrador de locatário).</span><span class="sxs-lookup"><span data-stu-id="c41e1-126">Assign a phone number to the application instance (only tenant admin).</span></span>

### <a name="create-an-application-instance"></a><span data-ttu-id="c41e1-127">Criar uma instância de aplicativo</span><span class="sxs-lookup"><span data-stu-id="c41e1-127">Create an application instance</span></span>

<span data-ttu-id="c41e1-128">Se ainda não tiver sido instalado, um administrador de locatários precisará instalar o [módulo do Skype for Business online](https://www.microsoft.com/download/details.aspx?id=39366) para o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c41e1-128">If it hasn't been installed already, a tenant admin needs to install the [Skype for Business Online Module](https://www.microsoft.com/download/details.aspx?id=39366) for PowerShell.</span></span> <span data-ttu-id="c41e1-129">O administrador de locatários deve entrar usando suas credenciais antes de executar o cmdlet.</span><span class="sxs-lookup"><span data-stu-id="c41e1-129">The tenant admin must sign in using their credentials before running the cmdlet.</span></span>

<span data-ttu-id="c41e1-130">Para criar uma nova instância de aplicativo, o administrador de locatários executa o cmdlet a seguir.</span><span class="sxs-lookup"><span data-stu-id="c41e1-130">To create a new application instance, the tenant admin runs the following cmdlet.</span></span>

`PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <user@contoso.com> -ApplicationId “<app_id>” -DisplayName "<bot_display_name>"`

<span data-ttu-id="c41e1-131">Quando a instância do aplicativo for criada, use o cmdlet Sync.</span><span class="sxs-lookup"><span data-stu-id="c41e1-131">When the application instance is created, use the sync cmdlet.</span></span>

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

### <a name="assign-a-virtual-user-license-to-your-application-instance"></a><span data-ttu-id="c41e1-132">Atribuir uma licença de usuário virtual à sua instância de aplicativo</span><span class="sxs-lookup"><span data-stu-id="c41e1-132">Assign a virtual user license to your application instance</span></span>

<span data-ttu-id="c41e1-133">Atribua uma licença de usuário virtual à sua instância de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c41e1-133">Assign a virtual user license to your application instance.</span></span> <span data-ttu-id="c41e1-134">Para obter detalhes, consulte [licença de usuário virtual do sistema de telefonia](/microsoftteams/teams-add-on-licensing/virtual-user).</span><span class="sxs-lookup"><span data-stu-id="c41e1-134">For details, see [Phone system virtual user license](/microsoftteams/teams-add-on-licensing/virtual-user).</span></span>

### <a name="assign-a-phone-number-to-the-application-instance-only-tenant-admin"></a><span data-ttu-id="c41e1-135">Atribuir um número de telefone à instância do aplicativo (somente administrador de locatário)</span><span class="sxs-lookup"><span data-stu-id="c41e1-135">Assign a phone number to the application instance (only tenant admin)</span></span>

<span data-ttu-id="c41e1-136">Para atribuir o número de telefone à instância do aplicativo, o administrador do locatário:</span><span class="sxs-lookup"><span data-stu-id="c41e1-136">To assign the phone number to the application instance, the tenant admin:</span></span>

1. <span data-ttu-id="c41e1-137">Entra no centro de administração do Microsoft Teams como um administrador de locatários.</span><span class="sxs-lookup"><span data-stu-id="c41e1-137">Signs in to the Teams admin center as a tenant admin.</span></span>
2. <span data-ttu-id="c41e1-138">Vai para os números de telefone de voz do **centro de administração do teams**  >  **Voice**  >  **Phone Numbers**.</span><span class="sxs-lookup"><span data-stu-id="c41e1-138">Goes to **Teams Admin center** > **Voice** > **Phone Numbers**.</span></span>
3. <span data-ttu-id="c41e1-139">Atribui um número de telefone de serviço (+ formato 11D) usando o cmdlet a seguir.</span><span class="sxs-lookup"><span data-stu-id="c41e1-139">Assigns a service phone number (+11D format) using the following cmdlet.</span></span>

  `PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <phone_number>`

## <a name="unassign-a-bot-phone-number"></a><span data-ttu-id="c41e1-140">Cancelar a atribuição de um número de telefone de bot</span><span class="sxs-lookup"><span data-stu-id="c41e1-140">Unassign a bot phone number</span></span>

<span data-ttu-id="c41e1-141">Use o cmdlet a seguir para cancelar a atribuição de um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="c41e1-141">Use the following cmdlet to unassign a phone number.</span></span>

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber $null`

><span data-ttu-id="c41e1-142">**Observação:** Atualmente, isso só funciona com números online e não para os números de roteamento direto (DR).</span><span class="sxs-lookup"><span data-stu-id="c41e1-142">**Note:** Currently this only works with online numbers and not direct routing (DR) numbers.</span></span> <span data-ttu-id="c41e1-143">Este é um problema conhecido.</span><span class="sxs-lookup"><span data-stu-id="c41e1-143">This is a known issue.</span></span>

## <a name="update-a-bot-phone-number"></a><span data-ttu-id="c41e1-144">Atualizar um número de telefone de bot</span><span class="sxs-lookup"><span data-stu-id="c41e1-144">Update a bot phone number</span></span>

<span data-ttu-id="c41e1-145">Depois de cancelar a atribuição do número, você pode atribuir um número diferente ao bot usando o cmdlet a seguir.</span><span class="sxs-lookup"><span data-stu-id="c41e1-145">After unassigning the number, you can assign a different number to the bot by using the following cmdlet.</span></span>

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <new phone_number>`

## <a name="see-also"></a><span data-ttu-id="c41e1-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="c41e1-146">See also</span></span>

- <span data-ttu-id="c41e1-147">[Exemplo de bot de incidentes](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot).</span><span class="sxs-lookup"><span data-stu-id="c41e1-147">[Incident bot sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot).</span></span> 
 - <span data-ttu-id="c41e1-148">Para obter detalhes sobre como implantar o, consulte [Deploying The Sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample).</span><span class="sxs-lookup"><span data-stu-id="c41e1-148">For details about how to deploy, see [Deploying the sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample).</span></span>