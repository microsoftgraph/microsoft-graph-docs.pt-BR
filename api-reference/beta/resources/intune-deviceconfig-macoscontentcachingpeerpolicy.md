---
title: tipo de enumeração macOSContentCachingPeerPolicy
description: Determina quais conteúdos em cache outros caches de conteúdo terão pontos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1f55bd6aafffc7602632155e4fa3c387c888aae9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735810"
---
# <a name="macoscontentcachingpeerpolicy-enum-type"></a><span data-ttu-id="cee6b-103">tipo de enumeração macOSContentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="cee6b-103">macOSContentCachingPeerPolicy enum type</span></span>

<span data-ttu-id="cee6b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cee6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cee6b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cee6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cee6b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cee6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cee6b-107">Determina quais conteúdos em cache outros caches de conteúdo terão pontos.</span><span class="sxs-lookup"><span data-stu-id="cee6b-107">Determines which content caches other content caches will peer with.</span></span>

## <a name="members"></a><span data-ttu-id="cee6b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="cee6b-108">Members</span></span>
|<span data-ttu-id="cee6b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="cee6b-109">Member</span></span>|<span data-ttu-id="cee6b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="cee6b-110">Value</span></span>|<span data-ttu-id="cee6b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cee6b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cee6b-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="cee6b-112">notConfigured</span></span>|<span data-ttu-id="cee6b-113">,0</span><span class="sxs-lookup"><span data-stu-id="cee6b-113">0</span></span>|<span data-ttu-id="cee6b-114">O padrão é para pares na rede local.</span><span class="sxs-lookup"><span data-stu-id="cee6b-114">Defaults to peers in local network.</span></span>|
|<span data-ttu-id="cee6b-115">peersInLocalNetwork</span><span class="sxs-lookup"><span data-stu-id="cee6b-115">peersInLocalNetwork</span></span>|<span data-ttu-id="cee6b-116">1</span><span class="sxs-lookup"><span data-stu-id="cee6b-116">1</span></span>|<span data-ttu-id="cee6b-117">Os caches de conteúdo só serão iguais aos caches em sua rede local imediata.</span><span class="sxs-lookup"><span data-stu-id="cee6b-117">Content caches will only peer with caches in their immediate local network.</span></span>|
|<span data-ttu-id="cee6b-118">peersWithSamePublicIpAddress</span><span class="sxs-lookup"><span data-stu-id="cee6b-118">peersWithSamePublicIpAddress</span></span>|<span data-ttu-id="cee6b-119">duas</span><span class="sxs-lookup"><span data-stu-id="cee6b-119">2</span></span>|<span data-ttu-id="cee6b-120">Os caches de conteúdo só serão pontos com caches que compartilham o mesmo endereço IP público.</span><span class="sxs-lookup"><span data-stu-id="cee6b-120">Content caches will only peer with caches that share the same public IP address.</span></span>|
|<span data-ttu-id="cee6b-121">peersInCustomLocalNetworks</span><span class="sxs-lookup"><span data-stu-id="cee6b-121">peersInCustomLocalNetworks</span></span>|<span data-ttu-id="cee6b-122">3D</span><span class="sxs-lookup"><span data-stu-id="cee6b-122">3</span></span>|<span data-ttu-id="cee6b-123">Os caches de conteúdo usarão o contentCachingPeerFilterRanges e o contentCachingPeerListenRanges para determinar em que caches os pontos serão.</span><span class="sxs-lookup"><span data-stu-id="cee6b-123">Content caches will use contentCachingPeerFilterRanges and contentCachingPeerListenRanges to determine which caches to peer with.</span></span>|





