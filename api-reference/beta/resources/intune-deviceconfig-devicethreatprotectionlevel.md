---
title: tipo de enum deviceThreatProtectionLevel
description: Níveis de proteção de ameaça de dispositivo para a API de proteção de ameaça do dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a4c9bbc599d424b91d07339a7a7cdad90b84c262
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411229"
---
# <a name="devicethreatprotectionlevel-enum-type"></a><span data-ttu-id="4d34b-103">tipo de enum deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="4d34b-103">deviceThreatProtectionLevel enum type</span></span>

> <span data-ttu-id="4d34b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4d34b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4d34b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4d34b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d34b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4d34b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d34b-107">Níveis de proteção de ameaça de dispositivo para a API de proteção de ameaça do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d34b-107">Device threat protection levels for the Device Threat Protection API.</span></span>

## <a name="members"></a><span data-ttu-id="4d34b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4d34b-108">Members</span></span>
|<span data-ttu-id="4d34b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4d34b-109">Member</span></span>|<span data-ttu-id="4d34b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4d34b-110">Value</span></span>|<span data-ttu-id="4d34b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d34b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d34b-112">indisponível</span><span class="sxs-lookup"><span data-stu-id="4d34b-112">unavailable</span></span>|<span data-ttu-id="4d34b-113">0</span><span class="sxs-lookup"><span data-stu-id="4d34b-113">0</span></span>|<span data-ttu-id="4d34b-114">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="4d34b-114">Default Value.</span></span> <span data-ttu-id="4d34b-115">Não a use.</span><span class="sxs-lookup"><span data-stu-id="4d34b-115">Do not use.</span></span>|
|<span data-ttu-id="4d34b-116">protegido</span><span class="sxs-lookup"><span data-stu-id="4d34b-116">secured</span></span>|<span data-ttu-id="4d34b-117">1</span><span class="sxs-lookup"><span data-stu-id="4d34b-117">1</span></span>|<span data-ttu-id="4d34b-118">Requisito de dispositivo de nível de ameaça: protegido.</span><span class="sxs-lookup"><span data-stu-id="4d34b-118">Device Threat Level requirement: Secured.</span></span> <span data-ttu-id="4d34b-119">Isso é o nível mais seguro e representa que nenhuma ameaça foram encontrada no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d34b-119">This is the most secure level, and represents that no threats were found on the device.</span></span>|
|<span data-ttu-id="4d34b-120">low</span><span class="sxs-lookup"><span data-stu-id="4d34b-120">low</span></span>|<span data-ttu-id="4d34b-121">2</span><span class="sxs-lookup"><span data-stu-id="4d34b-121">2</span></span>|<span data-ttu-id="4d34b-122">Requisito de nível de proteção contra ameaças de dispositivo: baixa.</span><span class="sxs-lookup"><span data-stu-id="4d34b-122">Device Threat Protection level requirement: Low.</span></span> <span data-ttu-id="4d34b-123">Baixa representa severidade ameaça que representa um risco mínimo para o dispositivo ou os dados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d34b-123">Low represents a severity of threat that poses minimal risk to the device or device data.</span></span>|
|<span data-ttu-id="4d34b-124">medium</span><span class="sxs-lookup"><span data-stu-id="4d34b-124">medium</span></span>|<span data-ttu-id="4d34b-125">3</span><span class="sxs-lookup"><span data-stu-id="4d34b-125">3</span></span>|<span data-ttu-id="4d34b-126">Requisito de nível de proteção contra ameaças de dispositivo: médio.</span><span class="sxs-lookup"><span data-stu-id="4d34b-126">Device Threat Protection level requirement: Medium.</span></span> <span data-ttu-id="4d34b-127">Médio representa severidade ameaça que traz moderar risco ao dispositivo ou dados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d34b-127">Medium represents a severity of threat that poses moderate risk to the device or device data.</span></span>|
|<span data-ttu-id="4d34b-128">high</span><span class="sxs-lookup"><span data-stu-id="4d34b-128">high</span></span>|<span data-ttu-id="4d34b-129">4</span><span class="sxs-lookup"><span data-stu-id="4d34b-129">4</span></span>|<span data-ttu-id="4d34b-130">Requisito de nível de proteção contra ameaças de dispositivo: alta.</span><span class="sxs-lookup"><span data-stu-id="4d34b-130">Device Threat Protection level requirement: High.</span></span> <span data-ttu-id="4d34b-131">Alta representa severidade ameaça que representa um risco severo para o dispositivo ou os dados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4d34b-131">High represents a severity of threat that poses severe risk to the device or device data.</span></span>|
|<span data-ttu-id="4d34b-132">notSet</span><span class="sxs-lookup"><span data-stu-id="4d34b-132">notSet</span></span>|<span data-ttu-id="4d34b-133">10</span><span class="sxs-lookup"><span data-stu-id="4d34b-133">10</span></span>|<span data-ttu-id="4d34b-134">Requisito de nível de proteção contra ameaças do dispositivo: não definido.</span><span class="sxs-lookup"><span data-stu-id="4d34b-134">Device Threat Protection level requirement: Not Set.</span></span> <span data-ttu-id="4d34b-135">Não set representa que não há nenhuma exigência para o dispositivo atender a um nível de proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="4d34b-135">Not set represents that there is no requirement for the device to meet a Threat Protection level.</span></span>|




