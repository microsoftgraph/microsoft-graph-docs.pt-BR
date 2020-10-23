---
title: tipo de enumeração à
description: Wi-Fi tipos de segurança.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e01faac094cd2ae040137b251d30006883388173
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732527"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="649d2-103">tipo de enumeração à</span><span class="sxs-lookup"><span data-stu-id="649d2-103">wiFiSecurityType enum type</span></span>

<span data-ttu-id="649d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="649d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="649d2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="649d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="649d2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="649d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="649d2-107">Wi-Fi tipos de segurança.</span><span class="sxs-lookup"><span data-stu-id="649d2-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="649d2-108">Membros</span><span class="sxs-lookup"><span data-stu-id="649d2-108">Members</span></span>
|<span data-ttu-id="649d2-109">Membro</span><span class="sxs-lookup"><span data-stu-id="649d2-109">Member</span></span>|<span data-ttu-id="649d2-110">Valor</span><span class="sxs-lookup"><span data-stu-id="649d2-110">Value</span></span>|<span data-ttu-id="649d2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="649d2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="649d2-112">Abre</span><span class="sxs-lookup"><span data-stu-id="649d2-112">open</span></span>|<span data-ttu-id="649d2-113">,0</span><span class="sxs-lookup"><span data-stu-id="649d2-113">0</span></span>|<span data-ttu-id="649d2-114">Abrir (sem autenticação).</span><span class="sxs-lookup"><span data-stu-id="649d2-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="649d2-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="649d2-115">wpaPersonal</span></span>|<span data-ttu-id="649d2-116">1</span><span class="sxs-lookup"><span data-stu-id="649d2-116">1</span></span>|<span data-ttu-id="649d2-117">WPA-pessoal.</span><span class="sxs-lookup"><span data-stu-id="649d2-117">WPA-Personal.</span></span>|
|<span data-ttu-id="649d2-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="649d2-118">wpaEnterprise</span></span>|<span data-ttu-id="649d2-119">duas</span><span class="sxs-lookup"><span data-stu-id="649d2-119">2</span></span>|<span data-ttu-id="649d2-120">WPA-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="649d2-120">WPA-Enterprise.</span></span> <span data-ttu-id="649d2-121">Deve usar o tipo IOSEnterpriseWifiConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="649d2-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="649d2-122">Deixa</span><span class="sxs-lookup"><span data-stu-id="649d2-122">wep</span></span>|<span data-ttu-id="649d2-123">3D</span><span class="sxs-lookup"><span data-stu-id="649d2-123">3</span></span>|<span data-ttu-id="649d2-124">Criptografia WEP.</span><span class="sxs-lookup"><span data-stu-id="649d2-124">WEP Encryption.</span></span>|
|<span data-ttu-id="649d2-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="649d2-125">wpa2Personal</span></span>|<span data-ttu-id="649d2-126">4 </span><span class="sxs-lookup"><span data-stu-id="649d2-126">4</span></span>|<span data-ttu-id="649d2-127">WPA2-Pessoal.</span><span class="sxs-lookup"><span data-stu-id="649d2-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="649d2-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="649d2-128">wpa2Enterprise</span></span>|<span data-ttu-id="649d2-129">5 </span><span class="sxs-lookup"><span data-stu-id="649d2-129">5</span></span>|<span data-ttu-id="649d2-130">WPA2-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="649d2-130">WPA2-Enterprise.</span></span> <span data-ttu-id="649d2-131">Deve usar o tipo WindowsWifiEnterpriseEAPConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="649d2-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





