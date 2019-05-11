---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e020b4f32cc9075acab6c783b4e9df3eb19a438b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944121"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="3cc12-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="3cc12-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="3cc12-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3cc12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cc12-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3cc12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cc12-106">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="3cc12-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="3cc12-107">Membros</span><span class="sxs-lookup"><span data-stu-id="3cc12-107">Members</span></span>
|<span data-ttu-id="3cc12-108">Membro</span><span class="sxs-lookup"><span data-stu-id="3cc12-108">Member</span></span>|<span data-ttu-id="3cc12-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3cc12-109">Value</span></span>|<span data-ttu-id="3cc12-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cc12-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cc12-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="3cc12-111">userDefined</span></span>|<span data-ttu-id="3cc12-112">,0</span><span class="sxs-lookup"><span data-stu-id="3cc12-112">0</span></span>|<span data-ttu-id="3cc12-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="3cc12-113">Allow the user to set.</span></span>|
|<span data-ttu-id="3cc12-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="3cc12-114">httpOnly</span></span>|<span data-ttu-id="3cc12-115">1</span><span class="sxs-lookup"><span data-stu-id="3cc12-115">1</span></span>|<span data-ttu-id="3cc12-116">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="3cc12-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="3cc12-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="3cc12-117">httpWithPeeringNat</span></span>|<span data-ttu-id="3cc12-118">duas</span><span class="sxs-lookup"><span data-stu-id="3cc12-118">2</span></span>|<span data-ttu-id="3cc12-119">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="3cc12-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="3cc12-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="3cc12-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="3cc12-121">3D</span><span class="sxs-lookup"><span data-stu-id="3cc12-121">3</span></span>|<span data-ttu-id="3cc12-122">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="3cc12-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="3cc12-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="3cc12-123">httpWithInternetPeering</span></span>|<span data-ttu-id="3cc12-124">quatro</span><span class="sxs-lookup"><span data-stu-id="3cc12-124">4</span></span>|<span data-ttu-id="3cc12-125">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="3cc12-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="3cc12-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="3cc12-126">simpleDownload</span></span>|<span data-ttu-id="3cc12-127">99</span><span class="sxs-lookup"><span data-stu-id="3cc12-127">99</span></span>|<span data-ttu-id="3cc12-128">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="3cc12-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="3cc12-129">bypassmode</span><span class="sxs-lookup"><span data-stu-id="3cc12-129">bypassMode</span></span>|<span data-ttu-id="3cc12-130">100</span><span class="sxs-lookup"><span data-stu-id="3cc12-130">100</span></span>|<span data-ttu-id="3cc12-131">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="3cc12-131">Bypass mode.</span></span> <span data-ttu-id="3cc12-132">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="3cc12-132">Do not use Delivery Optimization and use BITS instead</span></span>|




