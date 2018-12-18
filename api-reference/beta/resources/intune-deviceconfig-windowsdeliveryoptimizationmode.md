---
title: tipo de enum windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de ponto
author: tfitzmac
ms.openlocfilehash: b23bdc80bd8b1fb151f9e138e1a1802140455c4e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333478"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="26778-103">tipo de enum windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="26778-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="26778-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="26778-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26778-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="26778-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26778-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="26778-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26778-107">Modo de otimização de entrega para distribuição de ponto</span><span class="sxs-lookup"><span data-stu-id="26778-107">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="26778-108">Membros</span><span class="sxs-lookup"><span data-stu-id="26778-108">Members</span></span>
|<span data-ttu-id="26778-109">Membro</span><span class="sxs-lookup"><span data-stu-id="26778-109">Member</span></span>|<span data-ttu-id="26778-110">Valor</span><span class="sxs-lookup"><span data-stu-id="26778-110">Value</span></span>|<span data-ttu-id="26778-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="26778-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26778-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="26778-112">userDefined</span></span>|<span data-ttu-id="26778-113">0</span><span class="sxs-lookup"><span data-stu-id="26778-113">0</span></span>|<span data-ttu-id="26778-114">Permitir que o usuário pode definir.</span><span class="sxs-lookup"><span data-stu-id="26778-114">Allow the user to set.</span></span>|
|<span data-ttu-id="26778-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="26778-115">httpOnly</span></span>|<span data-ttu-id="26778-116">1</span><span class="sxs-lookup"><span data-stu-id="26778-116">1</span></span>|<span data-ttu-id="26778-117">HTTP apenas, nenhuma correspondência</span><span class="sxs-lookup"><span data-stu-id="26778-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="26778-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="26778-118">httpWithPeeringNat</span></span>|<span data-ttu-id="26778-119">2</span><span class="sxs-lookup"><span data-stu-id="26778-119">2</span></span>|<span data-ttu-id="26778-120">Padrão do sistema operacional – Http misturados com correspondência atrás do mesmo conversor de endereços de rede</span><span class="sxs-lookup"><span data-stu-id="26778-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="26778-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="26778-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="26778-122">3</span><span class="sxs-lookup"><span data-stu-id="26778-122">3</span></span>|<span data-ttu-id="26778-123">HTTP misturados com correspondência entre um grupo privado</span><span class="sxs-lookup"><span data-stu-id="26778-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="26778-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="26778-124">httpWithInternetPeering</span></span>|<span data-ttu-id="26778-125">4</span><span class="sxs-lookup"><span data-stu-id="26778-125">4</span></span>|<span data-ttu-id="26778-126">HTTP misturado com correspondência de Internet</span><span class="sxs-lookup"><span data-stu-id="26778-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="26778-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="26778-127">simpleDownload</span></span>|<span data-ttu-id="26778-128">99</span><span class="sxs-lookup"><span data-stu-id="26778-128">99</span></span>|<span data-ttu-id="26778-129">Modo de download simples com nenhuma correspondência</span><span class="sxs-lookup"><span data-stu-id="26778-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="26778-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="26778-130">bypassMode</span></span>|<span data-ttu-id="26778-131">100</span><span class="sxs-lookup"><span data-stu-id="26778-131">100</span></span>|<span data-ttu-id="26778-132">Modo de desvio.</span><span class="sxs-lookup"><span data-stu-id="26778-132">Bypass mode.</span></span> <span data-ttu-id="26778-133">Não use a otimização de entrega e usar o BITS</span><span class="sxs-lookup"><span data-stu-id="26778-133">Do not use Delivery Optimization and use BITS instead</span></span>|





