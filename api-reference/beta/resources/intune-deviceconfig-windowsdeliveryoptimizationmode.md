---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a41d359f77f0fd2a893236c9a4e952b321d003b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994080"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="3e5b2-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="3e5b2-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="3e5b2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3e5b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e5b2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e5b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e5b2-106">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="3e5b2-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="3e5b2-107">Membros</span><span class="sxs-lookup"><span data-stu-id="3e5b2-107">Members</span></span>
|<span data-ttu-id="3e5b2-108">Membro</span><span class="sxs-lookup"><span data-stu-id="3e5b2-108">Member</span></span>|<span data-ttu-id="3e5b2-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3e5b2-109">Value</span></span>|<span data-ttu-id="3e5b2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e5b2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e5b2-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="3e5b2-111">userDefined</span></span>|<span data-ttu-id="3e5b2-112">,0</span><span class="sxs-lookup"><span data-stu-id="3e5b2-112">0</span></span>|<span data-ttu-id="3e5b2-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="3e5b2-113">Allow the user to set.</span></span>|
|<span data-ttu-id="3e5b2-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="3e5b2-114">httpOnly</span></span>|<span data-ttu-id="3e5b2-115">1</span><span class="sxs-lookup"><span data-stu-id="3e5b2-115">1</span></span>|<span data-ttu-id="3e5b2-116">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="3e5b2-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="3e5b2-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="3e5b2-117">httpWithPeeringNat</span></span>|<span data-ttu-id="3e5b2-118">duas</span><span class="sxs-lookup"><span data-stu-id="3e5b2-118">2</span></span>|<span data-ttu-id="3e5b2-119">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="3e5b2-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="3e5b2-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="3e5b2-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="3e5b2-121">3D</span><span class="sxs-lookup"><span data-stu-id="3e5b2-121">3</span></span>|<span data-ttu-id="3e5b2-122">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="3e5b2-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="3e5b2-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="3e5b2-123">httpWithInternetPeering</span></span>|<span data-ttu-id="3e5b2-124">quatro</span><span class="sxs-lookup"><span data-stu-id="3e5b2-124">4</span></span>|<span data-ttu-id="3e5b2-125">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="3e5b2-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="3e5b2-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="3e5b2-126">simpleDownload</span></span>|<span data-ttu-id="3e5b2-127">99</span><span class="sxs-lookup"><span data-stu-id="3e5b2-127">99</span></span>|<span data-ttu-id="3e5b2-128">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="3e5b2-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="3e5b2-129">bypassmode</span><span class="sxs-lookup"><span data-stu-id="3e5b2-129">bypassMode</span></span>|<span data-ttu-id="3e5b2-130">100</span><span class="sxs-lookup"><span data-stu-id="3e5b2-130">100</span></span>|<span data-ttu-id="3e5b2-131">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="3e5b2-131">Bypass mode.</span></span> <span data-ttu-id="3e5b2-132">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="3e5b2-132">Do not use Delivery Optimization and use BITS instead</span></span>|





