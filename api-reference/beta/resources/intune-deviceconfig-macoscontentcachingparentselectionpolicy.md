---
title: tipo de enumeração macOSContentCachingParentSelectionPolicy
description: Determina como os caches de conteúdo selecionam um cache pai.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 726c6d4feb7387fd67583c451a9f3399a316f4a0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735817"
---
# <a name="macoscontentcachingparentselectionpolicy-enum-type"></a><span data-ttu-id="cf0c6-103">tipo de enumeração macOSContentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="cf0c6-103">macOSContentCachingParentSelectionPolicy enum type</span></span>

<span data-ttu-id="cf0c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf0c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf0c6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf0c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf0c6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf0c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf0c6-107">Determina como os caches de conteúdo selecionam um cache pai.</span><span class="sxs-lookup"><span data-stu-id="cf0c6-107">Determines how content caches select a parent cache.</span></span>

## <a name="members"></a><span data-ttu-id="cf0c6-108">Membros</span><span class="sxs-lookup"><span data-stu-id="cf0c6-108">Members</span></span>
|<span data-ttu-id="cf0c6-109">Membro</span><span class="sxs-lookup"><span data-stu-id="cf0c6-109">Member</span></span>|<span data-ttu-id="cf0c6-110">Valor</span><span class="sxs-lookup"><span data-stu-id="cf0c6-110">Value</span></span>|<span data-ttu-id="cf0c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf0c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf0c6-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="cf0c6-112">notConfigured</span></span>|<span data-ttu-id="cf0c6-113">,0</span><span class="sxs-lookup"><span data-stu-id="cf0c6-113">0</span></span>|<span data-ttu-id="cf0c6-114">O padrão é a estratégia de rodízio.</span><span class="sxs-lookup"><span data-stu-id="cf0c6-114">Defaults to round-robin strategy.</span></span>|
|<span data-ttu-id="cf0c6-115">roundRobin</span><span class="sxs-lookup"><span data-stu-id="cf0c6-115">roundRobin</span></span>|<span data-ttu-id="cf0c6-116">1</span><span class="sxs-lookup"><span data-stu-id="cf0c6-116">1</span></span>|<span data-ttu-id="cf0c6-117">Girar através dos pais na ordem.</span><span class="sxs-lookup"><span data-stu-id="cf0c6-117">Rotate through the parents in order.</span></span> <span data-ttu-id="cf0c6-118">Use esta política para balanceamento de carga.</span><span class="sxs-lookup"><span data-stu-id="cf0c6-118">Use this policy for load balancing.</span></span>|
|<span data-ttu-id="cf0c6-119">firstAvailable</span><span class="sxs-lookup"><span data-stu-id="cf0c6-119">firstAvailable</span></span>|<span data-ttu-id="cf0c6-120">duas</span><span class="sxs-lookup"><span data-stu-id="cf0c6-120">2</span></span>|<span data-ttu-id="cf0c6-121">Sempre use o primeiro pai disponível na lista de pais.</span><span class="sxs-lookup"><span data-stu-id="cf0c6-121">Always use the first available parent in the Parents list.</span></span> <span data-ttu-id="cf0c6-122">Use essa política para designar os pais primários, secundários e subsequentes permanentes.</span><span class="sxs-lookup"><span data-stu-id="cf0c6-122">Use this policy to designate permanent primary, secondary, and subsequent parents.</span></span>|
|<span data-ttu-id="cf0c6-123">urlPathHash</span><span class="sxs-lookup"><span data-stu-id="cf0c6-123">urlPathHash</span></span>|<span data-ttu-id="cf0c6-124">3D</span><span class="sxs-lookup"><span data-stu-id="cf0c6-124">3</span></span>|<span data-ttu-id="cf0c6-125">Hash a parte do caminho da URL solicitada para que o mesmo pai seja sempre usado para a mesma URL.</span><span class="sxs-lookup"><span data-stu-id="cf0c6-125">Hash the path part of the requested URL so that the same parent is always used for the same URL.</span></span> <span data-ttu-id="cf0c6-126">Isso é útil para maximizar o tamanho dos caches combinados dos pais.</span><span class="sxs-lookup"><span data-stu-id="cf0c6-126">This is useful for maximizing the size of the combined caches of the parents.</span></span>|
|<span data-ttu-id="cf0c6-127">aleatório</span><span class="sxs-lookup"><span data-stu-id="cf0c6-127">random</span></span>|<span data-ttu-id="cf0c6-128">4 </span><span class="sxs-lookup"><span data-stu-id="cf0c6-128">4</span></span>|<span data-ttu-id="cf0c6-129">Escolha um pai aleatoriamente.</span><span class="sxs-lookup"><span data-stu-id="cf0c6-129">Choose a parent at random.</span></span> <span data-ttu-id="cf0c6-130">Use esta política para balanceamento de carga.</span><span class="sxs-lookup"><span data-stu-id="cf0c6-130">Use this policy for load balancing.</span></span>|
|<span data-ttu-id="cf0c6-131">stickyAvailable</span><span class="sxs-lookup"><span data-stu-id="cf0c6-131">stickyAvailable</span></span>|<span data-ttu-id="cf0c6-132">5 </span><span class="sxs-lookup"><span data-stu-id="cf0c6-132">5</span></span>|<span data-ttu-id="cf0c6-133">Use o primeiro pai disponível que está disponível na lista de pais até que fique indisponível e vá para o próximo.</span><span class="sxs-lookup"><span data-stu-id="cf0c6-133">Use the first available parent that is available in the Parents list until it becomes unavailable, then advance to the next one.</span></span> <span data-ttu-id="cf0c6-134">Use essa política para designar os pais primários, secundários e subsequentes.</span><span class="sxs-lookup"><span data-stu-id="cf0c6-134">Use this policy for designating floating primary, secondary, and subsequent parents.</span></span>|





