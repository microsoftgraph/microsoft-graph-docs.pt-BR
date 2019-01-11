---
title: tipo de enum deviceComplianceActionType
description: Enumeração de tipo de ação de agendadas
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e2b89dbdaa3e67918b1b0c3e76eb6638e492994c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881869"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="2c2f8-103">tipo de enum deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="2c2f8-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="2c2f8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2c2f8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c2f8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2c2f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c2f8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2c2f8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c2f8-107">Enumeração de tipo de ação de agendadas</span><span class="sxs-lookup"><span data-stu-id="2c2f8-107">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="2c2f8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2c2f8-108">Members</span></span>
|<span data-ttu-id="2c2f8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2c2f8-109">Member</span></span>|<span data-ttu-id="2c2f8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2c2f8-110">Value</span></span>|<span data-ttu-id="2c2f8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c2f8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c2f8-112">noAction</span><span class="sxs-lookup"><span data-stu-id="2c2f8-112">noAction</span></span>|<span data-ttu-id="2c2f8-113">0</span><span class="sxs-lookup"><span data-stu-id="2c2f8-113">0</span></span>|<span data-ttu-id="2c2f8-114">Nenhuma ação</span><span class="sxs-lookup"><span data-stu-id="2c2f8-114">No Action</span></span>|
|<span data-ttu-id="2c2f8-115">notificação</span><span class="sxs-lookup"><span data-stu-id="2c2f8-115">notification</span></span>|<span data-ttu-id="2c2f8-116">1</span><span class="sxs-lookup"><span data-stu-id="2c2f8-116">1</span></span>|<span data-ttu-id="2c2f8-117">Enviar notificação</span><span class="sxs-lookup"><span data-stu-id="2c2f8-117">Send Notification</span></span>|
|<span data-ttu-id="2c2f8-118">bloquear</span><span class="sxs-lookup"><span data-stu-id="2c2f8-118">block</span></span>|<span data-ttu-id="2c2f8-119">2</span><span class="sxs-lookup"><span data-stu-id="2c2f8-119">2</span></span>|<span data-ttu-id="2c2f8-120">Bloquear o dispositivo em AAD</span><span class="sxs-lookup"><span data-stu-id="2c2f8-120">Block the device in AAD</span></span>|
|<span data-ttu-id="2c2f8-121">retirar</span><span class="sxs-lookup"><span data-stu-id="2c2f8-121">retire</span></span>|<span data-ttu-id="2c2f8-122">3</span><span class="sxs-lookup"><span data-stu-id="2c2f8-122">3</span></span>|<span data-ttu-id="2c2f8-123">Desative o dispositivo</span><span class="sxs-lookup"><span data-stu-id="2c2f8-123">Retire the device</span></span>|
|<span data-ttu-id="2c2f8-124">apagar</span><span class="sxs-lookup"><span data-stu-id="2c2f8-124">wipe</span></span>|<span data-ttu-id="2c2f8-125">4</span><span class="sxs-lookup"><span data-stu-id="2c2f8-125">4</span></span>|<span data-ttu-id="2c2f8-126">Apagar dispositivo</span><span class="sxs-lookup"><span data-stu-id="2c2f8-126">Wipe the device</span></span>|
|<span data-ttu-id="2c2f8-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="2c2f8-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="2c2f8-128">5</span><span class="sxs-lookup"><span data-stu-id="2c2f8-128">5</span></span>|<span data-ttu-id="2c2f8-129">Remover o recurso perfis de acesso do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2c2f8-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="2c2f8-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="2c2f8-130">pushNotification</span></span>|<span data-ttu-id="2c2f8-131">9</span><span class="sxs-lookup"><span data-stu-id="2c2f8-131">9</span></span>|<span data-ttu-id="2c2f8-132">Enviar notificação por push para dispositivos</span><span class="sxs-lookup"><span data-stu-id="2c2f8-132">Send push notification to device</span></span>|
|<span data-ttu-id="2c2f8-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="2c2f8-133">remoteLock</span></span>|<span data-ttu-id="2c2f8-134">10</span><span class="sxs-lookup"><span data-stu-id="2c2f8-134">10</span></span>|<span data-ttu-id="2c2f8-135">Bloquear remotamente o dispositivo</span><span class="sxs-lookup"><span data-stu-id="2c2f8-135">Remotely lock the device</span></span>|





