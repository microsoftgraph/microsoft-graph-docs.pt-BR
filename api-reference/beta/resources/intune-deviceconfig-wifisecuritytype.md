---
title: tipo de enumeração à
description: Wi-Fi tipos de segurança.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 112612969027be87805b77c5743e1a8d0561c03b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49215334"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="6ebd4-103">tipo de enumeração à</span><span class="sxs-lookup"><span data-stu-id="6ebd4-103">wiFiSecurityType enum type</span></span>

<span data-ttu-id="6ebd4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ebd4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ebd4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ebd4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ebd4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ebd4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ebd4-107">Wi-Fi tipos de segurança.</span><span class="sxs-lookup"><span data-stu-id="6ebd4-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="6ebd4-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6ebd4-108">Members</span></span>
|<span data-ttu-id="6ebd4-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6ebd4-109">Member</span></span>|<span data-ttu-id="6ebd4-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6ebd4-110">Value</span></span>|<span data-ttu-id="6ebd4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ebd4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ebd4-112">Abre</span><span class="sxs-lookup"><span data-stu-id="6ebd4-112">open</span></span>|<span data-ttu-id="6ebd4-113">,0</span><span class="sxs-lookup"><span data-stu-id="6ebd4-113">0</span></span>|<span data-ttu-id="6ebd4-114">Abrir (sem autenticação).</span><span class="sxs-lookup"><span data-stu-id="6ebd4-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="6ebd4-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="6ebd4-115">wpaPersonal</span></span>|<span data-ttu-id="6ebd4-116">1</span><span class="sxs-lookup"><span data-stu-id="6ebd4-116">1</span></span>|<span data-ttu-id="6ebd4-117">WPA-pessoal.</span><span class="sxs-lookup"><span data-stu-id="6ebd4-117">WPA-Personal.</span></span>|
|<span data-ttu-id="6ebd4-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="6ebd4-118">wpaEnterprise</span></span>|<span data-ttu-id="6ebd4-119">duas</span><span class="sxs-lookup"><span data-stu-id="6ebd4-119">2</span></span>|<span data-ttu-id="6ebd4-120">WPA-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="6ebd4-120">WPA-Enterprise.</span></span> <span data-ttu-id="6ebd4-121">Deve usar o tipo IOSEnterpriseWifiConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="6ebd4-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="6ebd4-122">Deixa</span><span class="sxs-lookup"><span data-stu-id="6ebd4-122">wep</span></span>|<span data-ttu-id="6ebd4-123">3D</span><span class="sxs-lookup"><span data-stu-id="6ebd4-123">3</span></span>|<span data-ttu-id="6ebd4-124">Criptografia WEP.</span><span class="sxs-lookup"><span data-stu-id="6ebd4-124">WEP Encryption.</span></span>|
|<span data-ttu-id="6ebd4-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="6ebd4-125">wpa2Personal</span></span>|<span data-ttu-id="6ebd4-126">4 </span><span class="sxs-lookup"><span data-stu-id="6ebd4-126">4</span></span>|<span data-ttu-id="6ebd4-127">WPA2-Pessoal.</span><span class="sxs-lookup"><span data-stu-id="6ebd4-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="6ebd4-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="6ebd4-128">wpa2Enterprise</span></span>|<span data-ttu-id="6ebd4-129">5 </span><span class="sxs-lookup"><span data-stu-id="6ebd4-129">5</span></span>|<span data-ttu-id="6ebd4-130">WPA2-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="6ebd4-130">WPA2-Enterprise.</span></span> <span data-ttu-id="6ebd4-131">Deve usar o tipo WindowsWifiEnterpriseEAPConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="6ebd4-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|




