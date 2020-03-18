---
title: tipo de enumeração ManagementState
description: Estado de gerenciamento do dispositivo no Microsoft Intune.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fd0a4616f6f35c91ae6ce6269d452a00d3275bc5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783925"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="e5f0f-103">tipo de enumeração ManagementState</span><span class="sxs-lookup"><span data-stu-id="e5f0f-103">managementState enum type</span></span>

> <span data-ttu-id="e5f0f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5f0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5f0f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5f0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5f0f-106">Estado de gerenciamento do dispositivo no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="e5f0f-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="e5f0f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e5f0f-107">Members</span></span>
|<span data-ttu-id="e5f0f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e5f0f-108">Member</span></span>|<span data-ttu-id="e5f0f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e5f0f-109">Value</span></span>|<span data-ttu-id="e5f0f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5f0f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5f0f-111">Managed</span><span class="sxs-lookup"><span data-stu-id="e5f0f-111">managed</span></span>|<span data-ttu-id="e5f0f-112">,0</span><span class="sxs-lookup"><span data-stu-id="e5f0f-112">0</span></span>|<span data-ttu-id="e5f0f-113">O dispositivo está sob gerenciamento</span><span class="sxs-lookup"><span data-stu-id="e5f0f-113">The device is under management</span></span>|
|<span data-ttu-id="e5f0f-114">retirePending</span><span class="sxs-lookup"><span data-stu-id="e5f0f-114">retirePending</span></span>|<span data-ttu-id="e5f0f-115">1</span><span class="sxs-lookup"><span data-stu-id="e5f0f-115">1</span></span>|<span data-ttu-id="e5f0f-116">Um comando de desativação está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="e5f0f-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="e5f0f-117">retireFailed</span><span class="sxs-lookup"><span data-stu-id="e5f0f-117">retireFailed</span></span>|<span data-ttu-id="e5f0f-118">duas</span><span class="sxs-lookup"><span data-stu-id="e5f0f-118">2</span></span>|<span data-ttu-id="e5f0f-119">Falha no comando de desativação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="e5f0f-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="e5f0f-120">wipePending</span><span class="sxs-lookup"><span data-stu-id="e5f0f-120">wipePending</span></span>|<span data-ttu-id="e5f0f-121">3D</span><span class="sxs-lookup"><span data-stu-id="e5f0f-121">3</span></span>|<span data-ttu-id="e5f0f-122">Um comando de apagamento está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="e5f0f-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="e5f0f-123">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="e5f0f-123">wipeFailed</span></span>|<span data-ttu-id="e5f0f-124">4 </span><span class="sxs-lookup"><span data-stu-id="e5f0f-124">4</span></span>|<span data-ttu-id="e5f0f-125">Falha no comando apagar no dispositivo</span><span class="sxs-lookup"><span data-stu-id="e5f0f-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="e5f0f-126">íntegro</span><span class="sxs-lookup"><span data-stu-id="e5f0f-126">unhealthy</span></span>|<span data-ttu-id="e5f0f-127">5 </span><span class="sxs-lookup"><span data-stu-id="e5f0f-127">5</span></span>|<span data-ttu-id="e5f0f-128">O dispositivo não está íntegro.</span><span class="sxs-lookup"><span data-stu-id="e5f0f-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="e5f0f-129">deletePending</span><span class="sxs-lookup"><span data-stu-id="e5f0f-129">deletePending</span></span>|<span data-ttu-id="e5f0f-130">6 </span><span class="sxs-lookup"><span data-stu-id="e5f0f-130">6</span></span>|<span data-ttu-id="e5f0f-131">Um comando delete está ocorrendo no dispositivo</span><span class="sxs-lookup"><span data-stu-id="e5f0f-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="e5f0f-132">retireIssued</span><span class="sxs-lookup"><span data-stu-id="e5f0f-132">retireIssued</span></span>|<span data-ttu-id="e5f0f-133">7 </span><span class="sxs-lookup"><span data-stu-id="e5f0f-133">7</span></span>|<span data-ttu-id="e5f0f-134">Um comando de retirada foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="e5f0f-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="e5f0f-135">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="e5f0f-135">wipeIssued</span></span>|<span data-ttu-id="e5f0f-136">8 </span><span class="sxs-lookup"><span data-stu-id="e5f0f-136">8</span></span>|<span data-ttu-id="e5f0f-137">Um comando de apagamento foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="e5f0f-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="e5f0f-138">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="e5f0f-138">wipeCanceled</span></span>|<span data-ttu-id="e5f0f-139">9 </span><span class="sxs-lookup"><span data-stu-id="e5f0f-139">9</span></span>|<span data-ttu-id="e5f0f-140">Um comando de apagamento para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="e5f0f-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="e5f0f-141">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="e5f0f-141">retireCanceled</span></span>|<span data-ttu-id="e5f0f-142">10 </span><span class="sxs-lookup"><span data-stu-id="e5f0f-142">10</span></span>|<span data-ttu-id="e5f0f-143">Um comando de desativação para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="e5f0f-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="e5f0f-144">recém-descobertas</span><span class="sxs-lookup"><span data-stu-id="e5f0f-144">discovered</span></span>|<span data-ttu-id="e5f0f-145">11</span><span class="sxs-lookup"><span data-stu-id="e5f0f-145">11</span></span>|<span data-ttu-id="e5f0f-146">O dispositivo é descoberto, mas não está totalmente inscrito.</span><span class="sxs-lookup"><span data-stu-id="e5f0f-146">The device is discovered but not fully enrolled.</span></span>|



