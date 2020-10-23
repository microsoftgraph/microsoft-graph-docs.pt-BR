---
title: tipo de enumeração ManagementState
description: Estado de gerenciamento do dispositivo no Microsoft Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0ce5fc93bfd48d4beaccac1552573c228f1e6f09
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725439"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="1e712-103">tipo de enumeração ManagementState</span><span class="sxs-lookup"><span data-stu-id="1e712-103">managementState enum type</span></span>

<span data-ttu-id="1e712-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e712-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e712-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e712-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e712-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e712-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e712-107">Estado de gerenciamento do dispositivo no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="1e712-107">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="1e712-108">Membros</span><span class="sxs-lookup"><span data-stu-id="1e712-108">Members</span></span>
|<span data-ttu-id="1e712-109">Membro</span><span class="sxs-lookup"><span data-stu-id="1e712-109">Member</span></span>|<span data-ttu-id="1e712-110">Valor</span><span class="sxs-lookup"><span data-stu-id="1e712-110">Value</span></span>|<span data-ttu-id="1e712-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e712-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e712-112">Managed</span><span class="sxs-lookup"><span data-stu-id="1e712-112">managed</span></span>|<span data-ttu-id="1e712-113">,0</span><span class="sxs-lookup"><span data-stu-id="1e712-113">0</span></span>|<span data-ttu-id="1e712-114">O dispositivo está sob gerenciamento</span><span class="sxs-lookup"><span data-stu-id="1e712-114">The device is under management</span></span>|
|<span data-ttu-id="1e712-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="1e712-115">retirePending</span></span>|<span data-ttu-id="1e712-116">1</span><span class="sxs-lookup"><span data-stu-id="1e712-116">1</span></span>|<span data-ttu-id="1e712-117">Um comando de desativação está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="1e712-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="1e712-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="1e712-118">retireFailed</span></span>|<span data-ttu-id="1e712-119">duas</span><span class="sxs-lookup"><span data-stu-id="1e712-119">2</span></span>|<span data-ttu-id="1e712-120">Falha no comando de desativação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="1e712-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="1e712-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="1e712-121">wipePending</span></span>|<span data-ttu-id="1e712-122">3D</span><span class="sxs-lookup"><span data-stu-id="1e712-122">3</span></span>|<span data-ttu-id="1e712-123">Um comando de apagamento está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="1e712-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="1e712-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="1e712-124">wipeFailed</span></span>|<span data-ttu-id="1e712-125">4 </span><span class="sxs-lookup"><span data-stu-id="1e712-125">4</span></span>|<span data-ttu-id="1e712-126">Falha no comando apagar no dispositivo</span><span class="sxs-lookup"><span data-stu-id="1e712-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="1e712-127">íntegro</span><span class="sxs-lookup"><span data-stu-id="1e712-127">unhealthy</span></span>|<span data-ttu-id="1e712-128">5 </span><span class="sxs-lookup"><span data-stu-id="1e712-128">5</span></span>|<span data-ttu-id="1e712-129">O dispositivo não está íntegro.</span><span class="sxs-lookup"><span data-stu-id="1e712-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="1e712-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="1e712-130">deletePending</span></span>|<span data-ttu-id="1e712-131">6 </span><span class="sxs-lookup"><span data-stu-id="1e712-131">6</span></span>|<span data-ttu-id="1e712-132">Um comando delete está ocorrendo no dispositivo</span><span class="sxs-lookup"><span data-stu-id="1e712-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="1e712-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="1e712-133">retireIssued</span></span>|<span data-ttu-id="1e712-134">7 </span><span class="sxs-lookup"><span data-stu-id="1e712-134">7</span></span>|<span data-ttu-id="1e712-135">Um comando de retirada foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="1e712-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="1e712-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="1e712-136">wipeIssued</span></span>|<span data-ttu-id="1e712-137">8 </span><span class="sxs-lookup"><span data-stu-id="1e712-137">8</span></span>|<span data-ttu-id="1e712-138">Um comando de apagamento foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="1e712-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="1e712-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="1e712-139">wipeCanceled</span></span>|<span data-ttu-id="1e712-140">9 </span><span class="sxs-lookup"><span data-stu-id="1e712-140">9</span></span>|<span data-ttu-id="1e712-141">Um comando de apagamento para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="1e712-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="1e712-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="1e712-142">retireCanceled</span></span>|<span data-ttu-id="1e712-143">10 </span><span class="sxs-lookup"><span data-stu-id="1e712-143">10</span></span>|<span data-ttu-id="1e712-144">Um comando de desativação para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="1e712-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="1e712-145">recém-descobertas</span><span class="sxs-lookup"><span data-stu-id="1e712-145">discovered</span></span>|<span data-ttu-id="1e712-146">11</span><span class="sxs-lookup"><span data-stu-id="1e712-146">11</span></span>|<span data-ttu-id="1e712-147">O dispositivo é descoberto, mas não está totalmente inscrito.</span><span class="sxs-lookup"><span data-stu-id="1e712-147">The device is discovered but not fully enrolled.</span></span>|





