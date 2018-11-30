---
title: tipo de enum windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de ponto
ms.openlocfilehash: 2d393a82f855f3e3a0226c8ccb450fa2dae1a95c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004823"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="edd84-103">tipo de enum windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="edd84-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="edd84-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="edd84-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="edd84-105">Modo de otimização de entrega para distribuição de ponto</span><span class="sxs-lookup"><span data-stu-id="edd84-105">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="edd84-106">Membros</span><span class="sxs-lookup"><span data-stu-id="edd84-106">Members</span></span>
|<span data-ttu-id="edd84-107">Membro</span><span class="sxs-lookup"><span data-stu-id="edd84-107">Member</span></span>|<span data-ttu-id="edd84-108">Valor</span><span class="sxs-lookup"><span data-stu-id="edd84-108">Value</span></span>|<span data-ttu-id="edd84-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="edd84-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edd84-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="edd84-110">userDefined</span></span>|<span data-ttu-id="edd84-111">0</span><span class="sxs-lookup"><span data-stu-id="edd84-111">0</span></span>|<span data-ttu-id="edd84-112">Permitir que o usuário pode definir.</span><span class="sxs-lookup"><span data-stu-id="edd84-112">Allow the user to set.</span></span>|
|<span data-ttu-id="edd84-113">httpOnly</span><span class="sxs-lookup"><span data-stu-id="edd84-113">httpOnly</span></span>|<span data-ttu-id="edd84-114">1</span><span class="sxs-lookup"><span data-stu-id="edd84-114">1</span></span>|<span data-ttu-id="edd84-115">HTTP apenas, nenhuma correspondência</span><span class="sxs-lookup"><span data-stu-id="edd84-115">HTTP only, no peering</span></span>|
|<span data-ttu-id="edd84-116">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="edd84-116">httpWithPeeringNat</span></span>|<span data-ttu-id="edd84-117">2</span><span class="sxs-lookup"><span data-stu-id="edd84-117">2</span></span>|<span data-ttu-id="edd84-118">Padrão do sistema operacional – Http misturados com correspondência atrás do mesmo conversor de endereços de rede</span><span class="sxs-lookup"><span data-stu-id="edd84-118">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="edd84-119">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="edd84-119">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="edd84-120">3</span><span class="sxs-lookup"><span data-stu-id="edd84-120">3</span></span>|<span data-ttu-id="edd84-121">HTTP misturados com correspondência entre um grupo privado</span><span class="sxs-lookup"><span data-stu-id="edd84-121">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="edd84-122">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="edd84-122">httpWithInternetPeering</span></span>|<span data-ttu-id="edd84-123">4</span><span class="sxs-lookup"><span data-stu-id="edd84-123">4</span></span>|<span data-ttu-id="edd84-124">HTTP misturado com correspondência de Internet</span><span class="sxs-lookup"><span data-stu-id="edd84-124">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="edd84-125">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="edd84-125">simpleDownload</span></span>|<span data-ttu-id="edd84-126">99</span><span class="sxs-lookup"><span data-stu-id="edd84-126">99</span></span>|<span data-ttu-id="edd84-127">Modo de download simples com nenhuma correspondência</span><span class="sxs-lookup"><span data-stu-id="edd84-127">Simple download mode with no peering</span></span>|
|<span data-ttu-id="edd84-128">bypassMode</span><span class="sxs-lookup"><span data-stu-id="edd84-128">bypassMode</span></span>|<span data-ttu-id="edd84-129">100</span><span class="sxs-lookup"><span data-stu-id="edd84-129">100</span></span>|<span data-ttu-id="edd84-130">Modo de desvio.</span><span class="sxs-lookup"><span data-stu-id="edd84-130">Bypass mode.</span></span> <span data-ttu-id="edd84-131">Não use a otimização de entrega e usar o BITS</span><span class="sxs-lookup"><span data-stu-id="edd84-131">Do not use Delivery Optimization and use BITS instead</span></span>|



