---
title: tipo de enumeração managedDevicePartnerReportedHealthState
description: Estados de integridade disponíveis para a API de integridade do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b0df2859ccee3d4eff9b98c6effb44a4552d93db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091058"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a><span data-ttu-id="2f6b6-103">tipo de enumeração managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="2f6b6-103">managedDevicePartnerReportedHealthState enum type</span></span>

<span data-ttu-id="2f6b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f6b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f6b6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f6b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f6b6-106">Estados de integridade disponíveis para a API de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2f6b6-106">Available health states for the Device Health API</span></span>

## <a name="members"></a><span data-ttu-id="2f6b6-107">Membros</span><span class="sxs-lookup"><span data-stu-id="2f6b6-107">Members</span></span>
|<span data-ttu-id="2f6b6-108">Membro</span><span class="sxs-lookup"><span data-stu-id="2f6b6-108">Member</span></span>|<span data-ttu-id="2f6b6-109">Valor</span><span class="sxs-lookup"><span data-stu-id="2f6b6-109">Value</span></span>|<span data-ttu-id="2f6b6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f6b6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f6b6-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="2f6b6-111">unknown</span></span>|<span data-ttu-id="2f6b6-112">,0</span><span class="sxs-lookup"><span data-stu-id="2f6b6-112">0</span></span>|<span data-ttu-id="2f6b6-113">O estado de integridade do dispositivo ainda não foi relatado</span><span class="sxs-lookup"><span data-stu-id="2f6b6-113">Device health state is not yet reported</span></span>|
|<span data-ttu-id="2f6b6-114">ativado</span><span class="sxs-lookup"><span data-stu-id="2f6b6-114">activated</span></span>|<span data-ttu-id="2f6b6-115">1 </span><span class="sxs-lookup"><span data-stu-id="2f6b6-115">1</span></span>|<span data-ttu-id="2f6b6-116">O dispositivo foi ativado por um parceiro de defesa contra ameaças móveis, mas ainda não relatou a integridade.</span><span class="sxs-lookup"><span data-stu-id="2f6b6-116">Device has been activated by a mobile threat defense partner, but has not yet reported health.</span></span>|
|<span data-ttu-id="2f6b6-117">desativada</span><span class="sxs-lookup"><span data-stu-id="2f6b6-117">deactivated</span></span>|<span data-ttu-id="2f6b6-118">2 </span><span class="sxs-lookup"><span data-stu-id="2f6b6-118">2</span></span>|<span data-ttu-id="2f6b6-119">O dispositivo foi desativado por um parceiro de defesa contra ameaças móveis.</span><span class="sxs-lookup"><span data-stu-id="2f6b6-119">Device has been deactivated by a mobile threat defense partner.</span></span> <span data-ttu-id="2f6b6-120">A integridade do dispositivo não é conhecida.</span><span class="sxs-lookup"><span data-stu-id="2f6b6-120">The device health is not known.</span></span>|
|<span data-ttu-id="2f6b6-121">presos</span><span class="sxs-lookup"><span data-stu-id="2f6b6-121">secured</span></span>|<span data-ttu-id="2f6b6-122">3D</span><span class="sxs-lookup"><span data-stu-id="2f6b6-122">3</span></span>|<span data-ttu-id="2f6b6-123">O dispositivo é considerado protegido pelo parceiro de defesa contra ameaças móveis.</span><span class="sxs-lookup"><span data-stu-id="2f6b6-123">Device is considered secured by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="2f6b6-124">lowSeverity</span><span class="sxs-lookup"><span data-stu-id="2f6b6-124">lowSeverity</span></span>|<span data-ttu-id="2f6b6-125">4 </span><span class="sxs-lookup"><span data-stu-id="2f6b6-125">4</span></span>|<span data-ttu-id="2f6b6-126">O dispositivo é considerado com baixa ameaça pelo parceiro de defesa contra ameaças móveis.</span><span class="sxs-lookup"><span data-stu-id="2f6b6-126">Device is considered low threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="2f6b6-127">mediumSeverity</span><span class="sxs-lookup"><span data-stu-id="2f6b6-127">mediumSeverity</span></span>|<span data-ttu-id="2f6b6-128">5 </span><span class="sxs-lookup"><span data-stu-id="2f6b6-128">5</span></span>|<span data-ttu-id="2f6b6-129">O dispositivo é considerado como ameaça médio pelo parceiro de defesa contra ameaças móveis.</span><span class="sxs-lookup"><span data-stu-id="2f6b6-129">Device is considered medium threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="2f6b6-130">highSeverity</span><span class="sxs-lookup"><span data-stu-id="2f6b6-130">highSeverity</span></span>|<span data-ttu-id="2f6b6-131">6 </span><span class="sxs-lookup"><span data-stu-id="2f6b6-131">6</span></span>|<span data-ttu-id="2f6b6-132">O dispositivo é considerado de alta ameaça pelo parceiro de defesa contra ameaças móveis.</span><span class="sxs-lookup"><span data-stu-id="2f6b6-132">Device is considered high threat by the mobile threat defense partner.</span></span>|
|<span data-ttu-id="2f6b6-133">Não responde</span><span class="sxs-lookup"><span data-stu-id="2f6b6-133">unresponsive</span></span>|<span data-ttu-id="2f6b6-134">7 </span><span class="sxs-lookup"><span data-stu-id="2f6b6-134">7</span></span>|<span data-ttu-id="2f6b6-135">O dispositivo é considerado sem resposta pelo parceiro de defesa contra ameaças móveis.</span><span class="sxs-lookup"><span data-stu-id="2f6b6-135">Device is considered unresponsive by the mobile threat defense partner.</span></span> <span data-ttu-id="2f6b6-136">A integridade do dispositivo não é conhecida.</span><span class="sxs-lookup"><span data-stu-id="2f6b6-136">The device health is not known.</span></span>|
|<span data-ttu-id="2f6b6-137">ficasse</span><span class="sxs-lookup"><span data-stu-id="2f6b6-137">compromised</span></span>|<span data-ttu-id="2f6b6-138">8 </span><span class="sxs-lookup"><span data-stu-id="2f6b6-138">8</span></span>|<span data-ttu-id="2f6b6-139">O dispositivo é considerado comprometido pelo parceiro de proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="2f6b6-139">Device is considered compromised by the Threat Defense partner.</span></span> <span data-ttu-id="2f6b6-140">Isso significa que o dispositivo tem uma ameaça ou risco ativo que não pode ser corrigido facilmente pelo usuário final e o usuário deve entrar em contato com o administrador de ti.</span><span class="sxs-lookup"><span data-stu-id="2f6b6-140">This means the device has an active Threat or Risk which cannot be easily remediated by the end user and the user should contact their IT Admin.</span></span>|
|<span data-ttu-id="2f6b6-141">configurado incorretamente</span><span class="sxs-lookup"><span data-stu-id="2f6b6-141">misconfigured</span></span>|<span data-ttu-id="2f6b6-142">9 </span><span class="sxs-lookup"><span data-stu-id="2f6b6-142">9</span></span>|<span data-ttu-id="2f6b6-143">O dispositivo é considerado incorretamente configurado com o parceiro de proteção contra ameaças.</span><span class="sxs-lookup"><span data-stu-id="2f6b6-143">Device is considered misconfigured with the Threat Defense partner.</span></span> <span data-ttu-id="2f6b6-144">Isso significa que o dispositivo não tem um perfil ou uma configuração necessária para que o parceiro de defesa contra ameaças funcione corretamente, e, portanto, a análise de ameaças ou riscos não pode ser concluída.</span><span class="sxs-lookup"><span data-stu-id="2f6b6-144">This means the device is missing a required profile or configuration for the Threat Defense Partner to function properly and is thus threat or risk analysis is not able to complete.</span></span>|









