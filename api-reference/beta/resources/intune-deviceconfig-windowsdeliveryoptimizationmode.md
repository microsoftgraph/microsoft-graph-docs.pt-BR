---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 71bc7e364ca18fefe9ebc5fa5ed75d5dac485a01
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411909"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="67fe5-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="67fe5-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="67fe5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67fe5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67fe5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67fe5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67fe5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67fe5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67fe5-107">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="67fe5-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="67fe5-108">Membros</span><span class="sxs-lookup"><span data-stu-id="67fe5-108">Members</span></span>
|<span data-ttu-id="67fe5-109">Membro</span><span class="sxs-lookup"><span data-stu-id="67fe5-109">Member</span></span>|<span data-ttu-id="67fe5-110">Valor</span><span class="sxs-lookup"><span data-stu-id="67fe5-110">Value</span></span>|<span data-ttu-id="67fe5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="67fe5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67fe5-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="67fe5-112">userDefined</span></span>|<span data-ttu-id="67fe5-113">,0</span><span class="sxs-lookup"><span data-stu-id="67fe5-113">0</span></span>|<span data-ttu-id="67fe5-114">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="67fe5-114">Allow the user to set.</span></span>|
|<span data-ttu-id="67fe5-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="67fe5-115">httpOnly</span></span>|<span data-ttu-id="67fe5-116">1</span><span class="sxs-lookup"><span data-stu-id="67fe5-116">1</span></span>|<span data-ttu-id="67fe5-117">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="67fe5-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="67fe5-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="67fe5-118">httpWithPeeringNat</span></span>|<span data-ttu-id="67fe5-119">duas</span><span class="sxs-lookup"><span data-stu-id="67fe5-119">2</span></span>|<span data-ttu-id="67fe5-120">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="67fe5-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="67fe5-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="67fe5-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="67fe5-122">3D</span><span class="sxs-lookup"><span data-stu-id="67fe5-122">3</span></span>|<span data-ttu-id="67fe5-123">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="67fe5-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="67fe5-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="67fe5-124">httpWithInternetPeering</span></span>|<span data-ttu-id="67fe5-125">4 </span><span class="sxs-lookup"><span data-stu-id="67fe5-125">4</span></span>|<span data-ttu-id="67fe5-126">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="67fe5-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="67fe5-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="67fe5-127">simpleDownload</span></span>|<span data-ttu-id="67fe5-128">99</span><span class="sxs-lookup"><span data-stu-id="67fe5-128">99</span></span>|<span data-ttu-id="67fe5-129">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="67fe5-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="67fe5-130">bypassmode</span><span class="sxs-lookup"><span data-stu-id="67fe5-130">bypassMode</span></span>|<span data-ttu-id="67fe5-131">100</span><span class="sxs-lookup"><span data-stu-id="67fe5-131">100</span></span>|<span data-ttu-id="67fe5-132">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="67fe5-132">Bypass mode.</span></span> <span data-ttu-id="67fe5-133">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="67fe5-133">Do not use Delivery Optimization and use BITS instead</span></span>|



