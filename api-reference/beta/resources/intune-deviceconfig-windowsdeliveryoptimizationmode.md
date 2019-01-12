---
title: tipo de enum windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de ponto
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 004bb3d3984d8d304f89dc339899035d218546a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972653"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="24e33-103">tipo de enum windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="24e33-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="24e33-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="24e33-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24e33-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="24e33-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24e33-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="24e33-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24e33-107">Modo de otimização de entrega para distribuição de ponto</span><span class="sxs-lookup"><span data-stu-id="24e33-107">Delivery optimization mode for peer distribution</span></span>
## <a name="members"></a><span data-ttu-id="24e33-108">Membros</span><span class="sxs-lookup"><span data-stu-id="24e33-108">Members</span></span>
|<span data-ttu-id="24e33-109">Membro</span><span class="sxs-lookup"><span data-stu-id="24e33-109">Member</span></span>|<span data-ttu-id="24e33-110">Valor</span><span class="sxs-lookup"><span data-stu-id="24e33-110">Value</span></span>|<span data-ttu-id="24e33-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="24e33-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24e33-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="24e33-112">userDefined</span></span>|<span data-ttu-id="24e33-113">0</span><span class="sxs-lookup"><span data-stu-id="24e33-113">0</span></span>|<span data-ttu-id="24e33-114">Permitir que o usuário pode definir.</span><span class="sxs-lookup"><span data-stu-id="24e33-114">Allow the user to set.</span></span>|
|<span data-ttu-id="24e33-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="24e33-115">httpOnly</span></span>|<span data-ttu-id="24e33-116">1</span><span class="sxs-lookup"><span data-stu-id="24e33-116">1</span></span>|<span data-ttu-id="24e33-117">HTTP apenas, nenhuma correspondência</span><span class="sxs-lookup"><span data-stu-id="24e33-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="24e33-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="24e33-118">httpWithPeeringNat</span></span>|<span data-ttu-id="24e33-119">2</span><span class="sxs-lookup"><span data-stu-id="24e33-119">2</span></span>|<span data-ttu-id="24e33-120">Padrão do sistema operacional – Http misturados com correspondência atrás do mesmo conversor de endereços de rede</span><span class="sxs-lookup"><span data-stu-id="24e33-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="24e33-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="24e33-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="24e33-122">3</span><span class="sxs-lookup"><span data-stu-id="24e33-122">3</span></span>|<span data-ttu-id="24e33-123">HTTP misturados com correspondência entre um grupo privado</span><span class="sxs-lookup"><span data-stu-id="24e33-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="24e33-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="24e33-124">httpWithInternetPeering</span></span>|<span data-ttu-id="24e33-125">4</span><span class="sxs-lookup"><span data-stu-id="24e33-125">4</span></span>|<span data-ttu-id="24e33-126">HTTP misturado com correspondência de Internet</span><span class="sxs-lookup"><span data-stu-id="24e33-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="24e33-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="24e33-127">simpleDownload</span></span>|<span data-ttu-id="24e33-128">99</span><span class="sxs-lookup"><span data-stu-id="24e33-128">99</span></span>|<span data-ttu-id="24e33-129">Modo de download simples com nenhuma correspondência</span><span class="sxs-lookup"><span data-stu-id="24e33-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="24e33-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="24e33-130">bypassMode</span></span>|<span data-ttu-id="24e33-131">100</span><span class="sxs-lookup"><span data-stu-id="24e33-131">100</span></span>|<span data-ttu-id="24e33-132">Modo de desvio.</span><span class="sxs-lookup"><span data-stu-id="24e33-132">Bypass mode.</span></span> <span data-ttu-id="24e33-133">Não use a otimização de entrega e usar o BITS</span><span class="sxs-lookup"><span data-stu-id="24e33-133">Do not use Delivery Optimization and use BITS instead</span></span>|





