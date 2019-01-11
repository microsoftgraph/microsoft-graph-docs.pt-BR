---
title: tipo de enum windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de ponto
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af266b55fd58f788965d33d0d807511d263f6195
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888176"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="fcae3-103">tipo de enum windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="fcae3-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="fcae3-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fcae3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcae3-105">Modo de otimização de entrega para distribuição de ponto</span><span class="sxs-lookup"><span data-stu-id="fcae3-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="fcae3-106">Membros</span><span class="sxs-lookup"><span data-stu-id="fcae3-106">Members</span></span>
|<span data-ttu-id="fcae3-107">Membro</span><span class="sxs-lookup"><span data-stu-id="fcae3-107">Member</span></span>|<span data-ttu-id="fcae3-108">Valor</span><span class="sxs-lookup"><span data-stu-id="fcae3-108">Value</span></span>|<span data-ttu-id="fcae3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcae3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcae3-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="fcae3-110">userDefined</span></span>|<span data-ttu-id="fcae3-111">0</span><span class="sxs-lookup"><span data-stu-id="fcae3-111">0</span></span>|<span data-ttu-id="fcae3-112">Permitir que o usuário pode definir.</span><span class="sxs-lookup"><span data-stu-id="fcae3-112">Allow the user to set.</span></span>|
|<span data-ttu-id="fcae3-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="fcae3-113">httpOnly</span></span>|<span data-ttu-id="fcae3-114">1</span><span class="sxs-lookup"><span data-stu-id="fcae3-114">1</span></span>|<span data-ttu-id="fcae3-115">HTTP apenas, nenhuma correspondência</span><span class="sxs-lookup"><span data-stu-id="fcae3-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="fcae3-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="fcae3-116">httpWithPeeringNat</span></span>|<span data-ttu-id="fcae3-117">2</span><span class="sxs-lookup"><span data-stu-id="fcae3-117">2</span></span>|<span data-ttu-id="fcae3-118">Padrão do sistema operacional – Http misturados com correspondência atrás do mesmo conversor de endereços de rede</span><span class="sxs-lookup"><span data-stu-id="fcae3-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="fcae3-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="fcae3-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="fcae3-120">3</span><span class="sxs-lookup"><span data-stu-id="fcae3-120">3</span></span>|<span data-ttu-id="fcae3-121">HTTP misturados com correspondência entre um grupo privado</span><span class="sxs-lookup"><span data-stu-id="fcae3-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="fcae3-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="fcae3-122">httpWithInternetPeering</span></span>|<span data-ttu-id="fcae3-123">4</span><span class="sxs-lookup"><span data-stu-id="fcae3-123">4</span></span>|<span data-ttu-id="fcae3-124">HTTP misturado com correspondência de Internet</span><span class="sxs-lookup"><span data-stu-id="fcae3-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="fcae3-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="fcae3-125">simpleDownload</span></span>|<span data-ttu-id="fcae3-126">99</span><span class="sxs-lookup"><span data-stu-id="fcae3-126">99</span></span>|<span data-ttu-id="fcae3-127">Modo de download simples com nenhuma correspondência</span><span class="sxs-lookup"><span data-stu-id="fcae3-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="fcae3-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="fcae3-128">bypassMode</span></span>|<span data-ttu-id="fcae3-129">100</span><span class="sxs-lookup"><span data-stu-id="fcae3-129">100</span></span>|<span data-ttu-id="fcae3-130">Modo de desvio.</span><span class="sxs-lookup"><span data-stu-id="fcae3-130">Bypass mode.</span></span> <span data-ttu-id="fcae3-131">Não use a otimização de entrega e usar o BITS</span><span class="sxs-lookup"><span data-stu-id="fcae3-131">Do not use Delivery Optimization and use BITS instead</span></span>|



