---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3872b7c09c8934e95725565b83cc195d9b9d8da5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785290"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="e205c-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="e205c-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="e205c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e205c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e205c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e205c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e205c-106">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="e205c-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="e205c-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e205c-107">Members</span></span>
|<span data-ttu-id="e205c-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e205c-108">Member</span></span>|<span data-ttu-id="e205c-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e205c-109">Value</span></span>|<span data-ttu-id="e205c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e205c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e205c-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="e205c-111">userDefined</span></span>|<span data-ttu-id="e205c-112">,0</span><span class="sxs-lookup"><span data-stu-id="e205c-112">0</span></span>|<span data-ttu-id="e205c-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="e205c-113">Allow the user to set.</span></span>|
|<span data-ttu-id="e205c-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="e205c-114">httpOnly</span></span>|<span data-ttu-id="e205c-115">1</span><span class="sxs-lookup"><span data-stu-id="e205c-115">1</span></span>|<span data-ttu-id="e205c-116">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="e205c-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="e205c-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="e205c-117">httpWithPeeringNat</span></span>|<span data-ttu-id="e205c-118">duas</span><span class="sxs-lookup"><span data-stu-id="e205c-118">2</span></span>|<span data-ttu-id="e205c-119">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="e205c-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="e205c-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="e205c-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="e205c-121">3D</span><span class="sxs-lookup"><span data-stu-id="e205c-121">3</span></span>|<span data-ttu-id="e205c-122">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="e205c-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="e205c-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="e205c-123">httpWithInternetPeering</span></span>|<span data-ttu-id="e205c-124">quatro</span><span class="sxs-lookup"><span data-stu-id="e205c-124">4</span></span>|<span data-ttu-id="e205c-125">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="e205c-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="e205c-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="e205c-126">simpleDownload</span></span>|<span data-ttu-id="e205c-127">99</span><span class="sxs-lookup"><span data-stu-id="e205c-127">99</span></span>|<span data-ttu-id="e205c-128">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="e205c-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="e205c-129">bypassmode</span><span class="sxs-lookup"><span data-stu-id="e205c-129">bypassMode</span></span>|<span data-ttu-id="e205c-130">100</span><span class="sxs-lookup"><span data-stu-id="e205c-130">100</span></span>|<span data-ttu-id="e205c-131">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="e205c-131">Bypass mode.</span></span> <span data-ttu-id="e205c-132">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="e205c-132">Do not use Delivery Optimization and use BITS instead</span></span>|





