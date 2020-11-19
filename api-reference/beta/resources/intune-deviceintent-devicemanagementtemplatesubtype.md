---
title: tipo de enumeração deviceManagementTemplateSubtype
description: Subtipo de modelo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6766834a860d06501cd34a423c457f5ac584b6d3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209441"
---
# <a name="devicemanagementtemplatesubtype-enum-type"></a><span data-ttu-id="f39cc-103">tipo de enumeração deviceManagementTemplateSubtype</span><span class="sxs-lookup"><span data-stu-id="f39cc-103">deviceManagementTemplateSubtype enum type</span></span>

<span data-ttu-id="f39cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f39cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f39cc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f39cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f39cc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f39cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f39cc-107">Subtipo de modelo</span><span class="sxs-lookup"><span data-stu-id="f39cc-107">Template subtype</span></span>

## <a name="members"></a><span data-ttu-id="f39cc-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f39cc-108">Members</span></span>
|<span data-ttu-id="f39cc-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f39cc-109">Member</span></span>|<span data-ttu-id="f39cc-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f39cc-110">Value</span></span>|<span data-ttu-id="f39cc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f39cc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f39cc-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="f39cc-112">none</span></span>|<span data-ttu-id="f39cc-113">,0</span><span class="sxs-lookup"><span data-stu-id="f39cc-113">0</span></span>|<span data-ttu-id="f39cc-114">O modelo não tem subtipo</span><span class="sxs-lookup"><span data-stu-id="f39cc-114">Template has no subtype</span></span>|
|<span data-ttu-id="f39cc-115">Firewall</span><span class="sxs-lookup"><span data-stu-id="f39cc-115">firewall</span></span>|<span data-ttu-id="f39cc-116">1</span><span class="sxs-lookup"><span data-stu-id="f39cc-116">1</span></span>|<span data-ttu-id="f39cc-117">Subtipo de firewall de segurança do Endpoint</span><span class="sxs-lookup"><span data-stu-id="f39cc-117">Endpoint security firewall subtype</span></span>|
|<span data-ttu-id="f39cc-118">diskEncryption</span><span class="sxs-lookup"><span data-stu-id="f39cc-118">diskEncryption</span></span>|<span data-ttu-id="f39cc-119">duas</span><span class="sxs-lookup"><span data-stu-id="f39cc-119">2</span></span>|<span data-ttu-id="f39cc-120">Subtipo de criptografia de disco do Endpoint Security</span><span class="sxs-lookup"><span data-stu-id="f39cc-120">Endpoint security disk encryption subtype</span></span>|
|<span data-ttu-id="f39cc-121">attackSurfaceReduction</span><span class="sxs-lookup"><span data-stu-id="f39cc-121">attackSurfaceReduction</span></span>|<span data-ttu-id="f39cc-122">3D</span><span class="sxs-lookup"><span data-stu-id="f39cc-122">3</span></span>|<span data-ttu-id="f39cc-123">Subtipo de redução da superfície de ataque de segurança de pontos de extremidade</span><span class="sxs-lookup"><span data-stu-id="f39cc-123">Endpoint security attack surface reduction subtype</span></span>|
|<span data-ttu-id="f39cc-124">endpointDetectionReponse</span><span class="sxs-lookup"><span data-stu-id="f39cc-124">endpointDetectionReponse</span></span>|<span data-ttu-id="f39cc-125">4 </span><span class="sxs-lookup"><span data-stu-id="f39cc-125">4</span></span>|<span data-ttu-id="f39cc-126">Detecção de ponto de extremidade de segurança e subtipo de resposta do Endpoint Security</span><span class="sxs-lookup"><span data-stu-id="f39cc-126">Endpoint security endpoint detection and response subtype</span></span>|
|<span data-ttu-id="f39cc-127">accountProtection</span><span class="sxs-lookup"><span data-stu-id="f39cc-127">accountProtection</span></span>|<span data-ttu-id="f39cc-128">5 </span><span class="sxs-lookup"><span data-stu-id="f39cc-128">5</span></span>|<span data-ttu-id="f39cc-129">Subtipo de proteção da conta do Endpoint Security</span><span class="sxs-lookup"><span data-stu-id="f39cc-129">Endpoint security account protection subtype</span></span>|
|<span data-ttu-id="f39cc-130">vírus</span><span class="sxs-lookup"><span data-stu-id="f39cc-130">antivirus</span></span>|<span data-ttu-id="f39cc-131">6 </span><span class="sxs-lookup"><span data-stu-id="f39cc-131">6</span></span>|<span data-ttu-id="f39cc-132">Subtipo Anitivirus de segurança de ponto de extremidade</span><span class="sxs-lookup"><span data-stu-id="f39cc-132">Endpoint security anitivirus subtype</span></span>|
|<span data-ttu-id="f39cc-133">firewallSharedAppList</span><span class="sxs-lookup"><span data-stu-id="f39cc-133">firewallSharedAppList</span></span>|<span data-ttu-id="f39cc-134">7 </span><span class="sxs-lookup"><span data-stu-id="f39cc-134">7</span></span>|<span data-ttu-id="f39cc-135">Subtipo de aplicativo compartilhado do Endpoint Security firewall</span><span class="sxs-lookup"><span data-stu-id="f39cc-135">Endpoint security firewall shared app subtype</span></span>|
|<span data-ttu-id="f39cc-136">firewallSharedIpList</span><span class="sxs-lookup"><span data-stu-id="f39cc-136">firewallSharedIpList</span></span>|<span data-ttu-id="f39cc-137">8 </span><span class="sxs-lookup"><span data-stu-id="f39cc-137">8</span></span>|<span data-ttu-id="f39cc-138">Subtipo de lista de intervalos de IP compartilhado do firewall do Endpoint Security</span><span class="sxs-lookup"><span data-stu-id="f39cc-138">Endpoint security firewall shared ip range list subtype</span></span>|
|<span data-ttu-id="f39cc-139">firewallSharedPortlist</span><span class="sxs-lookup"><span data-stu-id="f39cc-139">firewallSharedPortlist</span></span>|<span data-ttu-id="f39cc-140">9 </span><span class="sxs-lookup"><span data-stu-id="f39cc-140">9</span></span>|<span data-ttu-id="f39cc-141">Subtipo de lista de intervalos de porta compartilhada do firewall do Endpoint Security</span><span class="sxs-lookup"><span data-stu-id="f39cc-141">Endpoint security firewall shared port range list subtype</span></span>|




