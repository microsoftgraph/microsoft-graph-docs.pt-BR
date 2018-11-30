---
title: tipo de enum deviceComplianceActionType
description: Enumeração de tipo de ação de agendadas
ms.openlocfilehash: 98e54f163663cc041a3e3c31123504c051884309
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036203"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="f01f0-103">tipo de enum deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="f01f0-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="f01f0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f01f0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f01f0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f01f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f01f0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f01f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f01f0-107">Enumeração de tipo de ação de agendadas</span><span class="sxs-lookup"><span data-stu-id="f01f0-107">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="f01f0-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f01f0-108">Members</span></span>
|<span data-ttu-id="f01f0-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f01f0-109">Member</span></span>|<span data-ttu-id="f01f0-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f01f0-110">Value</span></span>|<span data-ttu-id="f01f0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f01f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f01f0-112">noAction</span><span class="sxs-lookup"><span data-stu-id="f01f0-112">noAction</span></span>|<span data-ttu-id="f01f0-113">0</span><span class="sxs-lookup"><span data-stu-id="f01f0-113">0</span></span>|<span data-ttu-id="f01f0-114">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="f01f0-114">No Action</span></span>|
|<span data-ttu-id="f01f0-115">notificação</span><span class="sxs-lookup"><span data-stu-id="f01f0-115">notification</span></span>|<span data-ttu-id="f01f0-116">1</span><span class="sxs-lookup"><span data-stu-id="f01f0-116">1</span></span>|<span data-ttu-id="f01f0-117">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="f01f0-117">Send Notification</span></span>|
|<span data-ttu-id="f01f0-118">bloquear</span><span class="sxs-lookup"><span data-stu-id="f01f0-118">block</span></span>|<span data-ttu-id="f01f0-119">2</span><span class="sxs-lookup"><span data-stu-id="f01f0-119">2</span></span>|<span data-ttu-id="f01f0-120">Bloquear o dispositivo em AAD</span><span class="sxs-lookup"><span data-stu-id="f01f0-120">Block the device in AAD</span></span>|
|<span data-ttu-id="f01f0-121">retirar</span><span class="sxs-lookup"><span data-stu-id="f01f0-121">retire</span></span>|<span data-ttu-id="f01f0-122">3</span><span class="sxs-lookup"><span data-stu-id="f01f0-122">3</span></span>|<span data-ttu-id="f01f0-123">Desative o dispositivo</span><span class="sxs-lookup"><span data-stu-id="f01f0-123">Retire the device</span></span>|
|<span data-ttu-id="f01f0-124">apagar</span><span class="sxs-lookup"><span data-stu-id="f01f0-124">wipe</span></span>|<span data-ttu-id="f01f0-125">4</span><span class="sxs-lookup"><span data-stu-id="f01f0-125">4</span></span>|<span data-ttu-id="f01f0-126">Apagar dispositivo</span><span class="sxs-lookup"><span data-stu-id="f01f0-126">Wipe the device</span></span>|
|<span data-ttu-id="f01f0-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="f01f0-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="f01f0-128">5</span><span class="sxs-lookup"><span data-stu-id="f01f0-128">5</span></span>|<span data-ttu-id="f01f0-129">Remover o recurso perfis de acesso do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f01f0-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="f01f0-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="f01f0-130">pushNotification</span></span>|<span data-ttu-id="f01f0-131">9</span><span class="sxs-lookup"><span data-stu-id="f01f0-131">9</span></span>|<span data-ttu-id="f01f0-132">Enviar notificação por push para dispositivos</span><span class="sxs-lookup"><span data-stu-id="f01f0-132">Send push notification to device</span></span>|
|<span data-ttu-id="f01f0-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="f01f0-133">remoteLock</span></span>|<span data-ttu-id="f01f0-134">10</span><span class="sxs-lookup"><span data-stu-id="f01f0-134">10</span></span>|<span data-ttu-id="f01f0-135">Bloquear remotamente o dispositivo</span><span class="sxs-lookup"><span data-stu-id="f01f0-135">Remotely lock the device</span></span>|





