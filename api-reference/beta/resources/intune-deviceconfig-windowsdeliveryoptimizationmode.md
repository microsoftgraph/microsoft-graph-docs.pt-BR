---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: faf70d8cb1122b09d5fcc6a5dcbf221cf3a6991c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786513"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="3c9d3-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="3c9d3-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="3c9d3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c9d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c9d3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c9d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c9d3-106">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="3c9d3-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="3c9d3-107">Membros</span><span class="sxs-lookup"><span data-stu-id="3c9d3-107">Members</span></span>
|<span data-ttu-id="3c9d3-108">Membro</span><span class="sxs-lookup"><span data-stu-id="3c9d3-108">Member</span></span>|<span data-ttu-id="3c9d3-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3c9d3-109">Value</span></span>|<span data-ttu-id="3c9d3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c9d3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c9d3-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="3c9d3-111">userDefined</span></span>|<span data-ttu-id="3c9d3-112">,0</span><span class="sxs-lookup"><span data-stu-id="3c9d3-112">0</span></span>|<span data-ttu-id="3c9d3-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="3c9d3-113">Allow the user to set.</span></span>|
|<span data-ttu-id="3c9d3-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="3c9d3-114">httpOnly</span></span>|<span data-ttu-id="3c9d3-115">1</span><span class="sxs-lookup"><span data-stu-id="3c9d3-115">1</span></span>|<span data-ttu-id="3c9d3-116">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="3c9d3-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="3c9d3-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="3c9d3-117">httpWithPeeringNat</span></span>|<span data-ttu-id="3c9d3-118">duas</span><span class="sxs-lookup"><span data-stu-id="3c9d3-118">2</span></span>|<span data-ttu-id="3c9d3-119">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="3c9d3-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="3c9d3-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="3c9d3-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="3c9d3-121">3D</span><span class="sxs-lookup"><span data-stu-id="3c9d3-121">3</span></span>|<span data-ttu-id="3c9d3-122">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="3c9d3-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="3c9d3-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="3c9d3-123">httpWithInternetPeering</span></span>|<span data-ttu-id="3c9d3-124">4 </span><span class="sxs-lookup"><span data-stu-id="3c9d3-124">4</span></span>|<span data-ttu-id="3c9d3-125">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="3c9d3-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="3c9d3-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="3c9d3-126">simpleDownload</span></span>|<span data-ttu-id="3c9d3-127">99</span><span class="sxs-lookup"><span data-stu-id="3c9d3-127">99</span></span>|<span data-ttu-id="3c9d3-128">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="3c9d3-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="3c9d3-129">bypassmode</span><span class="sxs-lookup"><span data-stu-id="3c9d3-129">bypassMode</span></span>|<span data-ttu-id="3c9d3-130">100</span><span class="sxs-lookup"><span data-stu-id="3c9d3-130">100</span></span>|<span data-ttu-id="3c9d3-131">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="3c9d3-131">Bypass mode.</span></span> <span data-ttu-id="3c9d3-132">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="3c9d3-132">Do not use Delivery Optimization and use BITS instead</span></span>|



