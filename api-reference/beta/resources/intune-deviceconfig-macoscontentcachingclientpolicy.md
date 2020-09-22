---
title: tipo de enumeração macOSContentCachingClientPolicy
description: Determina quais clientes um cache de conteúdo servirá.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0ff1146d69fabdb8a9e734e0ae82747831e0a390
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026639"
---
# <a name="macoscontentcachingclientpolicy-enum-type"></a><span data-ttu-id="a80b7-103">tipo de enumeração macOSContentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="a80b7-103">macOSContentCachingClientPolicy enum type</span></span>

<span data-ttu-id="a80b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a80b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a80b7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a80b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a80b7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a80b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a80b7-107">Determina quais clientes um cache de conteúdo servirá.</span><span class="sxs-lookup"><span data-stu-id="a80b7-107">Determines which clients a content cache will serve.</span></span>

## <a name="members"></a><span data-ttu-id="a80b7-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a80b7-108">Members</span></span>
|<span data-ttu-id="a80b7-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a80b7-109">Member</span></span>|<span data-ttu-id="a80b7-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a80b7-110">Value</span></span>|<span data-ttu-id="a80b7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a80b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a80b7-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a80b7-112">notConfigured</span></span>|<span data-ttu-id="a80b7-113">,0</span><span class="sxs-lookup"><span data-stu-id="a80b7-113">0</span></span>|<span data-ttu-id="a80b7-114">O padrão é para os clientes na rede local.</span><span class="sxs-lookup"><span data-stu-id="a80b7-114">Defaults to clients in local network.</span></span>|
|<span data-ttu-id="a80b7-115">clientsInLocalNetwork</span><span class="sxs-lookup"><span data-stu-id="a80b7-115">clientsInLocalNetwork</span></span>|<span data-ttu-id="a80b7-116">1 </span><span class="sxs-lookup"><span data-stu-id="a80b7-116">1</span></span>|<span data-ttu-id="a80b7-117">Os caches de conteúdo fornecerão conteúdo aos dispositivos somente em sua rede local imediata.</span><span class="sxs-lookup"><span data-stu-id="a80b7-117">Content caches will provide content to devices only in their immediate local network.</span></span>|
|<span data-ttu-id="a80b7-118">clientsWithSamePublicIpAddress</span><span class="sxs-lookup"><span data-stu-id="a80b7-118">clientsWithSamePublicIpAddress</span></span>|<span data-ttu-id="a80b7-119">2 </span><span class="sxs-lookup"><span data-stu-id="a80b7-119">2</span></span>|<span data-ttu-id="a80b7-120">Os caches de conteúdo fornecerão conteúdo aos dispositivos que compartilham o mesmo endereço IP público.</span><span class="sxs-lookup"><span data-stu-id="a80b7-120">Content caches will provide content to devices that share the same public IP address.</span></span>|
|<span data-ttu-id="a80b7-121">clientsInCustomLocalNetworks</span><span class="sxs-lookup"><span data-stu-id="a80b7-121">clientsInCustomLocalNetworks</span></span>|<span data-ttu-id="a80b7-122">3 </span><span class="sxs-lookup"><span data-stu-id="a80b7-122">3</span></span>|<span data-ttu-id="a80b7-123">Os caches de conteúdo fornecerão conteúdo aos dispositivos no contentCachingClientListenRanges.</span><span class="sxs-lookup"><span data-stu-id="a80b7-123">Content caches will provide content to devices in contentCachingClientListenRanges.</span></span>|
|<span data-ttu-id="a80b7-124">clientsInCustomLocalNetworksWithFallback</span><span class="sxs-lookup"><span data-stu-id="a80b7-124">clientsInCustomLocalNetworksWithFallback</span></span>|<span data-ttu-id="a80b7-125">4 </span><span class="sxs-lookup"><span data-stu-id="a80b7-125">4</span></span>|<span data-ttu-id="a80b7-126">Os caches de conteúdo fornecerão conteúdo aos dispositivos no contentCachingClientListenRanges, contentCachingPeerListenRanges e contentCachingParents.</span><span class="sxs-lookup"><span data-stu-id="a80b7-126">Content caches will provide content to devices in contentCachingClientListenRanges, contentCachingPeerListenRanges, and contentCachingParents.</span></span>|






