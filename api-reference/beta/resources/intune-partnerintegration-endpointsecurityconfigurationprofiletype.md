---
title: tipo de enumeração endpointSecurityConfigurationProfileType
description: O tipo de perfil da política de segurança do ponto de extremidade.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e766ad484d26abd770e2655b1f75e455306ad82
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793164"
---
# <a name="endpointsecurityconfigurationprofiletype-enum-type"></a><span data-ttu-id="2790d-103">tipo de enumeração endpointSecurityConfigurationProfileType</span><span class="sxs-lookup"><span data-stu-id="2790d-103">endpointSecurityConfigurationProfileType enum type</span></span>

<span data-ttu-id="2790d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2790d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2790d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2790d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2790d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2790d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2790d-107">O tipo de perfil da política de segurança do ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="2790d-107">The endpoint security policy profile type.</span></span>

## <a name="members"></a><span data-ttu-id="2790d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2790d-108">Members</span></span>
|<span data-ttu-id="2790d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2790d-109">Member</span></span>|<span data-ttu-id="2790d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2790d-110">Value</span></span>|<span data-ttu-id="2790d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2790d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2790d-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="2790d-112">unknown</span></span>|<span data-ttu-id="2790d-113">,0</span><span class="sxs-lookup"><span data-stu-id="2790d-113">0</span></span>|<span data-ttu-id="2790d-114">Unknown.</span><span class="sxs-lookup"><span data-stu-id="2790d-114">Unknown.</span></span>|
|<span data-ttu-id="2790d-115">vírus</span><span class="sxs-lookup"><span data-stu-id="2790d-115">antivirus</span></span>|<span data-ttu-id="2790d-116">1</span><span class="sxs-lookup"><span data-stu-id="2790d-116">1</span></span>|<span data-ttu-id="2790d-117">Vírus.</span><span class="sxs-lookup"><span data-stu-id="2790d-117">Antivirus.</span></span>|
|<span data-ttu-id="2790d-118">windowsSecurity</span><span class="sxs-lookup"><span data-stu-id="2790d-118">windowsSecurity</span></span>|<span data-ttu-id="2790d-119">duas</span><span class="sxs-lookup"><span data-stu-id="2790d-119">2</span></span>|<span data-ttu-id="2790d-120">Segurança do Windows.</span><span class="sxs-lookup"><span data-stu-id="2790d-120">Windows Security.</span></span>|
|<span data-ttu-id="2790d-121">bitLocker</span><span class="sxs-lookup"><span data-stu-id="2790d-121">bitLocker</span></span>|<span data-ttu-id="2790d-122">3D</span><span class="sxs-lookup"><span data-stu-id="2790d-122">3</span></span>|<span data-ttu-id="2790d-123">BitLocker.</span><span class="sxs-lookup"><span data-stu-id="2790d-123">BitLocker.</span></span>|
|<span data-ttu-id="2790d-124">fileVault</span><span class="sxs-lookup"><span data-stu-id="2790d-124">fileVault</span></span>|<span data-ttu-id="2790d-125">4 </span><span class="sxs-lookup"><span data-stu-id="2790d-125">4</span></span>|<span data-ttu-id="2790d-126">FileVault.</span><span class="sxs-lookup"><span data-stu-id="2790d-126">FileVault.</span></span>|
|<span data-ttu-id="2790d-127">Firewall</span><span class="sxs-lookup"><span data-stu-id="2790d-127">firewall</span></span>|<span data-ttu-id="2790d-128">5 </span><span class="sxs-lookup"><span data-stu-id="2790d-128">5</span></span>|<span data-ttu-id="2790d-129">Firewall.</span><span class="sxs-lookup"><span data-stu-id="2790d-129">Firewall.</span></span>|
|<span data-ttu-id="2790d-130">firewallRules</span><span class="sxs-lookup"><span data-stu-id="2790d-130">firewallRules</span></span>|<span data-ttu-id="2790d-131">6 </span><span class="sxs-lookup"><span data-stu-id="2790d-131">6</span></span>|<span data-ttu-id="2790d-132">Regras de firewall.</span><span class="sxs-lookup"><span data-stu-id="2790d-132">Firewall rules.</span></span>|
|<span data-ttu-id="2790d-133">endpointDetectionAndResponse</span><span class="sxs-lookup"><span data-stu-id="2790d-133">endpointDetectionAndResponse</span></span>|<span data-ttu-id="2790d-134">7 </span><span class="sxs-lookup"><span data-stu-id="2790d-134">7</span></span>|<span data-ttu-id="2790d-135">Detecção e resposta do terminal.</span><span class="sxs-lookup"><span data-stu-id="2790d-135">Endpoint detection and response.</span></span>|
|<span data-ttu-id="2790d-136">deviceControl</span><span class="sxs-lookup"><span data-stu-id="2790d-136">deviceControl</span></span>|<span data-ttu-id="2790d-137">8 </span><span class="sxs-lookup"><span data-stu-id="2790d-137">8</span></span>|<span data-ttu-id="2790d-138">Controle de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2790d-138">Device control.</span></span>|
|<span data-ttu-id="2790d-139">appAndBrowserIsolation</span><span class="sxs-lookup"><span data-stu-id="2790d-139">appAndBrowserIsolation</span></span>|<span data-ttu-id="2790d-140">9 </span><span class="sxs-lookup"><span data-stu-id="2790d-140">9</span></span>|<span data-ttu-id="2790d-141">Isolamento de aplicativo e navegador.</span><span class="sxs-lookup"><span data-stu-id="2790d-141">App and browser isolation.</span></span>|
|<span data-ttu-id="2790d-142">exploitProtection</span><span class="sxs-lookup"><span data-stu-id="2790d-142">exploitProtection</span></span>|<span data-ttu-id="2790d-143">10 </span><span class="sxs-lookup"><span data-stu-id="2790d-143">10</span></span>|<span data-ttu-id="2790d-144">Explorar proteção.</span><span class="sxs-lookup"><span data-stu-id="2790d-144">Exploit protection.</span></span>|
|<span data-ttu-id="2790d-145">Proteção WebProtection</span><span class="sxs-lookup"><span data-stu-id="2790d-145">webProtection</span></span>|<span data-ttu-id="2790d-146">11</span><span class="sxs-lookup"><span data-stu-id="2790d-146">11</span></span>|<span data-ttu-id="2790d-147">Proteção da Web.</span><span class="sxs-lookup"><span data-stu-id="2790d-147">Web protection.</span></span>|
|<span data-ttu-id="2790d-148">applicationControl</span><span class="sxs-lookup"><span data-stu-id="2790d-148">applicationControl</span></span>|<span data-ttu-id="2790d-149">12 </span><span class="sxs-lookup"><span data-stu-id="2790d-149">12</span></span>|<span data-ttu-id="2790d-150">Controle da aplicação.</span><span class="sxs-lookup"><span data-stu-id="2790d-150">Application control.</span></span>|
|<span data-ttu-id="2790d-151">attackSurfaceReductionRules</span><span class="sxs-lookup"><span data-stu-id="2790d-151">attackSurfaceReductionRules</span></span>|<span data-ttu-id="2790d-152">Treze</span><span class="sxs-lookup"><span data-stu-id="2790d-152">13</span></span>|<span data-ttu-id="2790d-153">Regras de redução da superfície de ataque.</span><span class="sxs-lookup"><span data-stu-id="2790d-153">Attack surface reduction rules.</span></span>|
|<span data-ttu-id="2790d-154">accountProtection</span><span class="sxs-lookup"><span data-stu-id="2790d-154">accountProtection</span></span>|<span data-ttu-id="2790d-155">14 </span><span class="sxs-lookup"><span data-stu-id="2790d-155">14</span></span>|<span data-ttu-id="2790d-156">Proteção de conta.</span><span class="sxs-lookup"><span data-stu-id="2790d-156">Account protection.</span></span>|



