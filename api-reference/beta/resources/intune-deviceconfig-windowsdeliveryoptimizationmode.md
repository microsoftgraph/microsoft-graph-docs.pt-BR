---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 66ea4d13059cb9d3333c958481e711e5cd49b416
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529093"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="6819f-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="6819f-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="6819f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6819f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6819f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6819f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6819f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6819f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6819f-107">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="6819f-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="6819f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6819f-108">Members</span></span>
|<span data-ttu-id="6819f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6819f-109">Member</span></span>|<span data-ttu-id="6819f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6819f-110">Value</span></span>|<span data-ttu-id="6819f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6819f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6819f-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="6819f-112">userDefined</span></span>|<span data-ttu-id="6819f-113">,0</span><span class="sxs-lookup"><span data-stu-id="6819f-113">0</span></span>|<span data-ttu-id="6819f-114">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="6819f-114">Allow the user to set.</span></span>|
|<span data-ttu-id="6819f-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="6819f-115">httpOnly</span></span>|<span data-ttu-id="6819f-116">1 </span><span class="sxs-lookup"><span data-stu-id="6819f-116">1</span></span>|<span data-ttu-id="6819f-117">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="6819f-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="6819f-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="6819f-118">httpWithPeeringNat</span></span>|<span data-ttu-id="6819f-119">2 </span><span class="sxs-lookup"><span data-stu-id="6819f-119">2</span></span>|<span data-ttu-id="6819f-120">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="6819f-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="6819f-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="6819f-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="6819f-122">3 </span><span class="sxs-lookup"><span data-stu-id="6819f-122">3</span></span>|<span data-ttu-id="6819f-123">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="6819f-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="6819f-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="6819f-124">httpWithInternetPeering</span></span>|<span data-ttu-id="6819f-125">4 </span><span class="sxs-lookup"><span data-stu-id="6819f-125">4</span></span>|<span data-ttu-id="6819f-126">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="6819f-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="6819f-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="6819f-127">simpleDownload</span></span>|<span data-ttu-id="6819f-128">99</span><span class="sxs-lookup"><span data-stu-id="6819f-128">99</span></span>|<span data-ttu-id="6819f-129">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="6819f-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="6819f-130">bypassmode</span><span class="sxs-lookup"><span data-stu-id="6819f-130">bypassMode</span></span>|<span data-ttu-id="6819f-131">100</span><span class="sxs-lookup"><span data-stu-id="6819f-131">100</span></span>|<span data-ttu-id="6819f-132">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="6819f-132">Bypass mode.</span></span> <span data-ttu-id="6819f-133">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="6819f-133">Do not use Delivery Optimization and use BITS instead</span></span>|



