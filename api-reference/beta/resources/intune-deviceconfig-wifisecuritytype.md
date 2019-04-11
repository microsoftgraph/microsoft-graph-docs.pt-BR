---
title: tipo de enumeração à
description: Tipos de segurança Wi-Fi.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9144a5761691b0a50e40370b1f4d2d08967f2c28
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780004"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="b2583-103">tipo de enumeração à</span><span class="sxs-lookup"><span data-stu-id="b2583-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="b2583-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2583-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2583-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2583-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2583-106">Tipos de segurança Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b2583-106">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="b2583-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b2583-107">Members</span></span>
|<span data-ttu-id="b2583-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b2583-108">Member</span></span>|<span data-ttu-id="b2583-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b2583-109">Value</span></span>|<span data-ttu-id="b2583-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2583-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2583-111">Abre</span><span class="sxs-lookup"><span data-stu-id="b2583-111">open</span></span>|<span data-ttu-id="b2583-112">,0</span><span class="sxs-lookup"><span data-stu-id="b2583-112">0</span></span>|<span data-ttu-id="b2583-113">Abrir (sem autenticação).</span><span class="sxs-lookup"><span data-stu-id="b2583-113">Open (No Authentication).</span></span>|
|<span data-ttu-id="b2583-114">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="b2583-114">wpaPersonal</span></span>|<span data-ttu-id="b2583-115">1</span><span class="sxs-lookup"><span data-stu-id="b2583-115">1</span></span>|<span data-ttu-id="b2583-116">WPA-pessoal.</span><span class="sxs-lookup"><span data-stu-id="b2583-116">WPA-Personal.</span></span>|
|<span data-ttu-id="b2583-117">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="b2583-117">wpaEnterprise</span></span>|<span data-ttu-id="b2583-118">duas</span><span class="sxs-lookup"><span data-stu-id="b2583-118">2</span></span>|<span data-ttu-id="b2583-119">WPA-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="b2583-119">WPA-Enterprise.</span></span> <span data-ttu-id="b2583-120">Deve usar o tipo IOSEnterpriseWifiConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="b2583-120">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="b2583-121">Deixa</span><span class="sxs-lookup"><span data-stu-id="b2583-121">wep</span></span>|<span data-ttu-id="b2583-122">3D</span><span class="sxs-lookup"><span data-stu-id="b2583-122">3</span></span>|<span data-ttu-id="b2583-123">Criptografia WEP.</span><span class="sxs-lookup"><span data-stu-id="b2583-123">WEP Encryption.</span></span>|
|<span data-ttu-id="b2583-124">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="b2583-124">wpa2Personal</span></span>|<span data-ttu-id="b2583-125">quatro</span><span class="sxs-lookup"><span data-stu-id="b2583-125">4</span></span>|<span data-ttu-id="b2583-126">WPA2-Pessoal.</span><span class="sxs-lookup"><span data-stu-id="b2583-126">WPA2-Personal.</span></span>|
|<span data-ttu-id="b2583-127">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="b2583-127">wpa2Enterprise</span></span>|<span data-ttu-id="b2583-128">0,5</span><span class="sxs-lookup"><span data-stu-id="b2583-128">5</span></span>|<span data-ttu-id="b2583-129">WPA2-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="b2583-129">WPA2-Enterprise.</span></span> <span data-ttu-id="b2583-130">Deve usar o tipo WindowsWifiEnterpriseEAPConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="b2583-130">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





