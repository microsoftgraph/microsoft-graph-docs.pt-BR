---
title: tipo de enumeração applicationGuardBlockClipboardSharingType
description: Valores possíveis para applicationGuardBlockClipboardSharingType
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58c2a30a1dd1bf7e848cd6db702a002731bcaf7a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527115"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="e886b-103">tipo de enumeração applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="e886b-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="e886b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e886b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e886b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e886b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e886b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e886b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e886b-107">Valores possíveis para applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="e886b-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="e886b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e886b-108">Members</span></span>
|<span data-ttu-id="e886b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e886b-109">Member</span></span>|<span data-ttu-id="e886b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e886b-110">Value</span></span>|<span data-ttu-id="e886b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e886b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e886b-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e886b-112">notConfigured</span></span>|<span data-ttu-id="e886b-113">,0</span><span class="sxs-lookup"><span data-stu-id="e886b-113">0</span></span>|<span data-ttu-id="e886b-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="e886b-114">Not Configured</span></span>|
|<span data-ttu-id="e886b-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="e886b-115">blockBoth</span></span>|<span data-ttu-id="e886b-116">1 </span><span class="sxs-lookup"><span data-stu-id="e886b-116">1</span></span>|<span data-ttu-id="e886b-117">Bloquear a área de transferência para compartilhar dados do host para o contêiner e de contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="e886b-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="e886b-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="e886b-118">blockHostToContainer</span></span>|<span data-ttu-id="e886b-119">2 </span><span class="sxs-lookup"><span data-stu-id="e886b-119">2</span></span>|<span data-ttu-id="e886b-120">Bloquear a área de transferência para compartilhar dados do host para o contêiner</span><span class="sxs-lookup"><span data-stu-id="e886b-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="e886b-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="e886b-121">blockContainerToHost</span></span>|<span data-ttu-id="e886b-122">3 </span><span class="sxs-lookup"><span data-stu-id="e886b-122">3</span></span>|<span data-ttu-id="e886b-123">Bloquear área de transferência para compartilhar dados de contêiner para host</span><span class="sxs-lookup"><span data-stu-id="e886b-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="e886b-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="e886b-124">blockNone</span></span>|<span data-ttu-id="e886b-125">4 </span><span class="sxs-lookup"><span data-stu-id="e886b-125">4</span></span>|<span data-ttu-id="e886b-126">Bloquear área de transferência para compartilhar dados que não sejam do host para o contêiner nem do contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="e886b-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



