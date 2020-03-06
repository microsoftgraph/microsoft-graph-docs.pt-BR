---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 869c902e8fc0b02fed1037d1d1273d8584ece9fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530371"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="0f655-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="0f655-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="0f655-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f655-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f655-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f655-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f655-106">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="0f655-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="0f655-107">Membros</span><span class="sxs-lookup"><span data-stu-id="0f655-107">Members</span></span>
|<span data-ttu-id="0f655-108">Membro</span><span class="sxs-lookup"><span data-stu-id="0f655-108">Member</span></span>|<span data-ttu-id="0f655-109">Valor</span><span class="sxs-lookup"><span data-stu-id="0f655-109">Value</span></span>|<span data-ttu-id="0f655-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f655-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f655-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="0f655-111">userDefined</span></span>|<span data-ttu-id="0f655-112">,0</span><span class="sxs-lookup"><span data-stu-id="0f655-112">0</span></span>|<span data-ttu-id="0f655-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="0f655-113">Allow the user to set.</span></span>|
|<span data-ttu-id="0f655-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="0f655-114">httpOnly</span></span>|<span data-ttu-id="0f655-115">1 </span><span class="sxs-lookup"><span data-stu-id="0f655-115">1</span></span>|<span data-ttu-id="0f655-116">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="0f655-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="0f655-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="0f655-117">httpWithPeeringNat</span></span>|<span data-ttu-id="0f655-118">2 </span><span class="sxs-lookup"><span data-stu-id="0f655-118">2</span></span>|<span data-ttu-id="0f655-119">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="0f655-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="0f655-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="0f655-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="0f655-121">3 </span><span class="sxs-lookup"><span data-stu-id="0f655-121">3</span></span>|<span data-ttu-id="0f655-122">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="0f655-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="0f655-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="0f655-123">httpWithInternetPeering</span></span>|<span data-ttu-id="0f655-124">4 </span><span class="sxs-lookup"><span data-stu-id="0f655-124">4</span></span>|<span data-ttu-id="0f655-125">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="0f655-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="0f655-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="0f655-126">simpleDownload</span></span>|<span data-ttu-id="0f655-127">99</span><span class="sxs-lookup"><span data-stu-id="0f655-127">99</span></span>|<span data-ttu-id="0f655-128">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="0f655-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="0f655-129">bypassmode</span><span class="sxs-lookup"><span data-stu-id="0f655-129">bypassMode</span></span>|<span data-ttu-id="0f655-130">100</span><span class="sxs-lookup"><span data-stu-id="0f655-130">100</span></span>|<span data-ttu-id="0f655-131">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="0f655-131">Bypass mode.</span></span> <span data-ttu-id="0f655-132">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="0f655-132">Do not use Delivery Optimization and use BITS instead</span></span>|




