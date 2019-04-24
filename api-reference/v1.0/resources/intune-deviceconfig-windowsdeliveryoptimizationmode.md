---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9034c7c90257a7ca622cd203d4ab84387fd2014
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463891"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="9ddb7-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="9ddb7-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="9ddb7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ddb7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ddb7-105">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="9ddb7-105">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="9ddb7-106">Membros</span><span class="sxs-lookup"><span data-stu-id="9ddb7-106">Members</span></span>
|<span data-ttu-id="9ddb7-107">Membro</span><span class="sxs-lookup"><span data-stu-id="9ddb7-107">Member</span></span>|<span data-ttu-id="9ddb7-108">Valor</span><span class="sxs-lookup"><span data-stu-id="9ddb7-108">Value</span></span>|<span data-ttu-id="9ddb7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ddb7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ddb7-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="9ddb7-110">userDefined</span></span>|<span data-ttu-id="9ddb7-111">,0</span><span class="sxs-lookup"><span data-stu-id="9ddb7-111">0</span></span>|<span data-ttu-id="9ddb7-112">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="9ddb7-112">Allow the user to set.</span></span>|
|<span data-ttu-id="9ddb7-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="9ddb7-113">httpOnly</span></span>|<span data-ttu-id="9ddb7-114">1</span><span class="sxs-lookup"><span data-stu-id="9ddb7-114">1</span></span>|<span data-ttu-id="9ddb7-115">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="9ddb7-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="9ddb7-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="9ddb7-116">httpWithPeeringNat</span></span>|<span data-ttu-id="9ddb7-117">duas</span><span class="sxs-lookup"><span data-stu-id="9ddb7-117">2</span></span>|<span data-ttu-id="9ddb7-118">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="9ddb7-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="9ddb7-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="9ddb7-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="9ddb7-120">3D</span><span class="sxs-lookup"><span data-stu-id="9ddb7-120">3</span></span>|<span data-ttu-id="9ddb7-121">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="9ddb7-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="9ddb7-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="9ddb7-122">httpWithInternetPeering</span></span>|<span data-ttu-id="9ddb7-123">quatro</span><span class="sxs-lookup"><span data-stu-id="9ddb7-123">4</span></span>|<span data-ttu-id="9ddb7-124">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="9ddb7-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="9ddb7-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="9ddb7-125">simpleDownload</span></span>|<span data-ttu-id="9ddb7-126">99</span><span class="sxs-lookup"><span data-stu-id="9ddb7-126">99</span></span>|<span data-ttu-id="9ddb7-127">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="9ddb7-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="9ddb7-128">bypassmode</span><span class="sxs-lookup"><span data-stu-id="9ddb7-128">bypassMode</span></span>|<span data-ttu-id="9ddb7-129">100</span><span class="sxs-lookup"><span data-stu-id="9ddb7-129">100</span></span>|<span data-ttu-id="9ddb7-130">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="9ddb7-130">Bypass mode.</span></span> <span data-ttu-id="9ddb7-131">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="9ddb7-131">Do not use Delivery Optimization and use BITS instead</span></span>|



