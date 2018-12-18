---
title: tipo de enum deviceComplianceActionType
description: Enumeração de tipo de ação de agendadas
author: tfitzmac
ms.openlocfilehash: 9fd0a8bd045ad04fe0acf55f899e693d7fcce5d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335683"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="6bec8-103">tipo de enum deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="6bec8-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="6bec8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6bec8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bec8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6bec8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6bec8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6bec8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bec8-107">Enumeração de tipo de ação de agendadas</span><span class="sxs-lookup"><span data-stu-id="6bec8-107">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="6bec8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6bec8-108">Members</span></span>
|<span data-ttu-id="6bec8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6bec8-109">Member</span></span>|<span data-ttu-id="6bec8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6bec8-110">Value</span></span>|<span data-ttu-id="6bec8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bec8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bec8-112">noAction</span><span class="sxs-lookup"><span data-stu-id="6bec8-112">noAction</span></span>|<span data-ttu-id="6bec8-113">0</span><span class="sxs-lookup"><span data-stu-id="6bec8-113">0</span></span>|<span data-ttu-id="6bec8-114">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="6bec8-114">No Action</span></span>|
|<span data-ttu-id="6bec8-115">notificação</span><span class="sxs-lookup"><span data-stu-id="6bec8-115">notification</span></span>|<span data-ttu-id="6bec8-116">1</span><span class="sxs-lookup"><span data-stu-id="6bec8-116">1</span></span>|<span data-ttu-id="6bec8-117">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="6bec8-117">Send Notification</span></span>|
|<span data-ttu-id="6bec8-118">bloquear</span><span class="sxs-lookup"><span data-stu-id="6bec8-118">block</span></span>|<span data-ttu-id="6bec8-119">2</span><span class="sxs-lookup"><span data-stu-id="6bec8-119">2</span></span>|<span data-ttu-id="6bec8-120">Bloquear o dispositivo em AAD</span><span class="sxs-lookup"><span data-stu-id="6bec8-120">Block the device in AAD</span></span>|
|<span data-ttu-id="6bec8-121">retirar</span><span class="sxs-lookup"><span data-stu-id="6bec8-121">retire</span></span>|<span data-ttu-id="6bec8-122">3</span><span class="sxs-lookup"><span data-stu-id="6bec8-122">3</span></span>|<span data-ttu-id="6bec8-123">Desative o dispositivo</span><span class="sxs-lookup"><span data-stu-id="6bec8-123">Retire the device</span></span>|
|<span data-ttu-id="6bec8-124">apagar</span><span class="sxs-lookup"><span data-stu-id="6bec8-124">wipe</span></span>|<span data-ttu-id="6bec8-125">4</span><span class="sxs-lookup"><span data-stu-id="6bec8-125">4</span></span>|<span data-ttu-id="6bec8-126">Apagar dispositivo</span><span class="sxs-lookup"><span data-stu-id="6bec8-126">Wipe the device</span></span>|
|<span data-ttu-id="6bec8-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="6bec8-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="6bec8-128">5</span><span class="sxs-lookup"><span data-stu-id="6bec8-128">5</span></span>|<span data-ttu-id="6bec8-129">Remover o recurso perfis de acesso do dispositivo</span><span class="sxs-lookup"><span data-stu-id="6bec8-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="6bec8-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="6bec8-130">pushNotification</span></span>|<span data-ttu-id="6bec8-131">9</span><span class="sxs-lookup"><span data-stu-id="6bec8-131">9</span></span>|<span data-ttu-id="6bec8-132">Enviar notificação por push para dispositivos</span><span class="sxs-lookup"><span data-stu-id="6bec8-132">Send push notification to device</span></span>|
|<span data-ttu-id="6bec8-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="6bec8-133">remoteLock</span></span>|<span data-ttu-id="6bec8-134">10</span><span class="sxs-lookup"><span data-stu-id="6bec8-134">10</span></span>|<span data-ttu-id="6bec8-135">Bloquear remotamente o dispositivo</span><span class="sxs-lookup"><span data-stu-id="6bec8-135">Remotely lock the device</span></span>|





