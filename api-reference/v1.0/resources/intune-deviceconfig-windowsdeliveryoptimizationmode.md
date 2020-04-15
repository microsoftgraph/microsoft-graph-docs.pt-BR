---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9be3f6861076bed1ef2e6d45336d975c07cba576
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451484"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="5ee58-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="5ee58-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="5ee58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ee58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ee58-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ee58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ee58-106">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="5ee58-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="5ee58-107">Membros</span><span class="sxs-lookup"><span data-stu-id="5ee58-107">Members</span></span>
|<span data-ttu-id="5ee58-108">Membro</span><span class="sxs-lookup"><span data-stu-id="5ee58-108">Member</span></span>|<span data-ttu-id="5ee58-109">Valor</span><span class="sxs-lookup"><span data-stu-id="5ee58-109">Value</span></span>|<span data-ttu-id="5ee58-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ee58-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ee58-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="5ee58-111">userDefined</span></span>|<span data-ttu-id="5ee58-112">,0</span><span class="sxs-lookup"><span data-stu-id="5ee58-112">0</span></span>|<span data-ttu-id="5ee58-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="5ee58-113">Allow the user to set.</span></span>|
|<span data-ttu-id="5ee58-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="5ee58-114">httpOnly</span></span>|<span data-ttu-id="5ee58-115">1</span><span class="sxs-lookup"><span data-stu-id="5ee58-115">1</span></span>|<span data-ttu-id="5ee58-116">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="5ee58-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="5ee58-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="5ee58-117">httpWithPeeringNat</span></span>|<span data-ttu-id="5ee58-118">duas</span><span class="sxs-lookup"><span data-stu-id="5ee58-118">2</span></span>|<span data-ttu-id="5ee58-119">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="5ee58-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="5ee58-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="5ee58-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="5ee58-121">3D</span><span class="sxs-lookup"><span data-stu-id="5ee58-121">3</span></span>|<span data-ttu-id="5ee58-122">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="5ee58-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="5ee58-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="5ee58-123">httpWithInternetPeering</span></span>|<span data-ttu-id="5ee58-124">4 </span><span class="sxs-lookup"><span data-stu-id="5ee58-124">4</span></span>|<span data-ttu-id="5ee58-125">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="5ee58-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="5ee58-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="5ee58-126">simpleDownload</span></span>|<span data-ttu-id="5ee58-127">99</span><span class="sxs-lookup"><span data-stu-id="5ee58-127">99</span></span>|<span data-ttu-id="5ee58-128">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="5ee58-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="5ee58-129">bypassmode</span><span class="sxs-lookup"><span data-stu-id="5ee58-129">bypassMode</span></span>|<span data-ttu-id="5ee58-130">100</span><span class="sxs-lookup"><span data-stu-id="5ee58-130">100</span></span>|<span data-ttu-id="5ee58-131">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="5ee58-131">Bypass mode.</span></span> <span data-ttu-id="5ee58-132">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="5ee58-132">Do not use Delivery Optimization and use BITS instead</span></span>|







