---
title: tipo de enumeração applicationGuardBlockClipboardSharingType
description: Valores possíveis para applicationGuardBlockClipboardSharingType
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 91c2bceba0d4ffda030266d0f5617ce18ab29f68
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49216378"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="d7890-103">tipo de enumeração applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="d7890-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="d7890-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7890-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7890-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d7890-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7890-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7890-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7890-107">Valores possíveis para applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="d7890-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="d7890-108">Membros</span><span class="sxs-lookup"><span data-stu-id="d7890-108">Members</span></span>
|<span data-ttu-id="d7890-109">Membro</span><span class="sxs-lookup"><span data-stu-id="d7890-109">Member</span></span>|<span data-ttu-id="d7890-110">Valor</span><span class="sxs-lookup"><span data-stu-id="d7890-110">Value</span></span>|<span data-ttu-id="d7890-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7890-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7890-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d7890-112">notConfigured</span></span>|<span data-ttu-id="d7890-113">,0</span><span class="sxs-lookup"><span data-stu-id="d7890-113">0</span></span>|<span data-ttu-id="d7890-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="d7890-114">Not Configured</span></span>|
|<span data-ttu-id="d7890-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="d7890-115">blockBoth</span></span>|<span data-ttu-id="d7890-116">1</span><span class="sxs-lookup"><span data-stu-id="d7890-116">1</span></span>|<span data-ttu-id="d7890-117">Bloquear a área de transferência para compartilhar dados do host para o contêiner e de contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="d7890-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="d7890-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="d7890-118">blockHostToContainer</span></span>|<span data-ttu-id="d7890-119">duas</span><span class="sxs-lookup"><span data-stu-id="d7890-119">2</span></span>|<span data-ttu-id="d7890-120">Bloquear a área de transferência para compartilhar dados do host para o contêiner</span><span class="sxs-lookup"><span data-stu-id="d7890-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="d7890-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="d7890-121">blockContainerToHost</span></span>|<span data-ttu-id="d7890-122">3D</span><span class="sxs-lookup"><span data-stu-id="d7890-122">3</span></span>|<span data-ttu-id="d7890-123">Bloquear área de transferência para compartilhar dados de contêiner para host</span><span class="sxs-lookup"><span data-stu-id="d7890-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="d7890-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="d7890-124">blockNone</span></span>|<span data-ttu-id="d7890-125">4 </span><span class="sxs-lookup"><span data-stu-id="d7890-125">4</span></span>|<span data-ttu-id="d7890-126">Bloquear área de transferência para compartilhar dados que não sejam do host para o contêiner nem do contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="d7890-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|




