---
title: tipo de enum managementState
description: Estado de gerenciamento de dispositivo no Microsoft Intune.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8d0801949125f3b0cceb865ac1f8546195112e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420014"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="40bec-103">tipo de enum managementState</span><span class="sxs-lookup"><span data-stu-id="40bec-103">managementState enum type</span></span>

> <span data-ttu-id="40bec-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="40bec-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="40bec-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="40bec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40bec-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="40bec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40bec-107">Estado de gerenciamento de dispositivo no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="40bec-107">Management state of device in Microsoft Intune.</span></span>

## <a name="members"></a><span data-ttu-id="40bec-108">Membros</span><span class="sxs-lookup"><span data-stu-id="40bec-108">Members</span></span>
|<span data-ttu-id="40bec-109">Membro</span><span class="sxs-lookup"><span data-stu-id="40bec-109">Member</span></span>|<span data-ttu-id="40bec-110">Valor</span><span class="sxs-lookup"><span data-stu-id="40bec-110">Value</span></span>|<span data-ttu-id="40bec-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="40bec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40bec-112">gerenciados</span><span class="sxs-lookup"><span data-stu-id="40bec-112">managed</span></span>|<span data-ttu-id="40bec-113">0</span><span class="sxs-lookup"><span data-stu-id="40bec-113">0</span></span>|<span data-ttu-id="40bec-114">O dispositivo está sob gerenciamento</span><span class="sxs-lookup"><span data-stu-id="40bec-114">The device is under management</span></span>|
|<span data-ttu-id="40bec-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="40bec-115">retirePending</span></span>|<span data-ttu-id="40bec-116">1</span><span class="sxs-lookup"><span data-stu-id="40bec-116">1</span></span>|<span data-ttu-id="40bec-117">Um comando de aposentadoria está ocorrendo no dispositivo e no processo de unenrolling de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="40bec-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="40bec-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="40bec-118">retireFailed</span></span>|<span data-ttu-id="40bec-119">2</span><span class="sxs-lookup"><span data-stu-id="40bec-119">2</span></span>|<span data-ttu-id="40bec-120">Desative o comando falha no dispositivo</span><span class="sxs-lookup"><span data-stu-id="40bec-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="40bec-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="40bec-121">wipePending</span></span>|<span data-ttu-id="40bec-122">3</span><span class="sxs-lookup"><span data-stu-id="40bec-122">3</span></span>|<span data-ttu-id="40bec-123">Um comando de apagamento está ocorrendo no dispositivo e no processo de unenrolling de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="40bec-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="40bec-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="40bec-124">wipeFailed</span></span>|<span data-ttu-id="40bec-125">4</span><span class="sxs-lookup"><span data-stu-id="40bec-125">4</span></span>|<span data-ttu-id="40bec-126">Falha do comando de apagamento do dispositivo</span><span class="sxs-lookup"><span data-stu-id="40bec-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="40bec-127">não íntegro</span><span class="sxs-lookup"><span data-stu-id="40bec-127">unhealthy</span></span>|<span data-ttu-id="40bec-128">5</span><span class="sxs-lookup"><span data-stu-id="40bec-128">5</span></span>|<span data-ttu-id="40bec-129">O dispositivo não está íntegro.</span><span class="sxs-lookup"><span data-stu-id="40bec-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="40bec-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="40bec-130">deletePending</span></span>|<span data-ttu-id="40bec-131">6</span><span class="sxs-lookup"><span data-stu-id="40bec-131">6</span></span>|<span data-ttu-id="40bec-132">Um comando Excluir está ocorrendo no dispositivo</span><span class="sxs-lookup"><span data-stu-id="40bec-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="40bec-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="40bec-133">retireIssued</span></span>|<span data-ttu-id="40bec-134">7</span><span class="sxs-lookup"><span data-stu-id="40bec-134">7</span></span>|<span data-ttu-id="40bec-135">Um comando de aposentadoria foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="40bec-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="40bec-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="40bec-136">wipeIssued</span></span>|<span data-ttu-id="40bec-137">8</span><span class="sxs-lookup"><span data-stu-id="40bec-137">8</span></span>|<span data-ttu-id="40bec-138">Foi emitido um comando de apagamento do dispositivo</span><span class="sxs-lookup"><span data-stu-id="40bec-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="40bec-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="40bec-139">wipeCanceled</span></span>|<span data-ttu-id="40bec-140">9</span><span class="sxs-lookup"><span data-stu-id="40bec-140">9</span></span>|<span data-ttu-id="40bec-141">Um comando de apagamento para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="40bec-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="40bec-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="40bec-142">retireCanceled</span></span>|<span data-ttu-id="40bec-143">10</span><span class="sxs-lookup"><span data-stu-id="40bec-143">10</span></span>|<span data-ttu-id="40bec-144">Um comando de aposentadoria para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="40bec-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="40bec-145">descoberto</span><span class="sxs-lookup"><span data-stu-id="40bec-145">discovered</span></span>|<span data-ttu-id="40bec-146">11</span><span class="sxs-lookup"><span data-stu-id="40bec-146">11</span></span>|<span data-ttu-id="40bec-147">O dispositivo é descoberto, mas não totalmente registrado.</span><span class="sxs-lookup"><span data-stu-id="40bec-147">The device is discovered but not fully enrolled.</span></span>|




