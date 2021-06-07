---
title: Tipo de número deviceThreatProtectionLevel
description: Níveis de proteção contra ameaças de dispositivo para a API de Proteção contra Ameaças de Dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 21147e2be838bef34bc61eb401f57e1c650028d5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755088"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="1fcda-103">Tipo de número deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="1fcda-103">deviceThreatProtectionLevel enum type</span></span>

<span data-ttu-id="1fcda-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fcda-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1fcda-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1fcda-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fcda-106">Níveis de proteção contra ameaças de dispositivo para a API de Proteção contra Ameaças de Dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1fcda-106">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="1fcda-107">Membros</span><span class="sxs-lookup"><span data-stu-id="1fcda-107">Members</span></span>
|<span data-ttu-id="1fcda-108">Membro</span><span class="sxs-lookup"><span data-stu-id="1fcda-108">Member</span></span>|<span data-ttu-id="1fcda-109">Valor</span><span class="sxs-lookup"><span data-stu-id="1fcda-109">Value</span></span>|<span data-ttu-id="1fcda-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fcda-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fcda-111">unavailable</span><span class="sxs-lookup"><span data-stu-id="1fcda-111">unavailable</span></span>|<span data-ttu-id="1fcda-112">0</span><span class="sxs-lookup"><span data-stu-id="1fcda-112">0</span></span>|<span data-ttu-id="1fcda-113">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="1fcda-113">Default Value.</span></span> <span data-ttu-id="1fcda-114">Não usar.</span><span class="sxs-lookup"><span data-stu-id="1fcda-114">Do not use.</span></span>|
|<span data-ttu-id="1fcda-115">secured</span><span class="sxs-lookup"><span data-stu-id="1fcda-115">secured</span></span>|<span data-ttu-id="1fcda-116">1</span><span class="sxs-lookup"><span data-stu-id="1fcda-116">1</span></span>|<span data-ttu-id="1fcda-117">Requisito de Nível de Ameaça de Dispositivo: Protegido.</span><span class="sxs-lookup"><span data-stu-id="1fcda-117">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="1fcda-118">Esse é o nível mais seguro e representa que nenhuma ameaça foi encontrada no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1fcda-118">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="1fcda-119">low</span><span class="sxs-lookup"><span data-stu-id="1fcda-119">low</span></span>|<span data-ttu-id="1fcda-120">2</span><span class="sxs-lookup"><span data-stu-id="1fcda-120">2</span></span>|<span data-ttu-id="1fcda-121">Requisito de nível de Proteção contra Ameaças de Dispositivo: Baixo.</span><span class="sxs-lookup"><span data-stu-id="1fcda-121">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="1fcda-122">Baixo representa uma gravidade de ameaça que representa risco mínimo para os dados do dispositivo ou do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1fcda-122">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="1fcda-123">medium</span><span class="sxs-lookup"><span data-stu-id="1fcda-123">medium</span></span>|<span data-ttu-id="1fcda-124">3</span><span class="sxs-lookup"><span data-stu-id="1fcda-124">3</span></span>|<span data-ttu-id="1fcda-125">Requisito de nível de Proteção contra Ameaças de Dispositivo: Médio.</span><span class="sxs-lookup"><span data-stu-id="1fcda-125">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="1fcda-126">Médio representa uma gravidade de ameaça que representa um risco moderado para os dados do dispositivo ou do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1fcda-126">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="1fcda-127">high</span><span class="sxs-lookup"><span data-stu-id="1fcda-127">high</span></span>|<span data-ttu-id="1fcda-128">4 </span><span class="sxs-lookup"><span data-stu-id="1fcda-128">4</span></span>|<span data-ttu-id="1fcda-129">Requisito de nível de Proteção contra Ameaças de Dispositivo: Alto.</span><span class="sxs-lookup"><span data-stu-id="1fcda-129">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="1fcda-130">Alta representa uma gravidade de ameaça que representa um risco grave para os dados do dispositivo ou do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1fcda-130">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="1fcda-131">notSet</span><span class="sxs-lookup"><span data-stu-id="1fcda-131">notSet</span></span>|<span data-ttu-id="1fcda-132">10 </span><span class="sxs-lookup"><span data-stu-id="1fcda-132">10</span></span>|<span data-ttu-id="1fcda-133">Requisito de nível de Proteção contra Ameaças de Dispositivo: Não Definido.</span><span class="sxs-lookup"><span data-stu-id="1fcda-133">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="1fcda-134">Não definido representa que não há requisito para o dispositivo atender a um nível de Proteção contra Ameaças.</span><span class="sxs-lookup"><span data-stu-id="1fcda-134">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




