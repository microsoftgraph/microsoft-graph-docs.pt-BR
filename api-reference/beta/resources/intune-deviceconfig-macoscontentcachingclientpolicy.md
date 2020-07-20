---
title: tipo de enumeração macOSContentCachingClientPolicy
description: Determina quais clientes um cache de conteúdo servirá.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58ee56344d352b21e58eb86a795c6be5262f272d
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790240"
---
# <a name="macoscontentcachingclientpolicy-enum-type"></a><span data-ttu-id="6fd14-103">tipo de enumeração macOSContentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="6fd14-103">macOSContentCachingClientPolicy enum type</span></span>

<span data-ttu-id="6fd14-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fd14-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fd14-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6fd14-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fd14-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6fd14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fd14-107">Determina quais clientes um cache de conteúdo servirá.</span><span class="sxs-lookup"><span data-stu-id="6fd14-107">Determines which clients a content cache will serve.</span></span>

## <a name="members"></a><span data-ttu-id="6fd14-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6fd14-108">Members</span></span>
|<span data-ttu-id="6fd14-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6fd14-109">Member</span></span>|<span data-ttu-id="6fd14-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6fd14-110">Value</span></span>|<span data-ttu-id="6fd14-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fd14-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fd14-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6fd14-112">notConfigured</span></span>|<span data-ttu-id="6fd14-113">,0</span><span class="sxs-lookup"><span data-stu-id="6fd14-113">0</span></span>|<span data-ttu-id="6fd14-114">O padrão é para os clientes na rede local.</span><span class="sxs-lookup"><span data-stu-id="6fd14-114">Defaults to clients in local network.</span></span>|
|<span data-ttu-id="6fd14-115">clientsInLocalNetwork</span><span class="sxs-lookup"><span data-stu-id="6fd14-115">clientsInLocalNetwork</span></span>|<span data-ttu-id="6fd14-116">1 </span><span class="sxs-lookup"><span data-stu-id="6fd14-116">1</span></span>|<span data-ttu-id="6fd14-117">Os caches de conteúdo fornecerão conteúdo aos dispositivos somente em sua rede local imediata.</span><span class="sxs-lookup"><span data-stu-id="6fd14-117">Content caches will provide content to devices only in their immediate local network.</span></span>|
|<span data-ttu-id="6fd14-118">clientsWithSamePublicIpAddress</span><span class="sxs-lookup"><span data-stu-id="6fd14-118">clientsWithSamePublicIpAddress</span></span>|<span data-ttu-id="6fd14-119">duas</span><span class="sxs-lookup"><span data-stu-id="6fd14-119">2</span></span>|<span data-ttu-id="6fd14-120">Os caches de conteúdo fornecerão conteúdo aos dispositivos que compartilham o mesmo endereço IP público.</span><span class="sxs-lookup"><span data-stu-id="6fd14-120">Content caches will provide content to devices that share the same public IP address.</span></span>|
|<span data-ttu-id="6fd14-121">clientsInCustomLocalNetworks</span><span class="sxs-lookup"><span data-stu-id="6fd14-121">clientsInCustomLocalNetworks</span></span>|<span data-ttu-id="6fd14-122">3D</span><span class="sxs-lookup"><span data-stu-id="6fd14-122">3</span></span>|<span data-ttu-id="6fd14-123">Os caches de conteúdo fornecerão conteúdo aos dispositivos no contentCachingClientListenRanges.</span><span class="sxs-lookup"><span data-stu-id="6fd14-123">Content caches will provide content to devices in contentCachingClientListenRanges.</span></span>|
|<span data-ttu-id="6fd14-124">clientsInCustomLocalNetworksWithFallback</span><span class="sxs-lookup"><span data-stu-id="6fd14-124">clientsInCustomLocalNetworksWithFallback</span></span>|<span data-ttu-id="6fd14-125">4 </span><span class="sxs-lookup"><span data-stu-id="6fd14-125">4</span></span>|<span data-ttu-id="6fd14-126">Os caches de conteúdo fornecerão conteúdo aos dispositivos no contentCachingClientListenRanges, contentCachingPeerListenRanges e contentCachingParents.</span><span class="sxs-lookup"><span data-stu-id="6fd14-126">Content caches will provide content to devices in contentCachingClientListenRanges, contentCachingPeerListenRanges, and contentCachingParents.</span></span>|



