---
title: Tipo denum windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de pares
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5c483f00817858e7061bacf1b1e2b6ec6c00a02b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742745"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="c02fa-103">Tipo denum windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="c02fa-103">windowsDeliveryOptimizationMode enum type</span></span>

<span data-ttu-id="c02fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c02fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c02fa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c02fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c02fa-106">Modo de otimização de entrega para distribuição de pares</span><span class="sxs-lookup"><span data-stu-id="c02fa-106">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="c02fa-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c02fa-107">Members</span></span>
|<span data-ttu-id="c02fa-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c02fa-108">Member</span></span>|<span data-ttu-id="c02fa-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c02fa-109">Value</span></span>|<span data-ttu-id="c02fa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c02fa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c02fa-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="c02fa-111">userDefined</span></span>|<span data-ttu-id="c02fa-112">0</span><span class="sxs-lookup"><span data-stu-id="c02fa-112">0</span></span>|<span data-ttu-id="c02fa-113">Permitir que o usuário desem conjunto.</span><span class="sxs-lookup"><span data-stu-id="c02fa-113">Allow the user to set.</span></span>|
|<span data-ttu-id="c02fa-114">httpOnly</span><span class="sxs-lookup"><span data-stu-id="c02fa-114">httpOnly</span></span>|<span data-ttu-id="c02fa-115">1</span><span class="sxs-lookup"><span data-stu-id="c02fa-115">1</span></span>|<span data-ttu-id="c02fa-116">Somente HTTP, sem par</span><span class="sxs-lookup"><span data-stu-id="c02fa-116">HTTP only, no peering</span></span>|
|<span data-ttu-id="c02fa-117">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="c02fa-117">httpWithPeeringNat</span></span>|<span data-ttu-id="c02fa-118">2</span><span class="sxs-lookup"><span data-stu-id="c02fa-118">2</span></span>|<span data-ttu-id="c02fa-119">Padrão do sistema operacional – Http mesclado com o peering por trás do mesmo tradutor de endereços de rede</span><span class="sxs-lookup"><span data-stu-id="c02fa-119">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="c02fa-120">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="c02fa-120">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="c02fa-121">3</span><span class="sxs-lookup"><span data-stu-id="c02fa-121">3</span></span>|<span data-ttu-id="c02fa-122">HTTP mesclado com o peering em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="c02fa-122">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="c02fa-123">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="c02fa-123">httpWithInternetPeering</span></span>|<span data-ttu-id="c02fa-124">4 </span><span class="sxs-lookup"><span data-stu-id="c02fa-124">4</span></span>|<span data-ttu-id="c02fa-125">HTTP mesclado com o peering da Internet</span><span class="sxs-lookup"><span data-stu-id="c02fa-125">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="c02fa-126">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="c02fa-126">simpleDownload</span></span>|<span data-ttu-id="c02fa-127">99</span><span class="sxs-lookup"><span data-stu-id="c02fa-127">99</span></span>|<span data-ttu-id="c02fa-128">Modo de download simples sem par</span><span class="sxs-lookup"><span data-stu-id="c02fa-128">Simple download mode with no peering</span></span>|
|<span data-ttu-id="c02fa-129">bypassMode</span><span class="sxs-lookup"><span data-stu-id="c02fa-129">bypassMode</span></span>|<span data-ttu-id="c02fa-130">100</span><span class="sxs-lookup"><span data-stu-id="c02fa-130">100</span></span>|<span data-ttu-id="c02fa-131">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="c02fa-131">Bypass mode.</span></span> <span data-ttu-id="c02fa-132">Não use a Otimização de Entrega e use BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="c02fa-132">Do not use Delivery Optimization and use BITS instead</span></span>|




