---
title: tipo de enumeração macOSContentCachingType
description: Indica o tipo de conteúdo que pode ser armazenado em cache pelo serviço de cache de conteúdo da Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9022b320507cc10455e2eeb3ebd3a3ca58d52f71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993837"
---
# <a name="macoscontentcachingtype-enum-type"></a><span data-ttu-id="15bd4-103">tipo de enumeração macOSContentCachingType</span><span class="sxs-lookup"><span data-stu-id="15bd4-103">macOSContentCachingType enum type</span></span>

<span data-ttu-id="15bd4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15bd4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15bd4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="15bd4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15bd4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15bd4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15bd4-107">Indica o tipo de conteúdo que pode ser armazenado em cache pelo serviço de cache de conteúdo da Apple.</span><span class="sxs-lookup"><span data-stu-id="15bd4-107">Indicates the type of content allowed to be cached by Apple's content caching service.</span></span>

## <a name="members"></a><span data-ttu-id="15bd4-108">Membros</span><span class="sxs-lookup"><span data-stu-id="15bd4-108">Members</span></span>
|<span data-ttu-id="15bd4-109">Membro</span><span class="sxs-lookup"><span data-stu-id="15bd4-109">Member</span></span>|<span data-ttu-id="15bd4-110">Valor</span><span class="sxs-lookup"><span data-stu-id="15bd4-110">Value</span></span>|<span data-ttu-id="15bd4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="15bd4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15bd4-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="15bd4-112">notConfigured</span></span>|<span data-ttu-id="15bd4-113">,0</span><span class="sxs-lookup"><span data-stu-id="15bd4-113">0</span></span>|<span data-ttu-id="15bd4-114">Padrão.</span><span class="sxs-lookup"><span data-stu-id="15bd4-114">Default.</span></span> <span data-ttu-id="15bd4-115">Os dados de iCloud do usuário e os dados não iCloud serão armazenados em cache.</span><span class="sxs-lookup"><span data-stu-id="15bd4-115">Both user iCloud data and non-iCloud data will be cached.</span></span>|
|<span data-ttu-id="15bd4-116">userContentOnly</span><span class="sxs-lookup"><span data-stu-id="15bd4-116">userContentOnly</span></span>|<span data-ttu-id="15bd4-117">1 </span><span class="sxs-lookup"><span data-stu-id="15bd4-117">1</span></span>|<span data-ttu-id="15bd4-118">Permitir que o serviço de cache de conteúdo da Apple armazene em cache os dados do iCloud.</span><span class="sxs-lookup"><span data-stu-id="15bd4-118">Allow Apple's content caching service to cache user iCloud data.</span></span>|
|<span data-ttu-id="15bd4-119">sharedContentOnly</span><span class="sxs-lookup"><span data-stu-id="15bd4-119">sharedContentOnly</span></span>|<span data-ttu-id="15bd4-120">2 </span><span class="sxs-lookup"><span data-stu-id="15bd4-120">2</span></span>|<span data-ttu-id="15bd4-121">Permitir que o serviço de cache de conteúdo da Apple armazene em cache dados não iCloud (por exemplo, atualizações de aplicativo e software).</span><span class="sxs-lookup"><span data-stu-id="15bd4-121">Allow Apple's content caching service to cache non-iCloud data (e.g. app and software updates).</span></span>|






