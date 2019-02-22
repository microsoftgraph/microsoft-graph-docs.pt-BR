---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a4b0860e05d20ea480f9c91264033f7a9eb41a0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149165"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="a1366-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="a1366-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="a1366-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1366-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1366-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1366-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1366-106">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="a1366-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="a1366-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a1366-107">Members</span></span>
|<span data-ttu-id="a1366-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a1366-108">Member</span></span>|<span data-ttu-id="a1366-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a1366-109">Value</span></span>|<span data-ttu-id="a1366-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1366-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1366-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="a1366-111">userDefined</span></span>|<span data-ttu-id="a1366-112">,0</span><span class="sxs-lookup"><span data-stu-id="a1366-112">0</span></span>|<span data-ttu-id="a1366-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="a1366-113">Allow the user to set.</span></span>|
|<span data-ttu-id="a1366-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="a1366-114">httpOnly</span></span>|<span data-ttu-id="a1366-115">1</span><span class="sxs-lookup"><span data-stu-id="a1366-115">1</span></span>|<span data-ttu-id="a1366-116">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="a1366-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="a1366-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="a1366-117">httpWithPeeringNat</span></span>|<span data-ttu-id="a1366-118">duas</span><span class="sxs-lookup"><span data-stu-id="a1366-118">2</span></span>|<span data-ttu-id="a1366-119">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="a1366-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="a1366-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="a1366-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="a1366-121">3D</span><span class="sxs-lookup"><span data-stu-id="a1366-121">3</span></span>|<span data-ttu-id="a1366-122">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="a1366-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="a1366-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="a1366-123">httpWithInternetPeering</span></span>|<span data-ttu-id="a1366-124">quatro</span><span class="sxs-lookup"><span data-stu-id="a1366-124">4</span></span>|<span data-ttu-id="a1366-125">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="a1366-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="a1366-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="a1366-126">simpleDownload</span></span>|<span data-ttu-id="a1366-127">99</span><span class="sxs-lookup"><span data-stu-id="a1366-127">99</span></span>|<span data-ttu-id="a1366-128">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="a1366-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="a1366-129">bypassmode</span><span class="sxs-lookup"><span data-stu-id="a1366-129">bypassMode</span></span>|<span data-ttu-id="a1366-130">100</span><span class="sxs-lookup"><span data-stu-id="a1366-130">100</span></span>|<span data-ttu-id="a1366-131">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="a1366-131">Bypass mode.</span></span> <span data-ttu-id="a1366-132">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="a1366-132">Do not use Delivery Optimization and use BITS instead</span></span>|




