---
title: tipo de enumeração macOSContentCachingPeerPolicy
description: Determina quais conteúdos em cache outros caches de conteúdo terão pontos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e45f6d0e92624693139cd09ca4eff52cd483b46c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993823"
---
# <a name="macoscontentcachingpeerpolicy-enum-type"></a><span data-ttu-id="2a530-103">tipo de enumeração macOSContentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="2a530-103">macOSContentCachingPeerPolicy enum type</span></span>

<span data-ttu-id="2a530-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a530-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a530-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2a530-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a530-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2a530-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a530-107">Determina quais conteúdos em cache outros caches de conteúdo terão pontos.</span><span class="sxs-lookup"><span data-stu-id="2a530-107">Determines which content caches other content caches will peer with.</span></span>

## <a name="members"></a><span data-ttu-id="2a530-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2a530-108">Members</span></span>
|<span data-ttu-id="2a530-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2a530-109">Member</span></span>|<span data-ttu-id="2a530-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2a530-110">Value</span></span>|<span data-ttu-id="2a530-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a530-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a530-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2a530-112">notConfigured</span></span>|<span data-ttu-id="2a530-113">,0</span><span class="sxs-lookup"><span data-stu-id="2a530-113">0</span></span>|<span data-ttu-id="2a530-114">O padrão é para pares na rede local.</span><span class="sxs-lookup"><span data-stu-id="2a530-114">Defaults to peers in local network.</span></span>|
|<span data-ttu-id="2a530-115">peersInLocalNetwork</span><span class="sxs-lookup"><span data-stu-id="2a530-115">peersInLocalNetwork</span></span>|<span data-ttu-id="2a530-116">1 </span><span class="sxs-lookup"><span data-stu-id="2a530-116">1</span></span>|<span data-ttu-id="2a530-117">Os caches de conteúdo só serão iguais aos caches em sua rede local imediata.</span><span class="sxs-lookup"><span data-stu-id="2a530-117">Content caches will only peer with caches in their immediate local network.</span></span>|
|<span data-ttu-id="2a530-118">peersWithSamePublicIpAddress</span><span class="sxs-lookup"><span data-stu-id="2a530-118">peersWithSamePublicIpAddress</span></span>|<span data-ttu-id="2a530-119">2 </span><span class="sxs-lookup"><span data-stu-id="2a530-119">2</span></span>|<span data-ttu-id="2a530-120">Os caches de conteúdo só serão pontos com caches que compartilham o mesmo endereço IP público.</span><span class="sxs-lookup"><span data-stu-id="2a530-120">Content caches will only peer with caches that share the same public IP address.</span></span>|
|<span data-ttu-id="2a530-121">peersInCustomLocalNetworks</span><span class="sxs-lookup"><span data-stu-id="2a530-121">peersInCustomLocalNetworks</span></span>|<span data-ttu-id="2a530-122">3 </span><span class="sxs-lookup"><span data-stu-id="2a530-122">3</span></span>|<span data-ttu-id="2a530-123">Os caches de conteúdo usarão o contentCachingPeerFilterRanges e o contentCachingPeerListenRanges para determinar em que caches os pontos serão.</span><span class="sxs-lookup"><span data-stu-id="2a530-123">Content caches will use contentCachingPeerFilterRanges and contentCachingPeerListenRanges to determine which caches to peer with.</span></span>|






