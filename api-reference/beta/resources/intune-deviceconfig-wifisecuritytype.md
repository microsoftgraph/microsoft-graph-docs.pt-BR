---
title: tipo de enumeração à
description: Tipos de segurança Wi-Fi.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22dd7bf07e6355dd92f04461120e3afb142d6d9a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048873"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="f4a2f-103">tipo de enumeração à</span><span class="sxs-lookup"><span data-stu-id="f4a2f-103">wiFiSecurityType enum type</span></span>

<span data-ttu-id="f4a2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4a2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4a2f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4a2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4a2f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4a2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4a2f-107">Tipos de segurança Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f4a2f-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="f4a2f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f4a2f-108">Members</span></span>
|<span data-ttu-id="f4a2f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f4a2f-109">Member</span></span>|<span data-ttu-id="f4a2f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f4a2f-110">Value</span></span>|<span data-ttu-id="f4a2f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4a2f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4a2f-112">Abre</span><span class="sxs-lookup"><span data-stu-id="f4a2f-112">open</span></span>|<span data-ttu-id="f4a2f-113">,0</span><span class="sxs-lookup"><span data-stu-id="f4a2f-113">0</span></span>|<span data-ttu-id="f4a2f-114">Abrir (sem autenticação).</span><span class="sxs-lookup"><span data-stu-id="f4a2f-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="f4a2f-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="f4a2f-115">wpaPersonal</span></span>|<span data-ttu-id="f4a2f-116">1 </span><span class="sxs-lookup"><span data-stu-id="f4a2f-116">1</span></span>|<span data-ttu-id="f4a2f-117">WPA-pessoal.</span><span class="sxs-lookup"><span data-stu-id="f4a2f-117">WPA-Personal.</span></span>|
|<span data-ttu-id="f4a2f-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="f4a2f-118">wpaEnterprise</span></span>|<span data-ttu-id="f4a2f-119">2 </span><span class="sxs-lookup"><span data-stu-id="f4a2f-119">2</span></span>|<span data-ttu-id="f4a2f-120">WPA-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="f4a2f-120">WPA-Enterprise.</span></span> <span data-ttu-id="f4a2f-121">Deve usar o tipo IOSEnterpriseWifiConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="f4a2f-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="f4a2f-122">Deixa</span><span class="sxs-lookup"><span data-stu-id="f4a2f-122">wep</span></span>|<span data-ttu-id="f4a2f-123">3 </span><span class="sxs-lookup"><span data-stu-id="f4a2f-123">3</span></span>|<span data-ttu-id="f4a2f-124">Criptografia WEP.</span><span class="sxs-lookup"><span data-stu-id="f4a2f-124">WEP Encryption.</span></span>|
|<span data-ttu-id="f4a2f-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="f4a2f-125">wpa2Personal</span></span>|<span data-ttu-id="f4a2f-126">4 </span><span class="sxs-lookup"><span data-stu-id="f4a2f-126">4</span></span>|<span data-ttu-id="f4a2f-127">WPA2-Pessoal.</span><span class="sxs-lookup"><span data-stu-id="f4a2f-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="f4a2f-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="f4a2f-128">wpa2Enterprise</span></span>|<span data-ttu-id="f4a2f-129">5 </span><span class="sxs-lookup"><span data-stu-id="f4a2f-129">5</span></span>|<span data-ttu-id="f4a2f-130">WPA2-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="f4a2f-130">WPA2-Enterprise.</span></span> <span data-ttu-id="f4a2f-131">Deve usar o tipo WindowsWifiEnterpriseEAPConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="f4a2f-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|






