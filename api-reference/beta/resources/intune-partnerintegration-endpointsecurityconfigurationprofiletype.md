---
title: tipo de enumeração endpointSecurityConfigurationProfileType
description: O tipo de perfil da política de segurança do ponto de extremidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5b3f3340a9e3aa5aa211b39176e9fe43d74b8bf8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993641"
---
# <a name="endpointsecurityconfigurationprofiletype-enum-type"></a><span data-ttu-id="538da-103">tipo de enumeração endpointSecurityConfigurationProfileType</span><span class="sxs-lookup"><span data-stu-id="538da-103">endpointSecurityConfigurationProfileType enum type</span></span>

<span data-ttu-id="538da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="538da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="538da-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="538da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="538da-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="538da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="538da-107">O tipo de perfil da política de segurança do ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="538da-107">The endpoint security policy profile type.</span></span>

## <a name="members"></a><span data-ttu-id="538da-108">Membros</span><span class="sxs-lookup"><span data-stu-id="538da-108">Members</span></span>
|<span data-ttu-id="538da-109">Membro</span><span class="sxs-lookup"><span data-stu-id="538da-109">Member</span></span>|<span data-ttu-id="538da-110">Valor</span><span class="sxs-lookup"><span data-stu-id="538da-110">Value</span></span>|<span data-ttu-id="538da-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="538da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="538da-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="538da-112">unknown</span></span>|<span data-ttu-id="538da-113">,0</span><span class="sxs-lookup"><span data-stu-id="538da-113">0</span></span>|<span data-ttu-id="538da-114">Unknown.</span><span class="sxs-lookup"><span data-stu-id="538da-114">Unknown.</span></span>|
|<span data-ttu-id="538da-115">vírus</span><span class="sxs-lookup"><span data-stu-id="538da-115">antivirus</span></span>|<span data-ttu-id="538da-116">1 </span><span class="sxs-lookup"><span data-stu-id="538da-116">1</span></span>|<span data-ttu-id="538da-117">Vírus.</span><span class="sxs-lookup"><span data-stu-id="538da-117">Antivirus.</span></span>|
|<span data-ttu-id="538da-118">windowsSecurity</span><span class="sxs-lookup"><span data-stu-id="538da-118">windowsSecurity</span></span>|<span data-ttu-id="538da-119">2 </span><span class="sxs-lookup"><span data-stu-id="538da-119">2</span></span>|<span data-ttu-id="538da-120">Segurança do Windows.</span><span class="sxs-lookup"><span data-stu-id="538da-120">Windows Security.</span></span>|
|<span data-ttu-id="538da-121">bitLocker</span><span class="sxs-lookup"><span data-stu-id="538da-121">bitLocker</span></span>|<span data-ttu-id="538da-122">3 </span><span class="sxs-lookup"><span data-stu-id="538da-122">3</span></span>|<span data-ttu-id="538da-123">BitLocker.</span><span class="sxs-lookup"><span data-stu-id="538da-123">BitLocker.</span></span>|
|<span data-ttu-id="538da-124">fileVault</span><span class="sxs-lookup"><span data-stu-id="538da-124">fileVault</span></span>|<span data-ttu-id="538da-125">4 </span><span class="sxs-lookup"><span data-stu-id="538da-125">4</span></span>|<span data-ttu-id="538da-126">FileVault.</span><span class="sxs-lookup"><span data-stu-id="538da-126">FileVault.</span></span>|
|<span data-ttu-id="538da-127">Firewall</span><span class="sxs-lookup"><span data-stu-id="538da-127">firewall</span></span>|<span data-ttu-id="538da-128">5 </span><span class="sxs-lookup"><span data-stu-id="538da-128">5</span></span>|<span data-ttu-id="538da-129">Firewall.</span><span class="sxs-lookup"><span data-stu-id="538da-129">Firewall.</span></span>|
|<span data-ttu-id="538da-130">firewallRules</span><span class="sxs-lookup"><span data-stu-id="538da-130">firewallRules</span></span>|<span data-ttu-id="538da-131">6 </span><span class="sxs-lookup"><span data-stu-id="538da-131">6</span></span>|<span data-ttu-id="538da-132">Regras de firewall.</span><span class="sxs-lookup"><span data-stu-id="538da-132">Firewall rules.</span></span>|
|<span data-ttu-id="538da-133">endpointDetectionAndResponse</span><span class="sxs-lookup"><span data-stu-id="538da-133">endpointDetectionAndResponse</span></span>|<span data-ttu-id="538da-134">7 </span><span class="sxs-lookup"><span data-stu-id="538da-134">7</span></span>|<span data-ttu-id="538da-135">Detecção e resposta do terminal.</span><span class="sxs-lookup"><span data-stu-id="538da-135">Endpoint detection and response.</span></span>|
|<span data-ttu-id="538da-136">deviceControl</span><span class="sxs-lookup"><span data-stu-id="538da-136">deviceControl</span></span>|<span data-ttu-id="538da-137">8 </span><span class="sxs-lookup"><span data-stu-id="538da-137">8</span></span>|<span data-ttu-id="538da-138">Controle de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="538da-138">Device control.</span></span>|
|<span data-ttu-id="538da-139">appAndBrowserIsolation</span><span class="sxs-lookup"><span data-stu-id="538da-139">appAndBrowserIsolation</span></span>|<span data-ttu-id="538da-140">9 </span><span class="sxs-lookup"><span data-stu-id="538da-140">9</span></span>|<span data-ttu-id="538da-141">Isolamento de aplicativo e navegador.</span><span class="sxs-lookup"><span data-stu-id="538da-141">App and browser isolation.</span></span>|
|<span data-ttu-id="538da-142">exploitProtection</span><span class="sxs-lookup"><span data-stu-id="538da-142">exploitProtection</span></span>|<span data-ttu-id="538da-143">10 </span><span class="sxs-lookup"><span data-stu-id="538da-143">10</span></span>|<span data-ttu-id="538da-144">Explorar proteção.</span><span class="sxs-lookup"><span data-stu-id="538da-144">Exploit protection.</span></span>|
|<span data-ttu-id="538da-145">Proteção WebProtection</span><span class="sxs-lookup"><span data-stu-id="538da-145">webProtection</span></span>|<span data-ttu-id="538da-146">11 </span><span class="sxs-lookup"><span data-stu-id="538da-146">11</span></span>|<span data-ttu-id="538da-147">Proteção da Web.</span><span class="sxs-lookup"><span data-stu-id="538da-147">Web protection.</span></span>|
|<span data-ttu-id="538da-148">applicationControl</span><span class="sxs-lookup"><span data-stu-id="538da-148">applicationControl</span></span>|<span data-ttu-id="538da-149">12 </span><span class="sxs-lookup"><span data-stu-id="538da-149">12</span></span>|<span data-ttu-id="538da-150">Controle da aplicação.</span><span class="sxs-lookup"><span data-stu-id="538da-150">Application control.</span></span>|
|<span data-ttu-id="538da-151">attackSurfaceReductionRules</span><span class="sxs-lookup"><span data-stu-id="538da-151">attackSurfaceReductionRules</span></span>|<span data-ttu-id="538da-152">13 </span><span class="sxs-lookup"><span data-stu-id="538da-152">13</span></span>|<span data-ttu-id="538da-153">Regras de redução da superfície de ataque.</span><span class="sxs-lookup"><span data-stu-id="538da-153">Attack surface reduction rules.</span></span>|
|<span data-ttu-id="538da-154">accountProtection</span><span class="sxs-lookup"><span data-stu-id="538da-154">accountProtection</span></span>|<span data-ttu-id="538da-155">14 </span><span class="sxs-lookup"><span data-stu-id="538da-155">14</span></span>|<span data-ttu-id="538da-156">Proteção de conta.</span><span class="sxs-lookup"><span data-stu-id="538da-156">Account protection.</span></span>|






