---
title: tipo de enumeração ManagementState
description: Estado de gerenciamento do dispositivo no Microsoft Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a53b07f89ee551d3e559a42bbe23c5fba808f20
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174141"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="d3128-103">tipo de enumeração ManagementState</span><span class="sxs-lookup"><span data-stu-id="d3128-103">managementState enum type</span></span>

> <span data-ttu-id="d3128-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3128-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3128-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3128-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3128-106">Estado de gerenciamento do dispositivo no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="d3128-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="d3128-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d3128-107">Members</span></span>
|<span data-ttu-id="d3128-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d3128-108">Member</span></span>|<span data-ttu-id="d3128-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d3128-109">Value</span></span>|<span data-ttu-id="d3128-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3128-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3128-111">Managed</span><span class="sxs-lookup"><span data-stu-id="d3128-111">managed</span></span>|<span data-ttu-id="d3128-112">,0</span><span class="sxs-lookup"><span data-stu-id="d3128-112">0</span></span>|<span data-ttu-id="d3128-113">O dispositivo está sob gerenciamento</span><span class="sxs-lookup"><span data-stu-id="d3128-113">The device is under management</span></span>|
|<span data-ttu-id="d3128-114">retirePending</span><span class="sxs-lookup"><span data-stu-id="d3128-114">retirePending</span></span>|<span data-ttu-id="d3128-115">1</span><span class="sxs-lookup"><span data-stu-id="d3128-115">1</span></span>|<span data-ttu-id="d3128-116">Um comando de desativação está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="d3128-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="d3128-117">retireFailed</span><span class="sxs-lookup"><span data-stu-id="d3128-117">retireFailed</span></span>|<span data-ttu-id="d3128-118">duas</span><span class="sxs-lookup"><span data-stu-id="d3128-118">2</span></span>|<span data-ttu-id="d3128-119">Falha no comando de desAtivação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="d3128-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="d3128-120">wipePending</span><span class="sxs-lookup"><span data-stu-id="d3128-120">wipePending</span></span>|<span data-ttu-id="d3128-121">3D</span><span class="sxs-lookup"><span data-stu-id="d3128-121">3</span></span>|<span data-ttu-id="d3128-122">Um comando de apagamento está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="d3128-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="d3128-123">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="d3128-123">wipeFailed</span></span>|<span data-ttu-id="d3128-124">quatro</span><span class="sxs-lookup"><span data-stu-id="d3128-124">4</span></span>|<span data-ttu-id="d3128-125">Falha no comando apagar no dispositivo</span><span class="sxs-lookup"><span data-stu-id="d3128-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="d3128-126">íntegro</span><span class="sxs-lookup"><span data-stu-id="d3128-126">unhealthy</span></span>|<span data-ttu-id="d3128-127">0,5</span><span class="sxs-lookup"><span data-stu-id="d3128-127">5</span></span>|<span data-ttu-id="d3128-128">O dispositivo não está íntegro.</span><span class="sxs-lookup"><span data-stu-id="d3128-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="d3128-129">deletePending</span><span class="sxs-lookup"><span data-stu-id="d3128-129">deletePending</span></span>|<span data-ttu-id="d3128-130">6</span><span class="sxs-lookup"><span data-stu-id="d3128-130">6</span></span>|<span data-ttu-id="d3128-131">Um comando delete está ocorrendo no dispositivo</span><span class="sxs-lookup"><span data-stu-id="d3128-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="d3128-132">retireIssued</span><span class="sxs-lookup"><span data-stu-id="d3128-132">retireIssued</span></span>|<span data-ttu-id="d3128-133">178</span><span class="sxs-lookup"><span data-stu-id="d3128-133">7</span></span>|<span data-ttu-id="d3128-134">Um comando de retirada foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="d3128-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="d3128-135">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="d3128-135">wipeIssued</span></span>|<span data-ttu-id="d3128-136">8</span><span class="sxs-lookup"><span data-stu-id="d3128-136">8</span></span>|<span data-ttu-id="d3128-137">Um comando de apagamento foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="d3128-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="d3128-138">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="d3128-138">wipeCanceled</span></span>|<span data-ttu-id="d3128-139">241</span><span class="sxs-lookup"><span data-stu-id="d3128-139">9</span></span>|<span data-ttu-id="d3128-140">Um comando de apagamento para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="d3128-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="d3128-141">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="d3128-141">retireCanceled</span></span>|<span data-ttu-id="d3128-142">254</span><span class="sxs-lookup"><span data-stu-id="d3128-142">10</span></span>|<span data-ttu-id="d3128-143">Um comando de desativação para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="d3128-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="d3128-144">recém-descobertas</span><span class="sxs-lookup"><span data-stu-id="d3128-144">discovered</span></span>|<span data-ttu-id="d3128-145">11</span><span class="sxs-lookup"><span data-stu-id="d3128-145">11</span></span>|<span data-ttu-id="d3128-146">O dispositivo é descoberto, mas não está totalmente inscrito.</span><span class="sxs-lookup"><span data-stu-id="d3128-146">The device is discovered but not fully enrolled.</span></span>|




