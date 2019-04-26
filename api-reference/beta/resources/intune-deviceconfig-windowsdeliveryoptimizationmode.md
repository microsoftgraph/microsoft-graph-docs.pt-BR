---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3872b7c09c8934e95725565b83cc195d9b9d8da5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554146"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="d94e7-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="d94e7-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="d94e7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d94e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d94e7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d94e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d94e7-106">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="d94e7-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="d94e7-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d94e7-107">Members</span></span>
|<span data-ttu-id="d94e7-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d94e7-108">Member</span></span>|<span data-ttu-id="d94e7-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d94e7-109">Value</span></span>|<span data-ttu-id="d94e7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d94e7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d94e7-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="d94e7-111">userDefined</span></span>|<span data-ttu-id="d94e7-112">,0</span><span class="sxs-lookup"><span data-stu-id="d94e7-112">0</span></span>|<span data-ttu-id="d94e7-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="d94e7-113">Allow the user to set.</span></span>|
|<span data-ttu-id="d94e7-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="d94e7-114">httpOnly</span></span>|<span data-ttu-id="d94e7-115">1 </span><span class="sxs-lookup"><span data-stu-id="d94e7-115">1</span></span>|<span data-ttu-id="d94e7-116">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="d94e7-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="d94e7-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="d94e7-117">httpWithPeeringNat</span></span>|<span data-ttu-id="d94e7-118">2 </span><span class="sxs-lookup"><span data-stu-id="d94e7-118">2</span></span>|<span data-ttu-id="d94e7-119">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="d94e7-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="d94e7-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="d94e7-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="d94e7-121">3 </span><span class="sxs-lookup"><span data-stu-id="d94e7-121">3</span></span>|<span data-ttu-id="d94e7-122">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="d94e7-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="d94e7-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="d94e7-123">httpWithInternetPeering</span></span>|<span data-ttu-id="d94e7-124">4 </span><span class="sxs-lookup"><span data-stu-id="d94e7-124">4</span></span>|<span data-ttu-id="d94e7-125">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="d94e7-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="d94e7-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="d94e7-126">simpleDownload</span></span>|<span data-ttu-id="d94e7-127">99</span><span class="sxs-lookup"><span data-stu-id="d94e7-127">99</span></span>|<span data-ttu-id="d94e7-128">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="d94e7-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="d94e7-129">bypassmode</span><span class="sxs-lookup"><span data-stu-id="d94e7-129">bypassMode</span></span>|<span data-ttu-id="d94e7-130">100</span><span class="sxs-lookup"><span data-stu-id="d94e7-130">100</span></span>|<span data-ttu-id="d94e7-131">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="d94e7-131">Bypass mode.</span></span> <span data-ttu-id="d94e7-132">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="d94e7-132">Do not use Delivery Optimization and use BITS instead</span></span>|





