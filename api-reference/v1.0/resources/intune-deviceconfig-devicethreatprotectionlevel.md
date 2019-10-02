---
title: tipo de enumeração deviceThreatProtectionLevel
description: Níveis de proteção contra ameaças de dispositivos para a API de proteção contra ameaças de dispositivos.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e64bc6465e190e4e5da3629b6d638dc82813a2bb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359380"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="95c30-103">tipo de enumeração deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="95c30-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="95c30-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95c30-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95c30-105">Níveis de proteção contra ameaças de dispositivos para a API de proteção contra ameaças de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="95c30-105">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="95c30-106">Membros</span><span class="sxs-lookup"><span data-stu-id="95c30-106">Members</span></span>
|<span data-ttu-id="95c30-107">Membro</span><span class="sxs-lookup"><span data-stu-id="95c30-107">Member</span></span>|<span data-ttu-id="95c30-108">Valor</span><span class="sxs-lookup"><span data-stu-id="95c30-108">Value</span></span>|<span data-ttu-id="95c30-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="95c30-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95c30-110">indisponível</span><span class="sxs-lookup"><span data-stu-id="95c30-110">unavailable</span></span>|<span data-ttu-id="95c30-111">,0</span><span class="sxs-lookup"><span data-stu-id="95c30-111">0</span></span>|<span data-ttu-id="95c30-112">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="95c30-112">Default Value.</span></span> <span data-ttu-id="95c30-113">Não usar.</span><span class="sxs-lookup"><span data-stu-id="95c30-113">Do not use.</span></span>|
|<span data-ttu-id="95c30-114">presos</span><span class="sxs-lookup"><span data-stu-id="95c30-114">secured</span></span>|<span data-ttu-id="95c30-115">1</span><span class="sxs-lookup"><span data-stu-id="95c30-115">1</span></span>|<span data-ttu-id="95c30-116">Requisito de nível de ameaça de dispositivo: protegido.</span><span class="sxs-lookup"><span data-stu-id="95c30-116">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="95c30-117">Este é o nível mais seguro e representa que nenhuma ameaça foi encontrada no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95c30-117">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="95c30-118">low</span><span class="sxs-lookup"><span data-stu-id="95c30-118">low</span></span>|<span data-ttu-id="95c30-119">duas</span><span class="sxs-lookup"><span data-stu-id="95c30-119">2</span></span>|<span data-ttu-id="95c30-120">Requisito de nível de proteção contra ameaças de dispositivos: baixo.</span><span class="sxs-lookup"><span data-stu-id="95c30-120">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="95c30-121">Low representa uma severidade de ameaça que representa o risco mínimo para os dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95c30-121">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="95c30-122">medium</span><span class="sxs-lookup"><span data-stu-id="95c30-122">medium</span></span>|<span data-ttu-id="95c30-123">3D</span><span class="sxs-lookup"><span data-stu-id="95c30-123">3</span></span>|<span data-ttu-id="95c30-124">Requisito de nível de proteção contra ameaças de dispositivos: médio.</span><span class="sxs-lookup"><span data-stu-id="95c30-124">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="95c30-125">Médio representa uma severidade de ameaça que representa o risco moderado para os dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95c30-125">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="95c30-126">high</span><span class="sxs-lookup"><span data-stu-id="95c30-126">high</span></span>|<span data-ttu-id="95c30-127">quatro</span><span class="sxs-lookup"><span data-stu-id="95c30-127">4</span></span>|<span data-ttu-id="95c30-128">Requisito de nível de proteção contra ameaças de dispositivos: alto.</span><span class="sxs-lookup"><span data-stu-id="95c30-128">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="95c30-129">High representa uma severidade de ameaça que representa sérios riscos nos dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95c30-129">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="95c30-130">notSet</span><span class="sxs-lookup"><span data-stu-id="95c30-130">notSet</span></span>|<span data-ttu-id="95c30-131">10 </span><span class="sxs-lookup"><span data-stu-id="95c30-131">10</span></span>|<span data-ttu-id="95c30-132">Requisito de nível de proteção contra ameaças de dispositivos: não definido.</span><span class="sxs-lookup"><span data-stu-id="95c30-132">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="95c30-133">Not set indica que não há necessidade de o dispositivo atender a um nível de proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="95c30-133">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




