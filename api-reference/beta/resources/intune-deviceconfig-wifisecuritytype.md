---
title: tipo de enumeração à
description: Tipos de segurança Wi-Fi.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4c770ce8d3e00a8d7997b2b72fcd18eb9007ba83
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787233"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="51ed9-103">tipo de enumeração à</span><span class="sxs-lookup"><span data-stu-id="51ed9-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="51ed9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="51ed9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51ed9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51ed9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51ed9-106">Tipos de segurança Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="51ed9-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="51ed9-107">Membros</span><span class="sxs-lookup"><span data-stu-id="51ed9-107">Members</span></span>
|<span data-ttu-id="51ed9-108">Membro</span><span class="sxs-lookup"><span data-stu-id="51ed9-108">Member</span></span>|<span data-ttu-id="51ed9-109">Valor</span><span class="sxs-lookup"><span data-stu-id="51ed9-109">Value</span></span>|<span data-ttu-id="51ed9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="51ed9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51ed9-111">Abre</span><span class="sxs-lookup"><span data-stu-id="51ed9-111">open</span></span>|<span data-ttu-id="51ed9-112">,0</span><span class="sxs-lookup"><span data-stu-id="51ed9-112">0</span></span>|<span data-ttu-id="51ed9-113">Abrir (sem autenticação).</span><span class="sxs-lookup"><span data-stu-id="51ed9-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="51ed9-114">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="51ed9-114">wpaPersonal</span></span>|<span data-ttu-id="51ed9-115">1</span><span class="sxs-lookup"><span data-stu-id="51ed9-115">1</span></span>|<span data-ttu-id="51ed9-116">WPA-pessoal.</span><span class="sxs-lookup"><span data-stu-id="51ed9-116">WPA-Personal.</span></span>|
|<span data-ttu-id="51ed9-117">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="51ed9-117">wpaEnterprise</span></span>|<span data-ttu-id="51ed9-118">duas</span><span class="sxs-lookup"><span data-stu-id="51ed9-118">2</span></span>|<span data-ttu-id="51ed9-119">WPA-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="51ed9-119">WPA-Enterprise.</span></span> <span data-ttu-id="51ed9-120">Deve usar o tipo IOSEnterpriseWifiConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="51ed9-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="51ed9-121">Deixa</span><span class="sxs-lookup"><span data-stu-id="51ed9-121">wep</span></span>|<span data-ttu-id="51ed9-122">3D</span><span class="sxs-lookup"><span data-stu-id="51ed9-122">3</span></span>|<span data-ttu-id="51ed9-123">Criptografia WEP.</span><span class="sxs-lookup"><span data-stu-id="51ed9-123">WEP Encryption.</span></span>|
|<span data-ttu-id="51ed9-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="51ed9-124">wpa2Personal</span></span>|<span data-ttu-id="51ed9-125">4 </span><span class="sxs-lookup"><span data-stu-id="51ed9-125">4</span></span>|<span data-ttu-id="51ed9-126">WPA2-Pessoal.</span><span class="sxs-lookup"><span data-stu-id="51ed9-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="51ed9-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="51ed9-127">wpa2Enterprise</span></span>|<span data-ttu-id="51ed9-128">5 </span><span class="sxs-lookup"><span data-stu-id="51ed9-128">5</span></span>|<span data-ttu-id="51ed9-129">WPA2-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="51ed9-129">WPA2-Enterprise.</span></span> <span data-ttu-id="51ed9-130">Deve usar o tipo WindowsWifiEnterpriseEAPConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="51ed9-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|



