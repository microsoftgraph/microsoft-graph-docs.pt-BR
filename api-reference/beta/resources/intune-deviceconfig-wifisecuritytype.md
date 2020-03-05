---
title: tipo de enumeração à
description: Tipos de segurança Wi-Fi.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 33d7116bb686945672d96d20035d18ed1df3ee9e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525702"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="baa80-103">tipo de enumeração à</span><span class="sxs-lookup"><span data-stu-id="baa80-103">wiFiSecurityType enum type</span></span>

<span data-ttu-id="baa80-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="baa80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="baa80-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="baa80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="baa80-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="baa80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baa80-107">Tipos de segurança Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="baa80-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="baa80-108">Membros</span><span class="sxs-lookup"><span data-stu-id="baa80-108">Members</span></span>
|<span data-ttu-id="baa80-109">Membro</span><span class="sxs-lookup"><span data-stu-id="baa80-109">Member</span></span>|<span data-ttu-id="baa80-110">Valor</span><span class="sxs-lookup"><span data-stu-id="baa80-110">Value</span></span>|<span data-ttu-id="baa80-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="baa80-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baa80-112">Abre</span><span class="sxs-lookup"><span data-stu-id="baa80-112">open</span></span>|<span data-ttu-id="baa80-113">,0</span><span class="sxs-lookup"><span data-stu-id="baa80-113">0</span></span>|<span data-ttu-id="baa80-114">Abrir (sem autenticação).</span><span class="sxs-lookup"><span data-stu-id="baa80-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="baa80-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="baa80-115">wpaPersonal</span></span>|<span data-ttu-id="baa80-116">1 </span><span class="sxs-lookup"><span data-stu-id="baa80-116">1</span></span>|<span data-ttu-id="baa80-117">WPA-pessoal.</span><span class="sxs-lookup"><span data-stu-id="baa80-117">WPA-Personal.</span></span>|
|<span data-ttu-id="baa80-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="baa80-118">wpaEnterprise</span></span>|<span data-ttu-id="baa80-119">2 </span><span class="sxs-lookup"><span data-stu-id="baa80-119">2</span></span>|<span data-ttu-id="baa80-120">WPA-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="baa80-120">WPA-Enterprise.</span></span> <span data-ttu-id="baa80-121">Deve usar o tipo IOSEnterpriseWifiConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="baa80-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="baa80-122">Deixa</span><span class="sxs-lookup"><span data-stu-id="baa80-122">wep</span></span>|<span data-ttu-id="baa80-123">3 </span><span class="sxs-lookup"><span data-stu-id="baa80-123">3</span></span>|<span data-ttu-id="baa80-124">Criptografia WEP.</span><span class="sxs-lookup"><span data-stu-id="baa80-124">WEP Encryption.</span></span>|
|<span data-ttu-id="baa80-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="baa80-125">wpa2Personal</span></span>|<span data-ttu-id="baa80-126">4 </span><span class="sxs-lookup"><span data-stu-id="baa80-126">4</span></span>|<span data-ttu-id="baa80-127">WPA2-Pessoal.</span><span class="sxs-lookup"><span data-stu-id="baa80-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="baa80-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="baa80-128">wpa2Enterprise</span></span>|<span data-ttu-id="baa80-129">5 </span><span class="sxs-lookup"><span data-stu-id="baa80-129">5</span></span>|<span data-ttu-id="baa80-130">WPA2-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="baa80-130">WPA2-Enterprise.</span></span> <span data-ttu-id="baa80-131">Deve usar o tipo WindowsWifiEnterpriseEAPConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="baa80-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|



