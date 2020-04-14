---
title: tipo de enumeração ManagementState
description: Estado de gerenciamento do dispositivo no Microsoft Intune.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 88aef8765229a573818267c78e653000e3160dd3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443867"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="e11c9-103">tipo de enumeração ManagementState</span><span class="sxs-lookup"><span data-stu-id="e11c9-103">managementState enum type</span></span>

<span data-ttu-id="e11c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e11c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e11c9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e11c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e11c9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e11c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e11c9-107">Estado de gerenciamento do dispositivo no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="e11c9-107">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="e11c9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e11c9-108">Members</span></span>
|<span data-ttu-id="e11c9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e11c9-109">Member</span></span>|<span data-ttu-id="e11c9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e11c9-110">Value</span></span>|<span data-ttu-id="e11c9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e11c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e11c9-112">Managed</span><span class="sxs-lookup"><span data-stu-id="e11c9-112">managed</span></span>|<span data-ttu-id="e11c9-113">,0</span><span class="sxs-lookup"><span data-stu-id="e11c9-113">0</span></span>|<span data-ttu-id="e11c9-114">O dispositivo está sob gerenciamento</span><span class="sxs-lookup"><span data-stu-id="e11c9-114">The device is under management</span></span>|
|<span data-ttu-id="e11c9-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="e11c9-115">retirePending</span></span>|<span data-ttu-id="e11c9-116">1</span><span class="sxs-lookup"><span data-stu-id="e11c9-116">1</span></span>|<span data-ttu-id="e11c9-117">Um comando de desativação está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="e11c9-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="e11c9-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="e11c9-118">retireFailed</span></span>|<span data-ttu-id="e11c9-119">duas</span><span class="sxs-lookup"><span data-stu-id="e11c9-119">2</span></span>|<span data-ttu-id="e11c9-120">Falha no comando de desativação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="e11c9-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="e11c9-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="e11c9-121">wipePending</span></span>|<span data-ttu-id="e11c9-122">3D</span><span class="sxs-lookup"><span data-stu-id="e11c9-122">3</span></span>|<span data-ttu-id="e11c9-123">Um comando de apagamento está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="e11c9-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="e11c9-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="e11c9-124">wipeFailed</span></span>|<span data-ttu-id="e11c9-125">4 </span><span class="sxs-lookup"><span data-stu-id="e11c9-125">4</span></span>|<span data-ttu-id="e11c9-126">Falha no comando apagar no dispositivo</span><span class="sxs-lookup"><span data-stu-id="e11c9-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="e11c9-127">íntegro</span><span class="sxs-lookup"><span data-stu-id="e11c9-127">unhealthy</span></span>|<span data-ttu-id="e11c9-128">5 </span><span class="sxs-lookup"><span data-stu-id="e11c9-128">5</span></span>|<span data-ttu-id="e11c9-129">O dispositivo não está íntegro.</span><span class="sxs-lookup"><span data-stu-id="e11c9-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="e11c9-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="e11c9-130">deletePending</span></span>|<span data-ttu-id="e11c9-131">6 </span><span class="sxs-lookup"><span data-stu-id="e11c9-131">6</span></span>|<span data-ttu-id="e11c9-132">Um comando delete está ocorrendo no dispositivo</span><span class="sxs-lookup"><span data-stu-id="e11c9-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="e11c9-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="e11c9-133">retireIssued</span></span>|<span data-ttu-id="e11c9-134">7 </span><span class="sxs-lookup"><span data-stu-id="e11c9-134">7</span></span>|<span data-ttu-id="e11c9-135">Um comando de retirada foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="e11c9-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="e11c9-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="e11c9-136">wipeIssued</span></span>|<span data-ttu-id="e11c9-137">8 </span><span class="sxs-lookup"><span data-stu-id="e11c9-137">8</span></span>|<span data-ttu-id="e11c9-138">Um comando de apagamento foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="e11c9-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="e11c9-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="e11c9-139">wipeCanceled</span></span>|<span data-ttu-id="e11c9-140">9 </span><span class="sxs-lookup"><span data-stu-id="e11c9-140">9</span></span>|<span data-ttu-id="e11c9-141">Um comando de apagamento para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="e11c9-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="e11c9-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="e11c9-142">retireCanceled</span></span>|<span data-ttu-id="e11c9-143">10 </span><span class="sxs-lookup"><span data-stu-id="e11c9-143">10</span></span>|<span data-ttu-id="e11c9-144">Um comando de desativação para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="e11c9-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="e11c9-145">recém-descobertas</span><span class="sxs-lookup"><span data-stu-id="e11c9-145">discovered</span></span>|<span data-ttu-id="e11c9-146">11</span><span class="sxs-lookup"><span data-stu-id="e11c9-146">11</span></span>|<span data-ttu-id="e11c9-147">O dispositivo é descoberto, mas não está totalmente inscrito.</span><span class="sxs-lookup"><span data-stu-id="e11c9-147">The device is discovered but not fully enrolled.</span></span>|



