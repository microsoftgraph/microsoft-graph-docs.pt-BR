---
title: tipo de enumeração windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de mesmo nível
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9154a78af87dbef125e5d211aba284d7a0023e84
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027644"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="de208-103">tipo de enumeração windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="de208-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="de208-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de208-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de208-105">Modo de otimização de entrega para distribuição de mesmo nível</span><span class="sxs-lookup"><span data-stu-id="de208-105">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="de208-106">Membros</span><span class="sxs-lookup"><span data-stu-id="de208-106">Members</span></span>
|<span data-ttu-id="de208-107">Membro</span><span class="sxs-lookup"><span data-stu-id="de208-107">Member</span></span>|<span data-ttu-id="de208-108">Valor</span><span class="sxs-lookup"><span data-stu-id="de208-108">Value</span></span>|<span data-ttu-id="de208-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="de208-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de208-110">UserDefined</span><span class="sxs-lookup"><span data-stu-id="de208-110">userDefined</span></span>|<span data-ttu-id="de208-111">,0</span><span class="sxs-lookup"><span data-stu-id="de208-111">0</span></span>|<span data-ttu-id="de208-112">Permite que o usuário defina.</span><span class="sxs-lookup"><span data-stu-id="de208-112">Allow the user to set.</span></span>|
|<span data-ttu-id="de208-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="de208-113">httpOnly</span></span>|<span data-ttu-id="de208-114">1</span><span class="sxs-lookup"><span data-stu-id="de208-114">1</span></span>|<span data-ttu-id="de208-115">Somente HTTP, sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="de208-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="de208-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="de208-116">httpWithPeeringNat</span></span>|<span data-ttu-id="de208-117">duas</span><span class="sxs-lookup"><span data-stu-id="de208-117">2</span></span>|<span data-ttu-id="de208-118">Padrão de so – http combinado com emparelhamento atrás do mesmo conversor de endereço de rede</span><span class="sxs-lookup"><span data-stu-id="de208-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="de208-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="de208-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="de208-120">3D</span><span class="sxs-lookup"><span data-stu-id="de208-120">3</span></span>|<span data-ttu-id="de208-121">HTTP combinado com emparelhamento em um grupo privado</span><span class="sxs-lookup"><span data-stu-id="de208-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="de208-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="de208-122">httpWithInternetPeering</span></span>|<span data-ttu-id="de208-123">quatro</span><span class="sxs-lookup"><span data-stu-id="de208-123">4</span></span>|<span data-ttu-id="de208-124">HTTP combinado com emparelhamento da Internet</span><span class="sxs-lookup"><span data-stu-id="de208-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="de208-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="de208-125">simpleDownload</span></span>|<span data-ttu-id="de208-126">99</span><span class="sxs-lookup"><span data-stu-id="de208-126">99</span></span>|<span data-ttu-id="de208-127">Modo de download simples sem emparelhamento</span><span class="sxs-lookup"><span data-stu-id="de208-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="de208-128">bypassmode</span><span class="sxs-lookup"><span data-stu-id="de208-128">bypassMode</span></span>|<span data-ttu-id="de208-129">100</span><span class="sxs-lookup"><span data-stu-id="de208-129">100</span></span>|<span data-ttu-id="de208-130">Modo bypass.</span><span class="sxs-lookup"><span data-stu-id="de208-130">Bypass mode.</span></span> <span data-ttu-id="de208-131">Não usar otimização de entrega e usar BITS em vez disso</span><span class="sxs-lookup"><span data-stu-id="de208-131">Do not use Delivery Optimization and use BITS instead</span></span>|



