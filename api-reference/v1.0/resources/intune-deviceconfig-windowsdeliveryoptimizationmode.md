---
title: tipo de enum windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de ponto
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f80c6b5cbe7316c851954154bdb559f370f02b79
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951513"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="2179c-103">tipo de enum windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="2179c-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="2179c-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2179c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2179c-105">Modo de otimização de entrega para distribuição de ponto</span><span class="sxs-lookup"><span data-stu-id="2179c-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="2179c-106">Membros</span><span class="sxs-lookup"><span data-stu-id="2179c-106">Members</span></span>
|<span data-ttu-id="2179c-107">Membro</span><span class="sxs-lookup"><span data-stu-id="2179c-107">Member</span></span>|<span data-ttu-id="2179c-108">Valor</span><span class="sxs-lookup"><span data-stu-id="2179c-108">Value</span></span>|<span data-ttu-id="2179c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2179c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2179c-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="2179c-110">userDefined</span></span>|<span data-ttu-id="2179c-111">0</span><span class="sxs-lookup"><span data-stu-id="2179c-111">0</span></span>|<span data-ttu-id="2179c-112">Permitir que o usuário pode definir.</span><span class="sxs-lookup"><span data-stu-id="2179c-112">Allow the user to set.</span></span>|
|<span data-ttu-id="2179c-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="2179c-113">httpOnly</span></span>|<span data-ttu-id="2179c-114">1</span><span class="sxs-lookup"><span data-stu-id="2179c-114">1</span></span>|<span data-ttu-id="2179c-115">HTTP apenas, nenhuma correspondência</span><span class="sxs-lookup"><span data-stu-id="2179c-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="2179c-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="2179c-116">httpWithPeeringNat</span></span>|<span data-ttu-id="2179c-117">2</span><span class="sxs-lookup"><span data-stu-id="2179c-117">2</span></span>|<span data-ttu-id="2179c-118">Padrão do sistema operacional – Http misturados com correspondência atrás do mesmo conversor de endereços de rede</span><span class="sxs-lookup"><span data-stu-id="2179c-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="2179c-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="2179c-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="2179c-120">3</span><span class="sxs-lookup"><span data-stu-id="2179c-120">3</span></span>|<span data-ttu-id="2179c-121">HTTP misturados com correspondência entre um grupo privado</span><span class="sxs-lookup"><span data-stu-id="2179c-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="2179c-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="2179c-122">httpWithInternetPeering</span></span>|<span data-ttu-id="2179c-123">4</span><span class="sxs-lookup"><span data-stu-id="2179c-123">4</span></span>|<span data-ttu-id="2179c-124">HTTP misturado com correspondência de Internet</span><span class="sxs-lookup"><span data-stu-id="2179c-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="2179c-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="2179c-125">simpleDownload</span></span>|<span data-ttu-id="2179c-126">99</span><span class="sxs-lookup"><span data-stu-id="2179c-126">99</span></span>|<span data-ttu-id="2179c-127">Modo de download simples com nenhuma correspondência</span><span class="sxs-lookup"><span data-stu-id="2179c-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="2179c-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="2179c-128">bypassMode</span></span>|<span data-ttu-id="2179c-129">100</span><span class="sxs-lookup"><span data-stu-id="2179c-129">100</span></span>|<span data-ttu-id="2179c-130">Modo de desvio.</span><span class="sxs-lookup"><span data-stu-id="2179c-130">Bypass mode.</span></span> <span data-ttu-id="2179c-131">Não use a otimização de entrega e usar o BITS</span><span class="sxs-lookup"><span data-stu-id="2179c-131">Do not use Delivery Optimization and use BITS instead</span></span>|



