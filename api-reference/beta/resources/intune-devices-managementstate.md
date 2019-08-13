---
title: tipo de enumeração ManagementState
description: Estado de gerenciamento do dispositivo no Microsoft Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a61b9d228589f1d0a1e380ed45720f66faa650af
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372150"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="787bc-103">tipo de enumeração ManagementState</span><span class="sxs-lookup"><span data-stu-id="787bc-103">managementState enum type</span></span>

> <span data-ttu-id="787bc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="787bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="787bc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="787bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="787bc-106">Estado de gerenciamento do dispositivo no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="787bc-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="787bc-107">Membros</span><span class="sxs-lookup"><span data-stu-id="787bc-107">Members</span></span>
|<span data-ttu-id="787bc-108">Membro</span><span class="sxs-lookup"><span data-stu-id="787bc-108">Member</span></span>|<span data-ttu-id="787bc-109">Valor</span><span class="sxs-lookup"><span data-stu-id="787bc-109">Value</span></span>|<span data-ttu-id="787bc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="787bc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="787bc-111">Managed</span><span class="sxs-lookup"><span data-stu-id="787bc-111">managed</span></span>|<span data-ttu-id="787bc-112">,0</span><span class="sxs-lookup"><span data-stu-id="787bc-112">0</span></span>|<span data-ttu-id="787bc-113">O dispositivo está sob gerenciamento</span><span class="sxs-lookup"><span data-stu-id="787bc-113">The device is under management</span></span>|
|<span data-ttu-id="787bc-114">retirePending</span><span class="sxs-lookup"><span data-stu-id="787bc-114">retirePending</span></span>|<span data-ttu-id="787bc-115">1</span><span class="sxs-lookup"><span data-stu-id="787bc-115">1</span></span>|<span data-ttu-id="787bc-116">Um comando de desativação está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="787bc-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="787bc-117">retireFailed</span><span class="sxs-lookup"><span data-stu-id="787bc-117">retireFailed</span></span>|<span data-ttu-id="787bc-118">duas</span><span class="sxs-lookup"><span data-stu-id="787bc-118">2</span></span>|<span data-ttu-id="787bc-119">Falha no comando de desativação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="787bc-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="787bc-120">wipePending</span><span class="sxs-lookup"><span data-stu-id="787bc-120">wipePending</span></span>|<span data-ttu-id="787bc-121">3D</span><span class="sxs-lookup"><span data-stu-id="787bc-121">3</span></span>|<span data-ttu-id="787bc-122">Um comando de apagamento está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="787bc-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="787bc-123">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="787bc-123">wipeFailed</span></span>|<span data-ttu-id="787bc-124">quatro</span><span class="sxs-lookup"><span data-stu-id="787bc-124">4</span></span>|<span data-ttu-id="787bc-125">Falha no comando apagar no dispositivo</span><span class="sxs-lookup"><span data-stu-id="787bc-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="787bc-126">íntegro</span><span class="sxs-lookup"><span data-stu-id="787bc-126">unhealthy</span></span>|<span data-ttu-id="787bc-127">0,5</span><span class="sxs-lookup"><span data-stu-id="787bc-127">5</span></span>|<span data-ttu-id="787bc-128">O dispositivo não está íntegro.</span><span class="sxs-lookup"><span data-stu-id="787bc-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="787bc-129">deletePending</span><span class="sxs-lookup"><span data-stu-id="787bc-129">deletePending</span></span>|<span data-ttu-id="787bc-130">6</span><span class="sxs-lookup"><span data-stu-id="787bc-130">6</span></span>|<span data-ttu-id="787bc-131">Um comando delete está ocorrendo no dispositivo</span><span class="sxs-lookup"><span data-stu-id="787bc-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="787bc-132">retireIssued</span><span class="sxs-lookup"><span data-stu-id="787bc-132">retireIssued</span></span>|<span data-ttu-id="787bc-133">178</span><span class="sxs-lookup"><span data-stu-id="787bc-133">7</span></span>|<span data-ttu-id="787bc-134">Um comando de retirada foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="787bc-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="787bc-135">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="787bc-135">wipeIssued</span></span>|<span data-ttu-id="787bc-136">8 </span><span class="sxs-lookup"><span data-stu-id="787bc-136">8</span></span>|<span data-ttu-id="787bc-137">Um comando de apagamento foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="787bc-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="787bc-138">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="787bc-138">wipeCanceled</span></span>|<span data-ttu-id="787bc-139">9 </span><span class="sxs-lookup"><span data-stu-id="787bc-139">9</span></span>|<span data-ttu-id="787bc-140">Um comando de apagamento para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="787bc-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="787bc-141">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="787bc-141">retireCanceled</span></span>|<span data-ttu-id="787bc-142">10 </span><span class="sxs-lookup"><span data-stu-id="787bc-142">10</span></span>|<span data-ttu-id="787bc-143">Um comando de desativação para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="787bc-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="787bc-144">recém-descobertas</span><span class="sxs-lookup"><span data-stu-id="787bc-144">discovered</span></span>|<span data-ttu-id="787bc-145">11</span><span class="sxs-lookup"><span data-stu-id="787bc-145">11</span></span>|<span data-ttu-id="787bc-146">O dispositivo é descoberto, mas não está totalmente inscrito.</span><span class="sxs-lookup"><span data-stu-id="787bc-146">The device is discovered but not fully enrolled.</span></span>|



