---
title: tipo de enum ratingGermanyTelevisionType
description: Rótulos de classificação de conteúdo de TV na Alemanha
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d9bbe383b13e5a6f3d9ec704977b284eaf740aed
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424613"
---
# <a name="ratinggermanytelevisiontype-enum-type"></a><span data-ttu-id="86f11-103">tipo de enum ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="86f11-103">ratingGermanyTelevisionType enum type</span></span>

> <span data-ttu-id="86f11-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="86f11-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="86f11-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="86f11-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86f11-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="86f11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86f11-107">Rótulos de classificação de conteúdo de TV na Alemanha</span><span class="sxs-lookup"><span data-stu-id="86f11-107">TV content rating labels in Germany</span></span>

## <a name="members"></a><span data-ttu-id="86f11-108">Membros</span><span class="sxs-lookup"><span data-stu-id="86f11-108">Members</span></span>
|<span data-ttu-id="86f11-109">Membro</span><span class="sxs-lookup"><span data-stu-id="86f11-109">Member</span></span>|<span data-ttu-id="86f11-110">Valor</span><span class="sxs-lookup"><span data-stu-id="86f11-110">Value</span></span>|<span data-ttu-id="86f11-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="86f11-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86f11-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="86f11-112">allAllowed</span></span>|<span data-ttu-id="86f11-113">0</span><span class="sxs-lookup"><span data-stu-id="86f11-113">0</span></span>|<span data-ttu-id="86f11-114">Valor padrão, para permitir que todos os TV mostra conteúdo</span><span class="sxs-lookup"><span data-stu-id="86f11-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="86f11-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="86f11-115">allBlocked</span></span>|<span data-ttu-id="86f11-116">1</span><span class="sxs-lookup"><span data-stu-id="86f11-116">1</span></span>|<span data-ttu-id="86f11-117">Não permitir que qualquer TV mostra conteúdo</span><span class="sxs-lookup"><span data-stu-id="86f11-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="86f11-118">geral</span><span class="sxs-lookup"><span data-stu-id="86f11-118">general</span></span>|<span data-ttu-id="86f11-119">2</span><span class="sxs-lookup"><span data-stu-id="86f11-119">2</span></span>|<span data-ttu-id="86f11-120">Jahren AB 0, não há restrições de idade</span><span class="sxs-lookup"><span data-stu-id="86f11-120">Ab 0 Jahren, no age restrictions</span></span>|
|<span data-ttu-id="86f11-121">agesAbove6</span><span class="sxs-lookup"><span data-stu-id="86f11-121">agesAbove6</span></span>|<span data-ttu-id="86f11-122">3</span><span class="sxs-lookup"><span data-stu-id="86f11-122">3</span></span>|<span data-ttu-id="86f11-123">Jahren de 6 AB, expira antigas e 6</span><span class="sxs-lookup"><span data-stu-id="86f11-123">Ab 6 Jahren, ages 6 and older</span></span>|
|<span data-ttu-id="86f11-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="86f11-124">agesAbove12</span></span>|<span data-ttu-id="86f11-125">4</span><span class="sxs-lookup"><span data-stu-id="86f11-125">4</span></span>|<span data-ttu-id="86f11-126">Jahren de 12 AB, expira antigas e 12</span><span class="sxs-lookup"><span data-stu-id="86f11-126">Ab 12 Jahren, ages 12 and older</span></span>|
|<span data-ttu-id="86f11-127">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="86f11-127">agesAbove16</span></span>|<span data-ttu-id="86f11-128">5</span><span class="sxs-lookup"><span data-stu-id="86f11-128">5</span></span>|<span data-ttu-id="86f11-129">Jahren de 16 AB, expira antigas e 16</span><span class="sxs-lookup"><span data-stu-id="86f11-129">Ab 16 Jahren, ages 16 and older</span></span>|
|<span data-ttu-id="86f11-130">adultos</span><span class="sxs-lookup"><span data-stu-id="86f11-130">adults</span></span>|<span data-ttu-id="86f11-131">6</span><span class="sxs-lookup"><span data-stu-id="86f11-131">6</span></span>|<span data-ttu-id="86f11-132">AB 18 Jahren, somente para adultos</span><span class="sxs-lookup"><span data-stu-id="86f11-132">Ab 18 Jahren, adults only</span></span>|




