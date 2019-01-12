---
title: tipo de enum windows10VpnConnectionType
description: Tipos de conexão VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 77b9fb91f86cfa29b13e58c9a4c1a4dff768c3a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937870"
---
# <a name="windows10vpnconnectiontype-enum-type"></a><span data-ttu-id="c09da-103">tipo de enum windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c09da-103">windows10VpnConnectionType enum type</span></span>

> <span data-ttu-id="c09da-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c09da-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c09da-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c09da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c09da-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c09da-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c09da-107">Tipos de conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="c09da-107">VPN connection types.</span></span>
## <a name="members"></a><span data-ttu-id="c09da-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c09da-108">Members</span></span>
|<span data-ttu-id="c09da-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c09da-109">Member</span></span>|<span data-ttu-id="c09da-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c09da-110">Value</span></span>|<span data-ttu-id="c09da-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c09da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c09da-112">pulseSecure</span><span class="sxs-lookup"><span data-stu-id="c09da-112">pulseSecure</span></span>|<span data-ttu-id="c09da-113">0</span><span class="sxs-lookup"><span data-stu-id="c09da-113">0</span></span>|<span data-ttu-id="c09da-114">Pulso seguro.</span><span class="sxs-lookup"><span data-stu-id="c09da-114">Pulse Secure.</span></span>|
|<span data-ttu-id="c09da-115">f5EdgeClient</span><span class="sxs-lookup"><span data-stu-id="c09da-115">f5EdgeClient</span></span>|<span data-ttu-id="c09da-116">1</span><span class="sxs-lookup"><span data-stu-id="c09da-116">1</span></span>|<span data-ttu-id="c09da-117">F5 Cliente de borda.</span><span class="sxs-lookup"><span data-stu-id="c09da-117">F5 Edge Client.</span></span>|
|<span data-ttu-id="c09da-118">dellSonicWallMobileConnect</span><span class="sxs-lookup"><span data-stu-id="c09da-118">dellSonicWallMobileConnect</span></span>|<span data-ttu-id="c09da-119">2</span><span class="sxs-lookup"><span data-stu-id="c09da-119">2</span></span>|<span data-ttu-id="c09da-120">Conexão do Dell SonicWALL Mobile.</span><span class="sxs-lookup"><span data-stu-id="c09da-120">Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="c09da-121">checkPointCapsuleVpn</span><span class="sxs-lookup"><span data-stu-id="c09da-121">checkPointCapsuleVpn</span></span>|<span data-ttu-id="c09da-122">3</span><span class="sxs-lookup"><span data-stu-id="c09da-122">3</span></span>|<span data-ttu-id="c09da-123">Verifique o ponto Cápsula VPN.</span><span class="sxs-lookup"><span data-stu-id="c09da-123">Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="c09da-124">automatic</span><span class="sxs-lookup"><span data-stu-id="c09da-124">automatic</span></span>|<span data-ttu-id="c09da-125">4</span><span class="sxs-lookup"><span data-stu-id="c09da-125">4</span></span>|<span data-ttu-id="c09da-126">Automático.</span><span class="sxs-lookup"><span data-stu-id="c09da-126">Automatic.</span></span>|
|<span data-ttu-id="c09da-127">ikEv2</span><span class="sxs-lookup"><span data-stu-id="c09da-127">ikEv2</span></span>|<span data-ttu-id="c09da-128">5</span><span class="sxs-lookup"><span data-stu-id="c09da-128">5</span></span>|<span data-ttu-id="c09da-129">IKEv2.</span><span class="sxs-lookup"><span data-stu-id="c09da-129">IKEv2.</span></span>|
|<span data-ttu-id="c09da-130">L2TP</span><span class="sxs-lookup"><span data-stu-id="c09da-130">l2tp</span></span>|<span data-ttu-id="c09da-131">6</span><span class="sxs-lookup"><span data-stu-id="c09da-131">6</span></span>|<span data-ttu-id="c09da-132">L2TP.</span><span class="sxs-lookup"><span data-stu-id="c09da-132">L2TP.</span></span>|
|<span data-ttu-id="c09da-133">PPTP</span><span class="sxs-lookup"><span data-stu-id="c09da-133">pptp</span></span>|<span data-ttu-id="c09da-134">7</span><span class="sxs-lookup"><span data-stu-id="c09da-134">7</span></span>|<span data-ttu-id="c09da-135">PPTP.</span><span class="sxs-lookup"><span data-stu-id="c09da-135">PPTP.</span></span>|
|<span data-ttu-id="c09da-136">Citrix</span><span class="sxs-lookup"><span data-stu-id="c09da-136">citrix</span></span>|<span data-ttu-id="c09da-137">8</span><span class="sxs-lookup"><span data-stu-id="c09da-137">8</span></span>|<span data-ttu-id="c09da-138">Citrix.</span><span class="sxs-lookup"><span data-stu-id="c09da-138">Citrix.</span></span>|
|<span data-ttu-id="c09da-139">paloAltoGlobalProtect</span><span class="sxs-lookup"><span data-stu-id="c09da-139">paloAltoGlobalProtect</span></span>|<span data-ttu-id="c09da-140">9</span><span class="sxs-lookup"><span data-stu-id="c09da-140">9</span></span>|<span data-ttu-id="c09da-141">GlobalProtect do Palo Alto redes.</span><span class="sxs-lookup"><span data-stu-id="c09da-141">Palo Alto Networks GlobalProtect.</span></span>|





