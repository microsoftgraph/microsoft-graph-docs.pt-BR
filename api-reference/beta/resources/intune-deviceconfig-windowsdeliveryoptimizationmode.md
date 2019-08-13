---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b2a66292ec6fb5db3fead93cbda7d24f5e505514
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371163"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="4eddc-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="4eddc-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="4eddc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4eddc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4eddc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4eddc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4eddc-106">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="4eddc-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="4eddc-107">Membros</span><span class="sxs-lookup"><span data-stu-id="4eddc-107">Members</span></span>
|<span data-ttu-id="4eddc-108">Membro</span><span class="sxs-lookup"><span data-stu-id="4eddc-108">Member</span></span>|<span data-ttu-id="4eddc-109">Valor</span><span class="sxs-lookup"><span data-stu-id="4eddc-109">Value</span></span>|<span data-ttu-id="4eddc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4eddc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eddc-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="4eddc-111">userDefined</span></span>|<span data-ttu-id="4eddc-112">,0</span><span class="sxs-lookup"><span data-stu-id="4eddc-112">0</span></span>|<span data-ttu-id="4eddc-113">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="4eddc-113">Allow the user to set.</span></span>|
|<span data-ttu-id="4eddc-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="4eddc-114">httpOnly</span></span>|<span data-ttu-id="4eddc-115">1</span><span class="sxs-lookup"><span data-stu-id="4eddc-115">1</span></span>|<span data-ttu-id="4eddc-116">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="4eddc-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="4eddc-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="4eddc-117">httpWithPeeringNat</span></span>|<span data-ttu-id="4eddc-118">duas</span><span class="sxs-lookup"><span data-stu-id="4eddc-118">2</span></span>|<span data-ttu-id="4eddc-119">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="4eddc-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="4eddc-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="4eddc-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="4eddc-121">3D</span><span class="sxs-lookup"><span data-stu-id="4eddc-121">3</span></span>|<span data-ttu-id="4eddc-122">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="4eddc-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="4eddc-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="4eddc-123">httpWithInternetPeering</span></span>|<span data-ttu-id="4eddc-124">quatro</span><span class="sxs-lookup"><span data-stu-id="4eddc-124">4</span></span>|<span data-ttu-id="4eddc-125">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="4eddc-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="4eddc-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="4eddc-126">simpleDownload</span></span>|<span data-ttu-id="4eddc-127">99</span><span class="sxs-lookup"><span data-stu-id="4eddc-127">99</span></span>|<span data-ttu-id="4eddc-128">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="4eddc-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="4eddc-129">bypassmode</span><span class="sxs-lookup"><span data-stu-id="4eddc-129">bypassMode</span></span>|<span data-ttu-id="4eddc-130">100</span><span class="sxs-lookup"><span data-stu-id="4eddc-130">100</span></span>|<span data-ttu-id="4eddc-131">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="4eddc-131">Bypass mode.</span></span> <span data-ttu-id="4eddc-132">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="4eddc-132">Do not use Delivery Optimization and use BITS instead</span></span>|



