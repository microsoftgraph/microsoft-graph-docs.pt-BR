---
title: tipo de enumeração applicationGuardBlockClipboardSharingType
description: Valores possíveis para applicationGuardBlockClipboardSharingType
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83a0adf84ea57e6afa1749d1f6f7152403847b5f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806598"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="39cb5-103">tipo de enumeração applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="39cb5-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="39cb5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="39cb5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39cb5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39cb5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39cb5-106">Valores possíveis para applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="39cb5-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="39cb5-107">Membros</span><span class="sxs-lookup"><span data-stu-id="39cb5-107">Members</span></span>
|<span data-ttu-id="39cb5-108">Membro</span><span class="sxs-lookup"><span data-stu-id="39cb5-108">Member</span></span>|<span data-ttu-id="39cb5-109">Valor</span><span class="sxs-lookup"><span data-stu-id="39cb5-109">Value</span></span>|<span data-ttu-id="39cb5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="39cb5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39cb5-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="39cb5-111">notConfigured</span></span>|<span data-ttu-id="39cb5-112">,0</span><span class="sxs-lookup"><span data-stu-id="39cb5-112">0</span></span>|<span data-ttu-id="39cb5-113">Não configurado</span><span class="sxs-lookup"><span data-stu-id="39cb5-113">Not Configured</span></span>|
|<span data-ttu-id="39cb5-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="39cb5-114">blockBoth</span></span>|<span data-ttu-id="39cb5-115">1</span><span class="sxs-lookup"><span data-stu-id="39cb5-115">1</span></span>|<span data-ttu-id="39cb5-116">Bloquear a área de transferência para compartilhar dados do host para o contêiner e de contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="39cb5-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="39cb5-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="39cb5-117">blockHostToContainer</span></span>|<span data-ttu-id="39cb5-118">duas</span><span class="sxs-lookup"><span data-stu-id="39cb5-118">2</span></span>|<span data-ttu-id="39cb5-119">Bloquear a área de transferência para compartilhar dados do host para o contêiner</span><span class="sxs-lookup"><span data-stu-id="39cb5-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="39cb5-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="39cb5-120">blockContainerToHost</span></span>|<span data-ttu-id="39cb5-121">3D</span><span class="sxs-lookup"><span data-stu-id="39cb5-121">3</span></span>|<span data-ttu-id="39cb5-122">Bloquear área de transferência para compartilhar dados de contêiner para host</span><span class="sxs-lookup"><span data-stu-id="39cb5-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="39cb5-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="39cb5-123">blockNone</span></span>|<span data-ttu-id="39cb5-124">quatro</span><span class="sxs-lookup"><span data-stu-id="39cb5-124">4</span></span>|<span data-ttu-id="39cb5-125">Bloquear área de transferência para compartilhar dados que não sejam do host para o contêiner nem do contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="39cb5-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





