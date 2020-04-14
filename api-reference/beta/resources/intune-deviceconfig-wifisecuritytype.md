---
title: tipo de enumeração à
description: Tipos de segurança Wi-Fi.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 24fb0361bfbf8bc12c62f232d08c54eca033b915
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466320"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="4e513-103">tipo de enumeração à</span><span class="sxs-lookup"><span data-stu-id="4e513-103">wiFiSecurityType enum type</span></span>

<span data-ttu-id="4e513-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e513-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e513-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4e513-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e513-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e513-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e513-107">Tipos de segurança Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="4e513-107">Wi-Fi Security Types.</span></span>

## <a name="members"></a><span data-ttu-id="4e513-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4e513-108">Members</span></span>
|<span data-ttu-id="4e513-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4e513-109">Member</span></span>|<span data-ttu-id="4e513-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4e513-110">Value</span></span>|<span data-ttu-id="4e513-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e513-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e513-112">Abre</span><span class="sxs-lookup"><span data-stu-id="4e513-112">open</span></span>|<span data-ttu-id="4e513-113">,0</span><span class="sxs-lookup"><span data-stu-id="4e513-113">0</span></span>|<span data-ttu-id="4e513-114">Abrir (sem autenticação).</span><span class="sxs-lookup"><span data-stu-id="4e513-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="4e513-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="4e513-115">wpaPersonal</span></span>|<span data-ttu-id="4e513-116">1</span><span class="sxs-lookup"><span data-stu-id="4e513-116">1</span></span>|<span data-ttu-id="4e513-117">WPA-pessoal.</span><span class="sxs-lookup"><span data-stu-id="4e513-117">WPA-Personal.</span></span>|
|<span data-ttu-id="4e513-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="4e513-118">wpaEnterprise</span></span>|<span data-ttu-id="4e513-119">duas</span><span class="sxs-lookup"><span data-stu-id="4e513-119">2</span></span>|<span data-ttu-id="4e513-120">WPA-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="4e513-120">WPA-Enterprise.</span></span> <span data-ttu-id="4e513-121">Deve usar o tipo IOSEnterpriseWifiConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="4e513-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="4e513-122">Deixa</span><span class="sxs-lookup"><span data-stu-id="4e513-122">wep</span></span>|<span data-ttu-id="4e513-123">3D</span><span class="sxs-lookup"><span data-stu-id="4e513-123">3</span></span>|<span data-ttu-id="4e513-124">Criptografia WEP.</span><span class="sxs-lookup"><span data-stu-id="4e513-124">WEP Encryption.</span></span>|
|<span data-ttu-id="4e513-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="4e513-125">wpa2Personal</span></span>|<span data-ttu-id="4e513-126">4 </span><span class="sxs-lookup"><span data-stu-id="4e513-126">4</span></span>|<span data-ttu-id="4e513-127">WPA2-Pessoal.</span><span class="sxs-lookup"><span data-stu-id="4e513-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="4e513-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="4e513-128">wpa2Enterprise</span></span>|<span data-ttu-id="4e513-129">5 </span><span class="sxs-lookup"><span data-stu-id="4e513-129">5</span></span>|<span data-ttu-id="4e513-130">WPA2-Enterprise.</span><span class="sxs-lookup"><span data-stu-id="4e513-130">WPA2-Enterprise.</span></span> <span data-ttu-id="4e513-131">Deve usar o tipo WindowsWifiEnterpriseEAPConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="4e513-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|



