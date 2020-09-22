---
title: tipo de enumeração deviceThreatProtectionLevel
description: Níveis de proteção contra ameaças de dispositivos para a API de proteção contra ameaças de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e6169a6f7816a04b0e3a81065fc78869eadc3b7e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040025"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="a39c2-103">tipo de enumeração deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="a39c2-103">deviceThreatProtectionLevel enum type</span></span>

<span data-ttu-id="a39c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a39c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a39c2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a39c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a39c2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a39c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a39c2-107">Níveis de proteção contra ameaças de dispositivos para a API de proteção contra ameaças de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a39c2-107">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="a39c2-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a39c2-108">Members</span></span>
|<span data-ttu-id="a39c2-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a39c2-109">Member</span></span>|<span data-ttu-id="a39c2-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a39c2-110">Value</span></span>|<span data-ttu-id="a39c2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a39c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a39c2-112">indisponível</span><span class="sxs-lookup"><span data-stu-id="a39c2-112">unavailable</span></span>|<span data-ttu-id="a39c2-113">,0</span><span class="sxs-lookup"><span data-stu-id="a39c2-113">0</span></span>|<span data-ttu-id="a39c2-114">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="a39c2-114">Default Value.</span></span> <span data-ttu-id="a39c2-115">Não usar.</span><span class="sxs-lookup"><span data-stu-id="a39c2-115">Do not use.</span></span>|
|<span data-ttu-id="a39c2-116">presos</span><span class="sxs-lookup"><span data-stu-id="a39c2-116">secured</span></span>|<span data-ttu-id="a39c2-117">1 </span><span class="sxs-lookup"><span data-stu-id="a39c2-117">1</span></span>|<span data-ttu-id="a39c2-118">Requisito de nível de ameaça de dispositivo: protegido.</span><span class="sxs-lookup"><span data-stu-id="a39c2-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="a39c2-119">Este é o nível mais seguro e representa que nenhuma ameaça foi encontrada no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a39c2-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="a39c2-120">low</span><span class="sxs-lookup"><span data-stu-id="a39c2-120">low</span></span>|<span data-ttu-id="a39c2-121">2 </span><span class="sxs-lookup"><span data-stu-id="a39c2-121">2</span></span>|<span data-ttu-id="a39c2-122">Requisito de nível de proteção contra ameaças de dispositivos: baixo.</span><span class="sxs-lookup"><span data-stu-id="a39c2-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="a39c2-123">Low representa uma severidade de ameaça que representa o risco mínimo para os dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a39c2-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="a39c2-124">medium</span><span class="sxs-lookup"><span data-stu-id="a39c2-124">medium</span></span>|<span data-ttu-id="a39c2-125">3 </span><span class="sxs-lookup"><span data-stu-id="a39c2-125">3</span></span>|<span data-ttu-id="a39c2-126">Requisito de nível de proteção contra ameaças de dispositivos: médio.</span><span class="sxs-lookup"><span data-stu-id="a39c2-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="a39c2-127">Médio representa uma severidade de ameaça que representa o risco moderado para os dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a39c2-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="a39c2-128">high</span><span class="sxs-lookup"><span data-stu-id="a39c2-128">high</span></span>|<span data-ttu-id="a39c2-129">4 </span><span class="sxs-lookup"><span data-stu-id="a39c2-129">4</span></span>|<span data-ttu-id="a39c2-130">Requisito de nível de proteção contra ameaças de dispositivos: alto.</span><span class="sxs-lookup"><span data-stu-id="a39c2-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="a39c2-131">High representa uma severidade de ameaça que representa sérios riscos nos dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a39c2-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="a39c2-132">notSet</span><span class="sxs-lookup"><span data-stu-id="a39c2-132">notSet</span></span>|<span data-ttu-id="a39c2-133">10 </span><span class="sxs-lookup"><span data-stu-id="a39c2-133">10</span></span>|<span data-ttu-id="a39c2-134">Requisito de nível de proteção contra ameaças de dispositivos: não definido.</span><span class="sxs-lookup"><span data-stu-id="a39c2-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="a39c2-135">Not set indica que não há necessidade de o dispositivo atender a um nível de proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="a39c2-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|






