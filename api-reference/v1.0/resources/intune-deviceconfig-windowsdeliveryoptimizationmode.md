---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: eabc09c8eba7267041eaf5bb318d6269373f48b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091548"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="4b8b8-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="4b8b8-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="4b8b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b8b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b8b8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b8b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b8b8-106">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="4b8b8-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="4b8b8-107">Membros</span><span class="sxs-lookup"><span data-stu-id="4b8b8-107">Members</span></span>
|<span data-ttu-id="4b8b8-108">Membro</span><span class="sxs-lookup"><span data-stu-id="4b8b8-108">Member</span></span>|<span data-ttu-id="4b8b8-109">Valor</span><span class="sxs-lookup"><span data-stu-id="4b8b8-109">Value</span></span>|<span data-ttu-id="4b8b8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b8b8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b8b8-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="4b8b8-111">userDefined</span></span>|<span data-ttu-id="4b8b8-112">,0</span><span class="sxs-lookup"><span data-stu-id="4b8b8-112">0</span></span>|<span data-ttu-id="4b8b8-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="4b8b8-113">Allow the user to set.</span></span>|
|<span data-ttu-id="4b8b8-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="4b8b8-114">httpOnly</span></span>|<span data-ttu-id="4b8b8-115">1 </span><span class="sxs-lookup"><span data-stu-id="4b8b8-115">1</span></span>|<span data-ttu-id="4b8b8-116">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="4b8b8-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="4b8b8-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="4b8b8-117">httpWithPeeringNat</span></span>|<span data-ttu-id="4b8b8-118">2 </span><span class="sxs-lookup"><span data-stu-id="4b8b8-118">2</span></span>|<span data-ttu-id="4b8b8-119">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="4b8b8-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="4b8b8-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="4b8b8-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="4b8b8-121">3D</span><span class="sxs-lookup"><span data-stu-id="4b8b8-121">3</span></span>|<span data-ttu-id="4b8b8-122">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="4b8b8-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="4b8b8-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="4b8b8-123">httpWithInternetPeering</span></span>|<span data-ttu-id="4b8b8-124">4 </span><span class="sxs-lookup"><span data-stu-id="4b8b8-124">4</span></span>|<span data-ttu-id="4b8b8-125">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="4b8b8-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="4b8b8-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="4b8b8-126">simpleDownload</span></span>|<span data-ttu-id="4b8b8-127">99</span><span class="sxs-lookup"><span data-stu-id="4b8b8-127">99</span></span>|<span data-ttu-id="4b8b8-128">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="4b8b8-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="4b8b8-129">bypassmode</span><span class="sxs-lookup"><span data-stu-id="4b8b8-129">bypassMode</span></span>|<span data-ttu-id="4b8b8-130">100</span><span class="sxs-lookup"><span data-stu-id="4b8b8-130">100</span></span>|<span data-ttu-id="4b8b8-131">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="4b8b8-131">Bypass mode.</span></span> <span data-ttu-id="4b8b8-132">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="4b8b8-132">Do not use Delivery Optimization and use BITS instead</span></span>|









