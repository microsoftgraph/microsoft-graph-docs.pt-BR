---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 674dd699831afd0e733adb4d436cf8d42d35a0b6
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357252"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="44690-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="44690-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="44690-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44690-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44690-105">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="44690-105">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="44690-106">Membros</span><span class="sxs-lookup"><span data-stu-id="44690-106">Members</span></span>
|<span data-ttu-id="44690-107">Membro</span><span class="sxs-lookup"><span data-stu-id="44690-107">Member</span></span>|<span data-ttu-id="44690-108">Valor</span><span class="sxs-lookup"><span data-stu-id="44690-108">Value</span></span>|<span data-ttu-id="44690-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="44690-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44690-110">UserDefined</span><span class="sxs-lookup"><span data-stu-id="44690-110">userDefined</span></span>|<span data-ttu-id="44690-111">,0</span><span class="sxs-lookup"><span data-stu-id="44690-111">0</span></span>|<span data-ttu-id="44690-112">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="44690-112">Allow the user to set.</span></span>|
|<span data-ttu-id="44690-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="44690-113">httpOnly</span></span>|<span data-ttu-id="44690-114">1</span><span class="sxs-lookup"><span data-stu-id="44690-114">1</span></span>|<span data-ttu-id="44690-115">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="44690-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="44690-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="44690-116">httpWithPeeringNat</span></span>|<span data-ttu-id="44690-117">duas</span><span class="sxs-lookup"><span data-stu-id="44690-117">2</span></span>|<span data-ttu-id="44690-118">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="44690-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="44690-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="44690-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="44690-120">3D</span><span class="sxs-lookup"><span data-stu-id="44690-120">3</span></span>|<span data-ttu-id="44690-121">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="44690-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="44690-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="44690-122">httpWithInternetPeering</span></span>|<span data-ttu-id="44690-123">quatro</span><span class="sxs-lookup"><span data-stu-id="44690-123">4</span></span>|<span data-ttu-id="44690-124">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="44690-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="44690-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="44690-125">simpleDownload</span></span>|<span data-ttu-id="44690-126">99</span><span class="sxs-lookup"><span data-stu-id="44690-126">99</span></span>|<span data-ttu-id="44690-127">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="44690-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="44690-128">bypassmode</span><span class="sxs-lookup"><span data-stu-id="44690-128">bypassMode</span></span>|<span data-ttu-id="44690-129">100</span><span class="sxs-lookup"><span data-stu-id="44690-129">100</span></span>|<span data-ttu-id="44690-130">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="44690-130">Bypass mode.</span></span> <span data-ttu-id="44690-131">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="44690-131">Do not use Delivery Optimization and use BITS instead</span></span>|




