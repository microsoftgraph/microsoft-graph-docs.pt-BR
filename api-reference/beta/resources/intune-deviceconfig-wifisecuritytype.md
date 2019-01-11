---
title: tipo de enum wiFiSecurityType
description: Tipos de segurança Wi-Fi.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 90290b9b47154b95aca81d931fa66e7984688db1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839918"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="c0f5d-103">tipo de enum wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="c0f5d-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="c0f5d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c0f5d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0f5d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c0f5d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0f5d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c0f5d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0f5d-107">Tipos de segurança Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="c0f5d-107">Wi-Fi Security Types.</span></span>
## <a name="members"></a><span data-ttu-id="c0f5d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c0f5d-108">Members</span></span>
|<span data-ttu-id="c0f5d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c0f5d-109">Member</span></span>|<span data-ttu-id="c0f5d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c0f5d-110">Value</span></span>|<span data-ttu-id="c0f5d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0f5d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0f5d-112">Abrir</span><span class="sxs-lookup"><span data-stu-id="c0f5d-112">open</span></span>|<span data-ttu-id="c0f5d-113">0</span><span class="sxs-lookup"><span data-stu-id="c0f5d-113">0</span></span>|<span data-ttu-id="c0f5d-114">Abra (nenhuma autenticação).</span><span class="sxs-lookup"><span data-stu-id="c0f5d-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="c0f5d-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="c0f5d-115">wpaPersonal</span></span>|<span data-ttu-id="c0f5d-116">1</span><span class="sxs-lookup"><span data-stu-id="c0f5d-116">1</span></span>|<span data-ttu-id="c0f5d-117">WPA-Pessoal.</span><span class="sxs-lookup"><span data-stu-id="c0f5d-117">WPA-Personal.</span></span>|
|<span data-ttu-id="c0f5d-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="c0f5d-118">wpaEnterprise</span></span>|<span data-ttu-id="c0f5d-119">2</span><span class="sxs-lookup"><span data-stu-id="c0f5d-119">2</span></span>|<span data-ttu-id="c0f5d-120">WPA-Empresa.</span><span class="sxs-lookup"><span data-stu-id="c0f5d-120">WPA-Enterprise.</span></span> <span data-ttu-id="c0f5d-121">Deve usar o tipo de IOSEnterpriseWifiConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="c0f5d-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="c0f5d-122">WEP</span><span class="sxs-lookup"><span data-stu-id="c0f5d-122">wep</span></span>|<span data-ttu-id="c0f5d-123">3</span><span class="sxs-lookup"><span data-stu-id="c0f5d-123">3</span></span>|<span data-ttu-id="c0f5d-124">Criptografia WEP.</span><span class="sxs-lookup"><span data-stu-id="c0f5d-124">WEP Encryption.</span></span>|
|<span data-ttu-id="c0f5d-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="c0f5d-125">wpa2Personal</span></span>|<span data-ttu-id="c0f5d-126">4</span><span class="sxs-lookup"><span data-stu-id="c0f5d-126">4</span></span>|<span data-ttu-id="c0f5d-127">WPA2-pessoal.</span><span class="sxs-lookup"><span data-stu-id="c0f5d-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="c0f5d-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="c0f5d-128">wpa2Enterprise</span></span>|<span data-ttu-id="c0f5d-129">5</span><span class="sxs-lookup"><span data-stu-id="c0f5d-129">5</span></span>|<span data-ttu-id="c0f5d-130">WPA2-Empresa.</span><span class="sxs-lookup"><span data-stu-id="c0f5d-130">WPA2-Enterprise.</span></span> <span data-ttu-id="c0f5d-131">Deve usar o tipo de WindowsWifiEnterpriseEAPConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="c0f5d-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





