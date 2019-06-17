---
title: tipo de enumeração à
description: Tipos de segurança Wi-Fi.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2245069bfda8ced7c16d23465d510c98f1bc5eef
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991531"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="2589e-103">tipo de enumeração à</span><span class="sxs-lookup"><span data-stu-id="2589e-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="2589e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2589e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2589e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2589e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2589e-106">Tipos de segurança Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="2589e-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="2589e-107">Membros</span><span class="sxs-lookup"><span data-stu-id="2589e-107">Members</span></span>
|<span data-ttu-id="2589e-108">Membro</span><span class="sxs-lookup"><span data-stu-id="2589e-108">Member</span></span>|<span data-ttu-id="2589e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="2589e-109">Value</span></span>|<span data-ttu-id="2589e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2589e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2589e-111">Abre</span><span class="sxs-lookup"><span data-stu-id="2589e-111">open</span></span>|<span data-ttu-id="2589e-112">,0</span><span class="sxs-lookup"><span data-stu-id="2589e-112">0</span></span>|<span data-ttu-id="2589e-113">Abrir (sem autenticação).</span><span class="sxs-lookup"><span data-stu-id="2589e-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="2589e-114">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="2589e-114">wpaPersonal</span></span>|<span data-ttu-id="2589e-115">1</span><span class="sxs-lookup"><span data-stu-id="2589e-115">1</span></span>|<span data-ttu-id="2589e-116">WPA-pessoal.</span><span class="sxs-lookup"><span data-stu-id="2589e-116">WPA-Personal.</span></span>|
|<span data-ttu-id="2589e-117">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="2589e-117">wpaEnterprise</span></span>|<span data-ttu-id="2589e-118">duas</span><span class="sxs-lookup"><span data-stu-id="2589e-118">2</span></span>|<span data-ttu-id="2589e-119">WPA-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="2589e-119">WPA-Enterprise.</span></span> <span data-ttu-id="2589e-120">Deve usar o tipo IOSEnterpriseWifiConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="2589e-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="2589e-121">Deixa</span><span class="sxs-lookup"><span data-stu-id="2589e-121">wep</span></span>|<span data-ttu-id="2589e-122">3D</span><span class="sxs-lookup"><span data-stu-id="2589e-122">3</span></span>|<span data-ttu-id="2589e-123">Criptografia WEP.</span><span class="sxs-lookup"><span data-stu-id="2589e-123">WEP Encryption.</span></span>|
|<span data-ttu-id="2589e-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="2589e-124">wpa2Personal</span></span>|<span data-ttu-id="2589e-125">quatro</span><span class="sxs-lookup"><span data-stu-id="2589e-125">4</span></span>|<span data-ttu-id="2589e-126">WPA2-Pessoal.</span><span class="sxs-lookup"><span data-stu-id="2589e-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="2589e-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="2589e-127">wpa2Enterprise</span></span>|<span data-ttu-id="2589e-128">0,5</span><span class="sxs-lookup"><span data-stu-id="2589e-128">5</span></span>|<span data-ttu-id="2589e-129">WPA2-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="2589e-129">WPA2-Enterprise.</span></span> <span data-ttu-id="2589e-130">Deve usar o tipo WindowsWifiEnterpriseEAPConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="2589e-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





