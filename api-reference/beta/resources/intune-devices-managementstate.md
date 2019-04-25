---
title: tipo de enumeração ManagementState
description: Estado de gerenciamento do dispositivo no Microsoft Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05dc0db1ecbe88616ca36db82bad2081b4133e3f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521289"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="8b50b-103">tipo de enumeração ManagementState</span><span class="sxs-lookup"><span data-stu-id="8b50b-103">managementState enum type</span></span>

> <span data-ttu-id="8b50b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8b50b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b50b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8b50b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b50b-106">Estado de gerenciamento do dispositivo no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="8b50b-106">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="8b50b-107">Membros</span><span class="sxs-lookup"><span data-stu-id="8b50b-107">Members</span></span>
|<span data-ttu-id="8b50b-108">Membro</span><span class="sxs-lookup"><span data-stu-id="8b50b-108">Member</span></span>|<span data-ttu-id="8b50b-109">Valor</span><span class="sxs-lookup"><span data-stu-id="8b50b-109">Value</span></span>|<span data-ttu-id="8b50b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b50b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b50b-111">Managed</span><span class="sxs-lookup"><span data-stu-id="8b50b-111">managed</span></span>|<span data-ttu-id="8b50b-112">,0</span><span class="sxs-lookup"><span data-stu-id="8b50b-112">0</span></span>|<span data-ttu-id="8b50b-113">O dispositivo está sob gerenciamento</span><span class="sxs-lookup"><span data-stu-id="8b50b-113">The device is under management</span></span>|
|<span data-ttu-id="8b50b-114">retirePending</span><span class="sxs-lookup"><span data-stu-id="8b50b-114">retirePending</span></span>|<span data-ttu-id="8b50b-115">1 </span><span class="sxs-lookup"><span data-stu-id="8b50b-115">1</span></span>|<span data-ttu-id="8b50b-116">Um comando de desativação está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="8b50b-116">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="8b50b-117">retireFailed</span><span class="sxs-lookup"><span data-stu-id="8b50b-117">retireFailed</span></span>|<span data-ttu-id="8b50b-118">2 </span><span class="sxs-lookup"><span data-stu-id="8b50b-118">2</span></span>|<span data-ttu-id="8b50b-119">Falha no comando de desAtivação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="8b50b-119">Retire command failed on the device</span></span>|
|<span data-ttu-id="8b50b-120">wipePending</span><span class="sxs-lookup"><span data-stu-id="8b50b-120">wipePending</span></span>|<span data-ttu-id="8b50b-121">3 </span><span class="sxs-lookup"><span data-stu-id="8b50b-121">3</span></span>|<span data-ttu-id="8b50b-122">Um comando de apagamento está ocorrendo no dispositivo e no processo de cancelamento de registro de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="8b50b-122">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="8b50b-123">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="8b50b-123">wipeFailed</span></span>|<span data-ttu-id="8b50b-124">4 </span><span class="sxs-lookup"><span data-stu-id="8b50b-124">4</span></span>|<span data-ttu-id="8b50b-125">Falha no comando apagar no dispositivo</span><span class="sxs-lookup"><span data-stu-id="8b50b-125">Wipe command failed on the device</span></span>|
|<span data-ttu-id="8b50b-126">íntegro</span><span class="sxs-lookup"><span data-stu-id="8b50b-126">unhealthy</span></span>|<span data-ttu-id="8b50b-127">5 </span><span class="sxs-lookup"><span data-stu-id="8b50b-127">5</span></span>|<span data-ttu-id="8b50b-128">O dispositivo não está íntegro.</span><span class="sxs-lookup"><span data-stu-id="8b50b-128">The device is unhealthy.</span></span>|
|<span data-ttu-id="8b50b-129">deletePending</span><span class="sxs-lookup"><span data-stu-id="8b50b-129">deletePending</span></span>|<span data-ttu-id="8b50b-130">6 </span><span class="sxs-lookup"><span data-stu-id="8b50b-130">6</span></span>|<span data-ttu-id="8b50b-131">Um comando delete está ocorrendo no dispositivo</span><span class="sxs-lookup"><span data-stu-id="8b50b-131">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="8b50b-132">retireIssued</span><span class="sxs-lookup"><span data-stu-id="8b50b-132">retireIssued</span></span>|<span data-ttu-id="8b50b-133">7 </span><span class="sxs-lookup"><span data-stu-id="8b50b-133">7</span></span>|<span data-ttu-id="8b50b-134">Um comando de retirada foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="8b50b-134">A retire command was issued for the device</span></span>|
|<span data-ttu-id="8b50b-135">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="8b50b-135">wipeIssued</span></span>|<span data-ttu-id="8b50b-136">8 </span><span class="sxs-lookup"><span data-stu-id="8b50b-136">8</span></span>|<span data-ttu-id="8b50b-137">Um comando de apagamento foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="8b50b-137">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="8b50b-138">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="8b50b-138">wipeCanceled</span></span>|<span data-ttu-id="8b50b-139">9 </span><span class="sxs-lookup"><span data-stu-id="8b50b-139">9</span></span>|<span data-ttu-id="8b50b-140">Um comando de apagamento para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="8b50b-140">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="8b50b-141">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="8b50b-141">retireCanceled</span></span>|<span data-ttu-id="8b50b-142">10 </span><span class="sxs-lookup"><span data-stu-id="8b50b-142">10</span></span>|<span data-ttu-id="8b50b-143">Um comando de desativação para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="8b50b-143">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="8b50b-144">recém-descobertas</span><span class="sxs-lookup"><span data-stu-id="8b50b-144">discovered</span></span>|<span data-ttu-id="8b50b-145">11 </span><span class="sxs-lookup"><span data-stu-id="8b50b-145">11</span></span>|<span data-ttu-id="8b50b-146">O dispositivo é descoberto, mas não está totalmente inscrito.</span><span class="sxs-lookup"><span data-stu-id="8b50b-146">The device is discovered but not fully enrolled.</span></span>|





