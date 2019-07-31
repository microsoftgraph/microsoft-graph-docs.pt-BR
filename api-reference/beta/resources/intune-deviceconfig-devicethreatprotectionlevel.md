---
title: tipo de enumeração deviceThreatProtectionLevel
description: Níveis de proteção contra ameaças de dispositivos para a API de proteção contra ameaças de dispositivos.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 46af5513a1f88de1e055b6b9697625e7e6652782
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004530"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="7cda6-103">tipo de enumeração deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="7cda6-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="7cda6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7cda6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7cda6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7cda6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cda6-106">Níveis de proteção contra ameaças de dispositivos para a API de proteção contra ameaças de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="7cda6-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="7cda6-107">Membros</span><span class="sxs-lookup"><span data-stu-id="7cda6-107">Members</span></span>
|<span data-ttu-id="7cda6-108">Membro</span><span class="sxs-lookup"><span data-stu-id="7cda6-108">Member</span></span>|<span data-ttu-id="7cda6-109">Valor</span><span class="sxs-lookup"><span data-stu-id="7cda6-109">Value</span></span>|<span data-ttu-id="7cda6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cda6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cda6-111">indisponível</span><span class="sxs-lookup"><span data-stu-id="7cda6-111">unavailable</span></span>|<span data-ttu-id="7cda6-112">,0</span><span class="sxs-lookup"><span data-stu-id="7cda6-112">0</span></span>|<span data-ttu-id="7cda6-113">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="7cda6-113">Default Value.</span></span> <span data-ttu-id="7cda6-114">Não usar.</span><span class="sxs-lookup"><span data-stu-id="7cda6-114">Do not use.</span></span>|
|<span data-ttu-id="7cda6-115">presos</span><span class="sxs-lookup"><span data-stu-id="7cda6-115">secured</span></span>|<span data-ttu-id="7cda6-116">1</span><span class="sxs-lookup"><span data-stu-id="7cda6-116">1</span></span>|<span data-ttu-id="7cda6-117">Requisito de nível de ameaça de dispositivo: protegido.</span><span class="sxs-lookup"><span data-stu-id="7cda6-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="7cda6-118">Este é o nível mais seguro e representa que nenhuma ameaça foi encontrada no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7cda6-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="7cda6-119">low</span><span class="sxs-lookup"><span data-stu-id="7cda6-119">low</span></span>|<span data-ttu-id="7cda6-120">duas</span><span class="sxs-lookup"><span data-stu-id="7cda6-120">2</span></span>|<span data-ttu-id="7cda6-121">Requisito de nível de proteção contra ameaças de dispositivos: baixo.</span><span class="sxs-lookup"><span data-stu-id="7cda6-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="7cda6-122">Low representa uma severidade de ameaça que representa o risco mínimo para os dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7cda6-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="7cda6-123">medium</span><span class="sxs-lookup"><span data-stu-id="7cda6-123">medium</span></span>|<span data-ttu-id="7cda6-124">3D</span><span class="sxs-lookup"><span data-stu-id="7cda6-124">3</span></span>|<span data-ttu-id="7cda6-125">Requisito de nível de proteção contra ameaças de dispositivos: médio.</span><span class="sxs-lookup"><span data-stu-id="7cda6-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="7cda6-126">Médio representa uma severidade de ameaça que representa o risco moderado para os dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7cda6-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="7cda6-127">high</span><span class="sxs-lookup"><span data-stu-id="7cda6-127">high</span></span>|<span data-ttu-id="7cda6-128">quatro</span><span class="sxs-lookup"><span data-stu-id="7cda6-128">4</span></span>|<span data-ttu-id="7cda6-129">Requisito de nível de proteção contra ameaças de dispositivos: alto.</span><span class="sxs-lookup"><span data-stu-id="7cda6-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="7cda6-130">High representa uma severidade de ameaça que representa sérios riscos nos dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7cda6-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="7cda6-131">notSet</span><span class="sxs-lookup"><span data-stu-id="7cda6-131">notSet</span></span>|<span data-ttu-id="7cda6-132">10 </span><span class="sxs-lookup"><span data-stu-id="7cda6-132">10</span></span>|<span data-ttu-id="7cda6-133">Requisito de nível de proteção contra ameaças de dispositivos: não definido.</span><span class="sxs-lookup"><span data-stu-id="7cda6-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="7cda6-134">Not set indica que não há necessidade de o dispositivo atender a um nível de proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="7cda6-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|





