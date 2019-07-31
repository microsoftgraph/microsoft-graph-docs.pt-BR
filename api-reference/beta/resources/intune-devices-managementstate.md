---
title: tipo de enumeração ManagementState
description: Estado de gerenciamento do dispositivo no Microsoft Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 928f2c1c9e7eb1530bdf7839691cf2469af11077
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968334"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="3bfea-103">tipo de enumeração ManagementState</span><span class="sxs-lookup"><span data-stu-id="3bfea-103">managementState enum type</span></span>

> <span data-ttu-id="3bfea-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3bfea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bfea-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3bfea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bfea-106">Estado de gerenciamento do dispositivo no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="3bfea-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="3bfea-107">Membros</span><span class="sxs-lookup"><span data-stu-id="3bfea-107">Members</span></span>
|<span data-ttu-id="3bfea-108">Membro</span><span class="sxs-lookup"><span data-stu-id="3bfea-108">Member</span></span>|<span data-ttu-id="3bfea-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3bfea-109">Value</span></span>|<span data-ttu-id="3bfea-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bfea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bfea-111">Managed</span><span class="sxs-lookup"><span data-stu-id="3bfea-111">managed</span></span>|<span data-ttu-id="3bfea-112">,0</span><span class="sxs-lookup"><span data-stu-id="3bfea-112">0</span></span>|<span data-ttu-id="3bfea-113">O dispositivo está sob gerenciamento</span><span class="sxs-lookup"><span data-stu-id="3bfea-113">The device is under management</span></span>|
|<span data-ttu-id="3bfea-114">retirePending</span><span class="sxs-lookup"><span data-stu-id="3bfea-114">retirePending</span></span>|<span data-ttu-id="3bfea-115">1</span><span class="sxs-lookup"><span data-stu-id="3bfea-115">1</span></span>|<span data-ttu-id="3bfea-116">Um comando de desativação está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="3bfea-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="3bfea-117">retireFailed</span><span class="sxs-lookup"><span data-stu-id="3bfea-117">retireFailed</span></span>|<span data-ttu-id="3bfea-118">duas</span><span class="sxs-lookup"><span data-stu-id="3bfea-118">2</span></span>|<span data-ttu-id="3bfea-119">Falha no comando de desativação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="3bfea-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="3bfea-120">wipePending</span><span class="sxs-lookup"><span data-stu-id="3bfea-120">wipePending</span></span>|<span data-ttu-id="3bfea-121">3D</span><span class="sxs-lookup"><span data-stu-id="3bfea-121">3</span></span>|<span data-ttu-id="3bfea-122">Um comando de apagamento está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="3bfea-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="3bfea-123">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="3bfea-123">wipeFailed</span></span>|<span data-ttu-id="3bfea-124">quatro</span><span class="sxs-lookup"><span data-stu-id="3bfea-124">4</span></span>|<span data-ttu-id="3bfea-125">Falha no comando apagar no dispositivo</span><span class="sxs-lookup"><span data-stu-id="3bfea-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="3bfea-126">íntegro</span><span class="sxs-lookup"><span data-stu-id="3bfea-126">unhealthy</span></span>|<span data-ttu-id="3bfea-127">0,5</span><span class="sxs-lookup"><span data-stu-id="3bfea-127">5</span></span>|<span data-ttu-id="3bfea-128">O dispositivo não está íntegro.</span><span class="sxs-lookup"><span data-stu-id="3bfea-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="3bfea-129">deletePending</span><span class="sxs-lookup"><span data-stu-id="3bfea-129">deletePending</span></span>|<span data-ttu-id="3bfea-130">6</span><span class="sxs-lookup"><span data-stu-id="3bfea-130">6</span></span>|<span data-ttu-id="3bfea-131">Um comando delete está ocorrendo no dispositivo</span><span class="sxs-lookup"><span data-stu-id="3bfea-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="3bfea-132">retireIssued</span><span class="sxs-lookup"><span data-stu-id="3bfea-132">retireIssued</span></span>|<span data-ttu-id="3bfea-133">178</span><span class="sxs-lookup"><span data-stu-id="3bfea-133">7</span></span>|<span data-ttu-id="3bfea-134">Um comando de retirada foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="3bfea-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="3bfea-135">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="3bfea-135">wipeIssued</span></span>|<span data-ttu-id="3bfea-136">8 </span><span class="sxs-lookup"><span data-stu-id="3bfea-136">8</span></span>|<span data-ttu-id="3bfea-137">Um comando de apagamento foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="3bfea-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="3bfea-138">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="3bfea-138">wipeCanceled</span></span>|<span data-ttu-id="3bfea-139">9 </span><span class="sxs-lookup"><span data-stu-id="3bfea-139">9</span></span>|<span data-ttu-id="3bfea-140">Um comando de apagamento para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="3bfea-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="3bfea-141">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="3bfea-141">retireCanceled</span></span>|<span data-ttu-id="3bfea-142">10 </span><span class="sxs-lookup"><span data-stu-id="3bfea-142">10</span></span>|<span data-ttu-id="3bfea-143">Um comando de desativação para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="3bfea-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="3bfea-144">recém-descobertas</span><span class="sxs-lookup"><span data-stu-id="3bfea-144">discovered</span></span>|<span data-ttu-id="3bfea-145">11</span><span class="sxs-lookup"><span data-stu-id="3bfea-145">11</span></span>|<span data-ttu-id="3bfea-146">O dispositivo é descoberto, mas não está totalmente inscrito.</span><span class="sxs-lookup"><span data-stu-id="3bfea-146">The device is discovered but not fully enrolled.</span></span>|





