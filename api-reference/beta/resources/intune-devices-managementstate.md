---
title: tipo de enumeração ManagementState
description: Estado de gerenciamento do dispositivo no Microsoft Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 78e511e830d58ed1fd22b851759cdb713643746c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081130"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="d3763-103">tipo de enumeração ManagementState</span><span class="sxs-lookup"><span data-stu-id="d3763-103">managementState enum type</span></span>

<span data-ttu-id="d3763-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3763-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3763-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3763-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3763-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3763-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3763-107">Estado de gerenciamento do dispositivo no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="d3763-107">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="d3763-108">Membros</span><span class="sxs-lookup"><span data-stu-id="d3763-108">Members</span></span>
|<span data-ttu-id="d3763-109">Membro</span><span class="sxs-lookup"><span data-stu-id="d3763-109">Member</span></span>|<span data-ttu-id="d3763-110">Valor</span><span class="sxs-lookup"><span data-stu-id="d3763-110">Value</span></span>|<span data-ttu-id="d3763-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3763-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3763-112">Managed</span><span class="sxs-lookup"><span data-stu-id="d3763-112">managed</span></span>|<span data-ttu-id="d3763-113">,0</span><span class="sxs-lookup"><span data-stu-id="d3763-113">0</span></span>|<span data-ttu-id="d3763-114">O dispositivo está sob gerenciamento</span><span class="sxs-lookup"><span data-stu-id="d3763-114">The device is under management</span></span>|
|<span data-ttu-id="d3763-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="d3763-115">retirePending</span></span>|<span data-ttu-id="d3763-116">1 </span><span class="sxs-lookup"><span data-stu-id="d3763-116">1</span></span>|<span data-ttu-id="d3763-117">Um comando de desativação está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="d3763-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="d3763-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="d3763-118">retireFailed</span></span>|<span data-ttu-id="d3763-119">2 </span><span class="sxs-lookup"><span data-stu-id="d3763-119">2</span></span>|<span data-ttu-id="d3763-120">Falha no comando de desativação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="d3763-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="d3763-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="d3763-121">wipePending</span></span>|<span data-ttu-id="d3763-122">3D</span><span class="sxs-lookup"><span data-stu-id="d3763-122">3</span></span>|<span data-ttu-id="d3763-123">Um comando de apagamento está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="d3763-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="d3763-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="d3763-124">wipeFailed</span></span>|<span data-ttu-id="d3763-125">4 </span><span class="sxs-lookup"><span data-stu-id="d3763-125">4</span></span>|<span data-ttu-id="d3763-126">Falha no comando apagar no dispositivo</span><span class="sxs-lookup"><span data-stu-id="d3763-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="d3763-127">íntegro</span><span class="sxs-lookup"><span data-stu-id="d3763-127">unhealthy</span></span>|<span data-ttu-id="d3763-128">5 </span><span class="sxs-lookup"><span data-stu-id="d3763-128">5</span></span>|<span data-ttu-id="d3763-129">O dispositivo não está íntegro.</span><span class="sxs-lookup"><span data-stu-id="d3763-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="d3763-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="d3763-130">deletePending</span></span>|<span data-ttu-id="d3763-131">6 </span><span class="sxs-lookup"><span data-stu-id="d3763-131">6</span></span>|<span data-ttu-id="d3763-132">Um comando delete está ocorrendo no dispositivo</span><span class="sxs-lookup"><span data-stu-id="d3763-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="d3763-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="d3763-133">retireIssued</span></span>|<span data-ttu-id="d3763-134">7 </span><span class="sxs-lookup"><span data-stu-id="d3763-134">7</span></span>|<span data-ttu-id="d3763-135">Um comando de retirada foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="d3763-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="d3763-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="d3763-136">wipeIssued</span></span>|<span data-ttu-id="d3763-137">8 </span><span class="sxs-lookup"><span data-stu-id="d3763-137">8</span></span>|<span data-ttu-id="d3763-138">Um comando de apagamento foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="d3763-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="d3763-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="d3763-139">wipeCanceled</span></span>|<span data-ttu-id="d3763-140">9 </span><span class="sxs-lookup"><span data-stu-id="d3763-140">9</span></span>|<span data-ttu-id="d3763-141">Um comando de apagamento para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="d3763-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="d3763-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="d3763-142">retireCanceled</span></span>|<span data-ttu-id="d3763-143">10 </span><span class="sxs-lookup"><span data-stu-id="d3763-143">10</span></span>|<span data-ttu-id="d3763-144">Um comando de desativação para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="d3763-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="d3763-145">recém-descobertas</span><span class="sxs-lookup"><span data-stu-id="d3763-145">discovered</span></span>|<span data-ttu-id="d3763-146">11 </span><span class="sxs-lookup"><span data-stu-id="d3763-146">11</span></span>|<span data-ttu-id="d3763-147">O dispositivo é descoberto, mas não está totalmente inscrito.</span><span class="sxs-lookup"><span data-stu-id="d3763-147">The device is discovered but not fully enrolled.</span></span>|






