---
title: tipo de enumeração applicationGuardBlockClipboardSharingType
description: Valores possíveis para applicationGuardBlockClipboardSharingType
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 89cfe40f949cf8daa5c7e2f68fa41366a498a31a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530939"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="d173f-103">tipo de enumeração applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="d173f-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="d173f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d173f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d173f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d173f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d173f-106">Valores possíveis para applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="d173f-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="d173f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d173f-107">Members</span></span>
|<span data-ttu-id="d173f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d173f-108">Member</span></span>|<span data-ttu-id="d173f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d173f-109">Value</span></span>|<span data-ttu-id="d173f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d173f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d173f-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d173f-111">notConfigured</span></span>|<span data-ttu-id="d173f-112">,0</span><span class="sxs-lookup"><span data-stu-id="d173f-112">0</span></span>|<span data-ttu-id="d173f-113">Não configurado</span><span class="sxs-lookup"><span data-stu-id="d173f-113">Not Configured</span></span>|
|<span data-ttu-id="d173f-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="d173f-114">blockBoth</span></span>|<span data-ttu-id="d173f-115">1 </span><span class="sxs-lookup"><span data-stu-id="d173f-115">1</span></span>|<span data-ttu-id="d173f-116">Bloquear a área de transferência para compartilhar dados do host para o contêiner e de contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="d173f-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="d173f-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="d173f-117">blockHostToContainer</span></span>|<span data-ttu-id="d173f-118">2 </span><span class="sxs-lookup"><span data-stu-id="d173f-118">2</span></span>|<span data-ttu-id="d173f-119">Bloquear a área de transferência para compartilhar dados do host para o contêiner</span><span class="sxs-lookup"><span data-stu-id="d173f-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="d173f-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="d173f-120">blockContainerToHost</span></span>|<span data-ttu-id="d173f-121">3 </span><span class="sxs-lookup"><span data-stu-id="d173f-121">3</span></span>|<span data-ttu-id="d173f-122">Bloquear área de transferência para compartilhar dados de contêiner para host</span><span class="sxs-lookup"><span data-stu-id="d173f-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="d173f-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="d173f-123">blockNone</span></span>|<span data-ttu-id="d173f-124">4 </span><span class="sxs-lookup"><span data-stu-id="d173f-124">4</span></span>|<span data-ttu-id="d173f-125">Bloquear área de transferência para compartilhar dados que não sejam do host para o contêiner nem do contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="d173f-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|




