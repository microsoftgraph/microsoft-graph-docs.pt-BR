---
title: tipo de enum managementState
description: Estado de gerenciamento de dispositivo no Microsoft Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7d9d083c56df366b9f896432328d51c295f62190
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961943"
---
# <a name="managementstate-enum-type"></a><span data-ttu-id="0adad-103">tipo de enum managementState</span><span class="sxs-lookup"><span data-stu-id="0adad-103">managementState enum type</span></span>

> <span data-ttu-id="0adad-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0adad-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0adad-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0adad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0adad-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0adad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0adad-107">Estado de gerenciamento de dispositivo no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="0adad-107">Management state of device in Microsoft Intune.</span></span>
## <a name="members"></a><span data-ttu-id="0adad-108">Membros</span><span class="sxs-lookup"><span data-stu-id="0adad-108">Members</span></span>
|<span data-ttu-id="0adad-109">Membro</span><span class="sxs-lookup"><span data-stu-id="0adad-109">Member</span></span>|<span data-ttu-id="0adad-110">Valor</span><span class="sxs-lookup"><span data-stu-id="0adad-110">Value</span></span>|<span data-ttu-id="0adad-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0adad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0adad-112">gerenciados</span><span class="sxs-lookup"><span data-stu-id="0adad-112">managed</span></span>|<span data-ttu-id="0adad-113">0</span><span class="sxs-lookup"><span data-stu-id="0adad-113">0</span></span>|<span data-ttu-id="0adad-114">O dispositivo está sob gerenciamento</span><span class="sxs-lookup"><span data-stu-id="0adad-114">The device is under management</span></span>|
|<span data-ttu-id="0adad-115">retirePending</span><span class="sxs-lookup"><span data-stu-id="0adad-115">retirePending</span></span>|<span data-ttu-id="0adad-116">1</span><span class="sxs-lookup"><span data-stu-id="0adad-116">1</span></span>|<span data-ttu-id="0adad-117">Um comando de aposentadoria está ocorrendo no dispositivo e no processo de unenrolling de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="0adad-117">A retire command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="0adad-118">retireFailed</span><span class="sxs-lookup"><span data-stu-id="0adad-118">retireFailed</span></span>|<span data-ttu-id="0adad-119">2</span><span class="sxs-lookup"><span data-stu-id="0adad-119">2</span></span>|<span data-ttu-id="0adad-120">Desative o comando falha no dispositivo</span><span class="sxs-lookup"><span data-stu-id="0adad-120">Retire command failed on the device</span></span>|
|<span data-ttu-id="0adad-121">wipePending</span><span class="sxs-lookup"><span data-stu-id="0adad-121">wipePending</span></span>|<span data-ttu-id="0adad-122">3</span><span class="sxs-lookup"><span data-stu-id="0adad-122">3</span></span>|<span data-ttu-id="0adad-123">Um comando de apagamento está ocorrendo no dispositivo e no processo de unenrolling de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="0adad-123">A wipe command is occuring on the device and in the process of unenrolling from management</span></span>|
|<span data-ttu-id="0adad-124">wipeFailed</span><span class="sxs-lookup"><span data-stu-id="0adad-124">wipeFailed</span></span>|<span data-ttu-id="0adad-125">4</span><span class="sxs-lookup"><span data-stu-id="0adad-125">4</span></span>|<span data-ttu-id="0adad-126">Falha do comando de apagamento do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0adad-126">Wipe command failed on the device</span></span>|
|<span data-ttu-id="0adad-127">não íntegro</span><span class="sxs-lookup"><span data-stu-id="0adad-127">unhealthy</span></span>|<span data-ttu-id="0adad-128">5</span><span class="sxs-lookup"><span data-stu-id="0adad-128">5</span></span>|<span data-ttu-id="0adad-129">O dispositivo não está íntegro.</span><span class="sxs-lookup"><span data-stu-id="0adad-129">The device is unhealthy.</span></span>|
|<span data-ttu-id="0adad-130">deletePending</span><span class="sxs-lookup"><span data-stu-id="0adad-130">deletePending</span></span>|<span data-ttu-id="0adad-131">6</span><span class="sxs-lookup"><span data-stu-id="0adad-131">6</span></span>|<span data-ttu-id="0adad-132">Um comando Excluir está ocorrendo no dispositivo</span><span class="sxs-lookup"><span data-stu-id="0adad-132">A delete command is occuring on the device</span></span> |
|<span data-ttu-id="0adad-133">retireIssued</span><span class="sxs-lookup"><span data-stu-id="0adad-133">retireIssued</span></span>|<span data-ttu-id="0adad-134">7</span><span class="sxs-lookup"><span data-stu-id="0adad-134">7</span></span>|<span data-ttu-id="0adad-135">Um comando de aposentadoria foi emitido para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="0adad-135">A retire command was issued for the device</span></span>|
|<span data-ttu-id="0adad-136">wipeIssued</span><span class="sxs-lookup"><span data-stu-id="0adad-136">wipeIssued</span></span>|<span data-ttu-id="0adad-137">8</span><span class="sxs-lookup"><span data-stu-id="0adad-137">8</span></span>|<span data-ttu-id="0adad-138">Foi emitido um comando de apagamento do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0adad-138">A wipe command was issued for the device</span></span>|
|<span data-ttu-id="0adad-139">wipeCanceled</span><span class="sxs-lookup"><span data-stu-id="0adad-139">wipeCanceled</span></span>|<span data-ttu-id="0adad-140">9</span><span class="sxs-lookup"><span data-stu-id="0adad-140">9</span></span>|<span data-ttu-id="0adad-141">Um comando de apagamento para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="0adad-141">A wipe command for this device has been canceled</span></span>|
|<span data-ttu-id="0adad-142">retireCanceled</span><span class="sxs-lookup"><span data-stu-id="0adad-142">retireCanceled</span></span>|<span data-ttu-id="0adad-143">10</span><span class="sxs-lookup"><span data-stu-id="0adad-143">10</span></span>|<span data-ttu-id="0adad-144">Um comando de aposentadoria para este dispositivo foi cancelado</span><span class="sxs-lookup"><span data-stu-id="0adad-144">A retire command for this device has been canceled</span></span>|
|<span data-ttu-id="0adad-145">descoberto</span><span class="sxs-lookup"><span data-stu-id="0adad-145">discovered</span></span>|<span data-ttu-id="0adad-146">11</span><span class="sxs-lookup"><span data-stu-id="0adad-146">11</span></span>|<span data-ttu-id="0adad-147">O dispositivo é descoberto, mas não totalmente registrado.</span><span class="sxs-lookup"><span data-stu-id="0adad-147">The device is discovered but not fully enrolled.</span></span>|





