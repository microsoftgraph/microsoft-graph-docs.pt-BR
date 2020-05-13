---
title: tipo de enumeração deviceThreatProtectionLevel
description: Níveis de proteção contra ameaças de dispositivos para a API de proteção contra ameaças de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b78118e624898c90e3bd2e0e4c281bf0a0a4ca41
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43469221"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="37b0a-103">tipo de enumeração deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="37b0a-103">deviceThreatProtectionLevel enum type</span></span>

<span data-ttu-id="37b0a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37b0a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37b0a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37b0a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37b0a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37b0a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37b0a-107">Níveis de proteção contra ameaças de dispositivos para a API de proteção contra ameaças de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="37b0a-107">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="37b0a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="37b0a-108">Members</span></span>
|<span data-ttu-id="37b0a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="37b0a-109">Member</span></span>|<span data-ttu-id="37b0a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="37b0a-110">Value</span></span>|<span data-ttu-id="37b0a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="37b0a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37b0a-112">indisponível</span><span class="sxs-lookup"><span data-stu-id="37b0a-112">unavailable</span></span>|<span data-ttu-id="37b0a-113">,0</span><span class="sxs-lookup"><span data-stu-id="37b0a-113">0</span></span>|<span data-ttu-id="37b0a-114">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="37b0a-114">Default Value.</span></span> <span data-ttu-id="37b0a-115">Não usar.</span><span class="sxs-lookup"><span data-stu-id="37b0a-115">Do not use.</span></span>|
|<span data-ttu-id="37b0a-116">presos</span><span class="sxs-lookup"><span data-stu-id="37b0a-116">secured</span></span>|<span data-ttu-id="37b0a-117">1 </span><span class="sxs-lookup"><span data-stu-id="37b0a-117">1</span></span>|<span data-ttu-id="37b0a-118">Requisito de nível de ameaça de dispositivo: protegido.</span><span class="sxs-lookup"><span data-stu-id="37b0a-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="37b0a-119">Este é o nível mais seguro e representa que nenhuma ameaça foi encontrada no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37b0a-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="37b0a-120">low</span><span class="sxs-lookup"><span data-stu-id="37b0a-120">low</span></span>|<span data-ttu-id="37b0a-121">2 </span><span class="sxs-lookup"><span data-stu-id="37b0a-121">2</span></span>|<span data-ttu-id="37b0a-122">Requisito de nível de proteção contra ameaças de dispositivos: baixo.</span><span class="sxs-lookup"><span data-stu-id="37b0a-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="37b0a-123">Low representa uma severidade de ameaça que representa o risco mínimo para os dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37b0a-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="37b0a-124">medium</span><span class="sxs-lookup"><span data-stu-id="37b0a-124">medium</span></span>|<span data-ttu-id="37b0a-125">3 </span><span class="sxs-lookup"><span data-stu-id="37b0a-125">3</span></span>|<span data-ttu-id="37b0a-126">Requisito de nível de proteção contra ameaças de dispositivos: médio.</span><span class="sxs-lookup"><span data-stu-id="37b0a-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="37b0a-127">Médio representa uma severidade de ameaça que representa o risco moderado para os dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37b0a-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="37b0a-128">high</span><span class="sxs-lookup"><span data-stu-id="37b0a-128">high</span></span>|<span data-ttu-id="37b0a-129">4 </span><span class="sxs-lookup"><span data-stu-id="37b0a-129">4</span></span>|<span data-ttu-id="37b0a-130">Requisito de nível de proteção contra ameaças de dispositivos: alto.</span><span class="sxs-lookup"><span data-stu-id="37b0a-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="37b0a-131">High representa uma severidade de ameaça que representa sérios riscos nos dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37b0a-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="37b0a-132">notSet</span><span class="sxs-lookup"><span data-stu-id="37b0a-132">notSet</span></span>|<span data-ttu-id="37b0a-133">10 </span><span class="sxs-lookup"><span data-stu-id="37b0a-133">10</span></span>|<span data-ttu-id="37b0a-134">Requisito de nível de proteção contra ameaças de dispositivos: não definido.</span><span class="sxs-lookup"><span data-stu-id="37b0a-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="37b0a-135">Not set indica que não há necessidade de o dispositivo atender a um nível de proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="37b0a-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|



