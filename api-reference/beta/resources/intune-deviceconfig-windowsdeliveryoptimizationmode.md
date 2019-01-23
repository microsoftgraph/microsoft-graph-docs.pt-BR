---
title: tipo de enum windowsDeliveryOptimizationMode
description: Modo de otimização de entrega para distribuição de ponto
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5565965f9ba9395d7cd07b2935e6772478e0bb50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406882"
---
# <a name="windowsdeliveryoptimizationmode-enum-type"></a><span data-ttu-id="0627a-103">tipo de enum windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="0627a-103">windowsDeliveryOptimizationMode enum type</span></span>

> <span data-ttu-id="0627a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0627a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0627a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0627a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0627a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0627a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0627a-107">Modo de otimização de entrega para distribuição de ponto</span><span class="sxs-lookup"><span data-stu-id="0627a-107">Delivery optimization mode for peer distribution</span></span>

## <a name="members"></a><span data-ttu-id="0627a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="0627a-108">Members</span></span>
|<span data-ttu-id="0627a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="0627a-109">Member</span></span>|<span data-ttu-id="0627a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="0627a-110">Value</span></span>|<span data-ttu-id="0627a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0627a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0627a-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="0627a-112">userDefined</span></span>|<span data-ttu-id="0627a-113">0</span><span class="sxs-lookup"><span data-stu-id="0627a-113">0</span></span>|<span data-ttu-id="0627a-114">Permitir que o usuário pode definir.</span><span class="sxs-lookup"><span data-stu-id="0627a-114">Allow the user to set.</span></span>|
|<span data-ttu-id="0627a-115">httpOnly</span><span class="sxs-lookup"><span data-stu-id="0627a-115">httpOnly</span></span>|<span data-ttu-id="0627a-116">1</span><span class="sxs-lookup"><span data-stu-id="0627a-116">1</span></span>|<span data-ttu-id="0627a-117">HTTP apenas, nenhuma correspondência</span><span class="sxs-lookup"><span data-stu-id="0627a-117">HTTP only, no peering</span></span>|
|<span data-ttu-id="0627a-118">httpWithPeeringNat</span><span class="sxs-lookup"><span data-stu-id="0627a-118">httpWithPeeringNat</span></span>|<span data-ttu-id="0627a-119">2</span><span class="sxs-lookup"><span data-stu-id="0627a-119">2</span></span>|<span data-ttu-id="0627a-120">Padrão do sistema operacional – Http misturados com correspondência atrás do mesmo conversor de endereços de rede</span><span class="sxs-lookup"><span data-stu-id="0627a-120">OS default – Http blended with peering behind the same network address translator</span></span>|
|<span data-ttu-id="0627a-121">httpWithPeeringPrivateGroup</span><span class="sxs-lookup"><span data-stu-id="0627a-121">httpWithPeeringPrivateGroup</span></span>|<span data-ttu-id="0627a-122">3</span><span class="sxs-lookup"><span data-stu-id="0627a-122">3</span></span>|<span data-ttu-id="0627a-123">HTTP misturados com correspondência entre um grupo privado</span><span class="sxs-lookup"><span data-stu-id="0627a-123">HTTP blended with peering across a private group</span></span>|
|<span data-ttu-id="0627a-124">httpWithInternetPeering</span><span class="sxs-lookup"><span data-stu-id="0627a-124">httpWithInternetPeering</span></span>|<span data-ttu-id="0627a-125">4</span><span class="sxs-lookup"><span data-stu-id="0627a-125">4</span></span>|<span data-ttu-id="0627a-126">HTTP misturado com correspondência de Internet</span><span class="sxs-lookup"><span data-stu-id="0627a-126">HTTP blended with Internet peering</span></span>|
|<span data-ttu-id="0627a-127">simpleDownload</span><span class="sxs-lookup"><span data-stu-id="0627a-127">simpleDownload</span></span>|<span data-ttu-id="0627a-128">99</span><span class="sxs-lookup"><span data-stu-id="0627a-128">99</span></span>|<span data-ttu-id="0627a-129">Modo de download simples com nenhuma correspondência</span><span class="sxs-lookup"><span data-stu-id="0627a-129">Simple download mode with no peering</span></span>|
|<span data-ttu-id="0627a-130">bypassMode</span><span class="sxs-lookup"><span data-stu-id="0627a-130">bypassMode</span></span>|<span data-ttu-id="0627a-131">100</span><span class="sxs-lookup"><span data-stu-id="0627a-131">100</span></span>|<span data-ttu-id="0627a-132">Modo de desvio.</span><span class="sxs-lookup"><span data-stu-id="0627a-132">Bypass mode.</span></span> <span data-ttu-id="0627a-133">Não use a otimização de entrega e usar o BITS</span><span class="sxs-lookup"><span data-stu-id="0627a-133">Do not use Delivery Optimization and use BITS instead</span></span>|




