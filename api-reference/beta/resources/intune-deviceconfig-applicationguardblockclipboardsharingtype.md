---
title: tipo de enumeração applicationGuardBlockClipboardSharingType
description: Valores possíveis para applicationGuardBlockClipboardSharingType
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 445d3fb20bcd159979694093eac0b03f6a876072
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796044"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="f1547-103">tipo de enumeração applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="f1547-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="f1547-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f1547-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1547-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1547-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1547-106">Valores possíveis para applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="f1547-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="f1547-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f1547-107">Members</span></span>
|<span data-ttu-id="f1547-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f1547-108">Member</span></span>|<span data-ttu-id="f1547-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f1547-109">Value</span></span>|<span data-ttu-id="f1547-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1547-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1547-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f1547-111">notConfigured</span></span>|<span data-ttu-id="f1547-112">,0</span><span class="sxs-lookup"><span data-stu-id="f1547-112">0</span></span>|<span data-ttu-id="f1547-113">Não configurado</span><span class="sxs-lookup"><span data-stu-id="f1547-113">Not Configured</span></span>|
|<span data-ttu-id="f1547-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="f1547-114">blockBoth</span></span>|<span data-ttu-id="f1547-115">1</span><span class="sxs-lookup"><span data-stu-id="f1547-115">1</span></span>|<span data-ttu-id="f1547-116">Bloquear a área de transferência para compartilhar dados do host para o contêiner e de contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="f1547-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="f1547-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="f1547-117">blockHostToContainer</span></span>|<span data-ttu-id="f1547-118">duas</span><span class="sxs-lookup"><span data-stu-id="f1547-118">2</span></span>|<span data-ttu-id="f1547-119">Bloquear a área de transferência para compartilhar dados do host para o contêiner</span><span class="sxs-lookup"><span data-stu-id="f1547-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="f1547-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="f1547-120">blockContainerToHost</span></span>|<span data-ttu-id="f1547-121">3D</span><span class="sxs-lookup"><span data-stu-id="f1547-121">3</span></span>|<span data-ttu-id="f1547-122">Bloquear área de transferência para compartilhar dados de contêiner para host</span><span class="sxs-lookup"><span data-stu-id="f1547-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="f1547-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="f1547-123">blockNone</span></span>|<span data-ttu-id="f1547-124">4 </span><span class="sxs-lookup"><span data-stu-id="f1547-124">4</span></span>|<span data-ttu-id="f1547-125">Bloquear área de transferência para compartilhar dados que não sejam do host para o contêiner nem do contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="f1547-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



