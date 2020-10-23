---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 719e315f8cccf52f98dfddb979d9f0fd5490dff8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692426"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="f18e4-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="f18e4-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="f18e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f18e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f18e4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f18e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f18e4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f18e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f18e4-107">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="f18e4-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="f18e4-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f18e4-108">Members</span></span>
|<span data-ttu-id="f18e4-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f18e4-109">Member</span></span>|<span data-ttu-id="f18e4-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f18e4-110">Value</span></span>|<span data-ttu-id="f18e4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f18e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f18e4-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="f18e4-112">userDefined</span></span>|<span data-ttu-id="f18e4-113">,0</span><span class="sxs-lookup"><span data-stu-id="f18e4-113">0</span></span>|<span data-ttu-id="f18e4-114">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="f18e4-114">Allow the user to set.</span></span>|
|<span data-ttu-id="f18e4-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="f18e4-115">httpOnly</span></span>|<span data-ttu-id="f18e4-116">1</span><span class="sxs-lookup"><span data-stu-id="f18e4-116">1</span></span>|<span data-ttu-id="f18e4-117">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="f18e4-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="f18e4-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="f18e4-118">httpWithPeeringNat</span></span>|<span data-ttu-id="f18e4-119">duas</span><span class="sxs-lookup"><span data-stu-id="f18e4-119">2</span></span>|<span data-ttu-id="f18e4-120">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="f18e4-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="f18e4-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="f18e4-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="f18e4-122">3D</span><span class="sxs-lookup"><span data-stu-id="f18e4-122">3</span></span>|<span data-ttu-id="f18e4-123">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="f18e4-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="f18e4-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="f18e4-124">httpWithInternetPeering</span></span>|<span data-ttu-id="f18e4-125">4 </span><span class="sxs-lookup"><span data-stu-id="f18e4-125">4</span></span>|<span data-ttu-id="f18e4-126">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="f18e4-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="f18e4-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="f18e4-127">simpleDownload</span></span>|<span data-ttu-id="f18e4-128">99</span><span class="sxs-lookup"><span data-stu-id="f18e4-128">99</span></span>|<span data-ttu-id="f18e4-129">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="f18e4-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="f18e4-130">bypassmode</span><span class="sxs-lookup"><span data-stu-id="f18e4-130">bypassMode</span></span>|<span data-ttu-id="f18e4-131">100</span><span class="sxs-lookup"><span data-stu-id="f18e4-131">100</span></span>|<span data-ttu-id="f18e4-132">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="f18e4-132">Bypass mode.</span></span> <span data-ttu-id="f18e4-133">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="f18e4-133">Do not use Delivery Optimization and use BITS instead</span></span>|





