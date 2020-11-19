---
title: tipo de enumeração macOSContentCachingPeerPolicy
description: Determina quais conteúdos em cache outros caches de conteúdo terão pontos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7305c42098782d9e69e734037fb08d3238c7b4a9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268745"
---
# <a name="macoscontentcachingpeerpolicy-enum-type"></a><span data-ttu-id="9d6e8-103">tipo de enumeração macOSContentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="9d6e8-103">macOSContentCachingPeerPolicy enum type</span></span>

<span data-ttu-id="9d6e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d6e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d6e8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9d6e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d6e8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d6e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d6e8-107">Determina quais conteúdos em cache outros caches de conteúdo terão pontos.</span><span class="sxs-lookup"><span data-stu-id="9d6e8-107">Determines which content caches other content caches will peer with.</span></span>

## <a name="members"></a><span data-ttu-id="9d6e8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="9d6e8-108">Members</span></span>
|<span data-ttu-id="9d6e8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="9d6e8-109">Member</span></span>|<span data-ttu-id="9d6e8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="9d6e8-110">Value</span></span>|<span data-ttu-id="9d6e8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d6e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d6e8-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9d6e8-112">notConfigured</span></span>|<span data-ttu-id="9d6e8-113">,0</span><span class="sxs-lookup"><span data-stu-id="9d6e8-113">0</span></span>|<span data-ttu-id="9d6e8-114">O padrão é para pares na rede local.</span><span class="sxs-lookup"><span data-stu-id="9d6e8-114">Defaults to peers in local network.</span></span>|
|<span data-ttu-id="9d6e8-115">peersInLocalNetwork</span><span class="sxs-lookup"><span data-stu-id="9d6e8-115">peersInLocalNetwork</span></span>|<span data-ttu-id="9d6e8-116">1</span><span class="sxs-lookup"><span data-stu-id="9d6e8-116">1</span></span>|<span data-ttu-id="9d6e8-117">Os caches de conteúdo só serão iguais aos caches em sua rede local imediata.</span><span class="sxs-lookup"><span data-stu-id="9d6e8-117">Content caches will only peer with caches in their immediate local network.</span></span>|
|<span data-ttu-id="9d6e8-118">peersWithSamePublicIpAddress</span><span class="sxs-lookup"><span data-stu-id="9d6e8-118">peersWithSamePublicIpAddress</span></span>|<span data-ttu-id="9d6e8-119">duas</span><span class="sxs-lookup"><span data-stu-id="9d6e8-119">2</span></span>|<span data-ttu-id="9d6e8-120">Os caches de conteúdo só serão pontos com caches que compartilham o mesmo endereço IP público.</span><span class="sxs-lookup"><span data-stu-id="9d6e8-120">Content caches will only peer with caches that share the same public IP address.</span></span>|
|<span data-ttu-id="9d6e8-121">peersInCustomLocalNetworks</span><span class="sxs-lookup"><span data-stu-id="9d6e8-121">peersInCustomLocalNetworks</span></span>|<span data-ttu-id="9d6e8-122">3D</span><span class="sxs-lookup"><span data-stu-id="9d6e8-122">3</span></span>|<span data-ttu-id="9d6e8-123">Os caches de conteúdo usarão o contentCachingPeerFilterRanges e o contentCachingPeerListenRanges para determinar em que caches os pontos serão.</span><span class="sxs-lookup"><span data-stu-id="9d6e8-123">Content caches will use contentCachingPeerFilterRanges and contentCachingPeerListenRanges to determine which caches to peer with.</span></span>|




