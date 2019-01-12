---
title: tipo de enum wiFiSecurityType
description: Tipos de segurança Wi-Fi.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6ddadaa31febaea08050ad49ffa540de53ff4819
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920216"
---
# <a name="wifisecuritytype-enum-type"></a><span data-ttu-id="61c97-103">tipo de enum wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="61c97-103">wiFiSecurityType enum type</span></span>

> <span data-ttu-id="61c97-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="61c97-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61c97-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="61c97-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61c97-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="61c97-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61c97-107">Tipos de segurança Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="61c97-107">Wi-Fi Security Types.</span></span>
## <a name="members"></a><span data-ttu-id="61c97-108">Membros</span><span class="sxs-lookup"><span data-stu-id="61c97-108">Members</span></span>
|<span data-ttu-id="61c97-109">Membro</span><span class="sxs-lookup"><span data-stu-id="61c97-109">Member</span></span>|<span data-ttu-id="61c97-110">Valor</span><span class="sxs-lookup"><span data-stu-id="61c97-110">Value</span></span>|<span data-ttu-id="61c97-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="61c97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61c97-112">Abrir</span><span class="sxs-lookup"><span data-stu-id="61c97-112">open</span></span>|<span data-ttu-id="61c97-113">0</span><span class="sxs-lookup"><span data-stu-id="61c97-113">0</span></span>|<span data-ttu-id="61c97-114">Abra (nenhuma autenticação).</span><span class="sxs-lookup"><span data-stu-id="61c97-114">Open (No Authentication).</span></span>|
|<span data-ttu-id="61c97-115">wpaPersonal</span><span class="sxs-lookup"><span data-stu-id="61c97-115">wpaPersonal</span></span>|<span data-ttu-id="61c97-116">1</span><span class="sxs-lookup"><span data-stu-id="61c97-116">1</span></span>|<span data-ttu-id="61c97-117">WPA-Pessoal.</span><span class="sxs-lookup"><span data-stu-id="61c97-117">WPA-Personal.</span></span>|
|<span data-ttu-id="61c97-118">wpaEnterprise</span><span class="sxs-lookup"><span data-stu-id="61c97-118">wpaEnterprise</span></span>|<span data-ttu-id="61c97-119">2</span><span class="sxs-lookup"><span data-stu-id="61c97-119">2</span></span>|<span data-ttu-id="61c97-120">WPA-Empresa.</span><span class="sxs-lookup"><span data-stu-id="61c97-120">WPA-Enterprise.</span></span> <span data-ttu-id="61c97-121">Deve usar o tipo de IOSEnterpriseWifiConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="61c97-121">Must use IOSEnterpriseWifiConfiguration type to configure enterprise options.</span></span>|
|<span data-ttu-id="61c97-122">WEP</span><span class="sxs-lookup"><span data-stu-id="61c97-122">wep</span></span>|<span data-ttu-id="61c97-123">3</span><span class="sxs-lookup"><span data-stu-id="61c97-123">3</span></span>|<span data-ttu-id="61c97-124">Criptografia WEP.</span><span class="sxs-lookup"><span data-stu-id="61c97-124">WEP Encryption.</span></span>|
|<span data-ttu-id="61c97-125">wpa2Personal</span><span class="sxs-lookup"><span data-stu-id="61c97-125">wpa2Personal</span></span>|<span data-ttu-id="61c97-126">4</span><span class="sxs-lookup"><span data-stu-id="61c97-126">4</span></span>|<span data-ttu-id="61c97-127">WPA2-pessoal.</span><span class="sxs-lookup"><span data-stu-id="61c97-127">WPA2-Personal.</span></span>|
|<span data-ttu-id="61c97-128">wpa2Enterprise</span><span class="sxs-lookup"><span data-stu-id="61c97-128">wpa2Enterprise</span></span>|<span data-ttu-id="61c97-129">5</span><span class="sxs-lookup"><span data-stu-id="61c97-129">5</span></span>|<span data-ttu-id="61c97-130">WPA2-Empresa.</span><span class="sxs-lookup"><span data-stu-id="61c97-130">WPA2-Enterprise.</span></span> <span data-ttu-id="61c97-131">Deve usar o tipo de WindowsWifiEnterpriseEAPConfiguration para configurar opções da empresa.</span><span class="sxs-lookup"><span data-stu-id="61c97-131">Must use WindowsWifiEnterpriseEAPConfiguration type to configure enterprise options.</span></span>|





