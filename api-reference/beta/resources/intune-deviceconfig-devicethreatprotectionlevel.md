---
title: tipo de enumeração deviceThreatProtectionLevel
description: Níveis de proteção contra ameaças de dispositivos para a API de proteção contra ameaças de dispositivos.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ecdf54051b1545b842cbc3c49359b9a77f12e2e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140240"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="02ff7-103">tipo de enumeração deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="02ff7-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="02ff7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02ff7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02ff7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02ff7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02ff7-106">Níveis de proteção contra ameaças de dispositivos para a API de proteção contra ameaças de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="02ff7-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="02ff7-107">Membros</span><span class="sxs-lookup"><span data-stu-id="02ff7-107">Members</span></span>
|<span data-ttu-id="02ff7-108">Membro</span><span class="sxs-lookup"><span data-stu-id="02ff7-108">Member</span></span>|<span data-ttu-id="02ff7-109">Valor</span><span class="sxs-lookup"><span data-stu-id="02ff7-109">Value</span></span>|<span data-ttu-id="02ff7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="02ff7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02ff7-111">indisponível</span><span class="sxs-lookup"><span data-stu-id="02ff7-111">unavailable</span></span>|<span data-ttu-id="02ff7-112">,0</span><span class="sxs-lookup"><span data-stu-id="02ff7-112">0</span></span>|<span data-ttu-id="02ff7-113">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="02ff7-113">Default Value.</span></span> <span data-ttu-id="02ff7-114">Não a use.</span><span class="sxs-lookup"><span data-stu-id="02ff7-114">Do not use.</span></span>|
|<span data-ttu-id="02ff7-115">presos</span><span class="sxs-lookup"><span data-stu-id="02ff7-115">secured</span></span>|<span data-ttu-id="02ff7-116">1</span><span class="sxs-lookup"><span data-stu-id="02ff7-116">1</span></span>|<span data-ttu-id="02ff7-117">Requisito de nível de ameaça de dispositivo: protegido.</span><span class="sxs-lookup"><span data-stu-id="02ff7-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="02ff7-118">Este é o nível mais seguro e representa que nenhuma ameaça foi encontrada no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02ff7-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="02ff7-119">low</span><span class="sxs-lookup"><span data-stu-id="02ff7-119">low</span></span>|<span data-ttu-id="02ff7-120">duas</span><span class="sxs-lookup"><span data-stu-id="02ff7-120">2</span></span>|<span data-ttu-id="02ff7-121">Requisito de nível de proteção contra ameaças de dispositivos: baixo.</span><span class="sxs-lookup"><span data-stu-id="02ff7-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="02ff7-122">Low representa uma severidade de ameaça que representa o risco mínimo para os dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02ff7-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="02ff7-123">medium</span><span class="sxs-lookup"><span data-stu-id="02ff7-123">medium</span></span>|<span data-ttu-id="02ff7-124">3D</span><span class="sxs-lookup"><span data-stu-id="02ff7-124">3</span></span>|<span data-ttu-id="02ff7-125">Requisito de nível de proteção contra ameaças de dispositivos: médio.</span><span class="sxs-lookup"><span data-stu-id="02ff7-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="02ff7-126">Médio representa uma severidade de ameaça que representa o risco moderado para os dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02ff7-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="02ff7-127">high</span><span class="sxs-lookup"><span data-stu-id="02ff7-127">high</span></span>|<span data-ttu-id="02ff7-128">quatro</span><span class="sxs-lookup"><span data-stu-id="02ff7-128">4</span></span>|<span data-ttu-id="02ff7-129">Requisito de nível de proteção contra ameaças de dispositivos: alto.</span><span class="sxs-lookup"><span data-stu-id="02ff7-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="02ff7-130">High representa uma severidade de ameaça que representa sérios riscos nos dados do dispositivo ou dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02ff7-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="02ff7-131">notSet</span><span class="sxs-lookup"><span data-stu-id="02ff7-131">notSet</span></span>|<span data-ttu-id="02ff7-132">254</span><span class="sxs-lookup"><span data-stu-id="02ff7-132">10</span></span>|<span data-ttu-id="02ff7-133">Requisito de nível de proteção contra ameaças de dispositivos: não definido.</span><span class="sxs-lookup"><span data-stu-id="02ff7-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="02ff7-134">Not set indica que não há necessidade de o dispositivo atender a um nível de proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="02ff7-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




