---
title: tipo de enumeração applicationGuardBlockClipboardSharingType
description: Valores possíveis para applicationGuardBlockClipboardSharingType
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d8aa4e34a9be5a3d2c3c9d8b0fa59635b7c16c6e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708883"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="5e8eb-103">tipo de enumeração applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="5e8eb-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="5e8eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e8eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e8eb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5e8eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e8eb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e8eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e8eb-107">Valores possíveis para applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="5e8eb-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="5e8eb-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5e8eb-108">Members</span></span>
|<span data-ttu-id="5e8eb-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5e8eb-109">Member</span></span>|<span data-ttu-id="5e8eb-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5e8eb-110">Value</span></span>|<span data-ttu-id="5e8eb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e8eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e8eb-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="5e8eb-112">notConfigured</span></span>|<span data-ttu-id="5e8eb-113">,0</span><span class="sxs-lookup"><span data-stu-id="5e8eb-113">0</span></span>|<span data-ttu-id="5e8eb-114">Não configurado</span><span class="sxs-lookup"><span data-stu-id="5e8eb-114">Not Configured</span></span>|
|<span data-ttu-id="5e8eb-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="5e8eb-115">blockBoth</span></span>|<span data-ttu-id="5e8eb-116">1</span><span class="sxs-lookup"><span data-stu-id="5e8eb-116">1</span></span>|<span data-ttu-id="5e8eb-117">Bloquear a área de transferência para compartilhar dados do host para o contêiner e de contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="5e8eb-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="5e8eb-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="5e8eb-118">blockHostToContainer</span></span>|<span data-ttu-id="5e8eb-119">duas</span><span class="sxs-lookup"><span data-stu-id="5e8eb-119">2</span></span>|<span data-ttu-id="5e8eb-120">Bloquear a área de transferência para compartilhar dados do host para o contêiner</span><span class="sxs-lookup"><span data-stu-id="5e8eb-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="5e8eb-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="5e8eb-121">blockContainerToHost</span></span>|<span data-ttu-id="5e8eb-122">3D</span><span class="sxs-lookup"><span data-stu-id="5e8eb-122">3</span></span>|<span data-ttu-id="5e8eb-123">Bloquear área de transferência para compartilhar dados de contêiner para host</span><span class="sxs-lookup"><span data-stu-id="5e8eb-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="5e8eb-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="5e8eb-124">blockNone</span></span>|<span data-ttu-id="5e8eb-125">4 </span><span class="sxs-lookup"><span data-stu-id="5e8eb-125">4</span></span>|<span data-ttu-id="5e8eb-126">Bloquear área de transferência para compartilhar dados que não sejam do host para o contêiner nem do contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="5e8eb-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





