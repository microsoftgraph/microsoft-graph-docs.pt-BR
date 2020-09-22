---
title: tipo de enumeração applicationGuardBlockClipboardSharingType
description: Valores possíveis para applicationGuardBlockClipboardSharingType
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 51f259fbd201869de2c69a019fa17f674fd095c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051169"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="14532-103">tipo de enumeração applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="14532-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="14532-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14532-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14532-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14532-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14532-106">Valores possíveis para applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="14532-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="14532-107">Membros</span><span class="sxs-lookup"><span data-stu-id="14532-107">Members</span></span>
|<span data-ttu-id="14532-108">Membro</span><span class="sxs-lookup"><span data-stu-id="14532-108">Member</span></span>|<span data-ttu-id="14532-109">Valor</span><span class="sxs-lookup"><span data-stu-id="14532-109">Value</span></span>|<span data-ttu-id="14532-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="14532-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14532-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="14532-111">notConfigured</span></span>|<span data-ttu-id="14532-112">,0</span><span class="sxs-lookup"><span data-stu-id="14532-112">0</span></span>|<span data-ttu-id="14532-113">Não configurado</span><span class="sxs-lookup"><span data-stu-id="14532-113">Not Configured</span></span>|
|<span data-ttu-id="14532-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="14532-114">blockBoth</span></span>|<span data-ttu-id="14532-115">1 </span><span class="sxs-lookup"><span data-stu-id="14532-115">1</span></span>|<span data-ttu-id="14532-116">Bloquear a área de transferência para compartilhar dados do host para o contêiner e de contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="14532-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="14532-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="14532-117">blockHostToContainer</span></span>|<span data-ttu-id="14532-118">2 </span><span class="sxs-lookup"><span data-stu-id="14532-118">2</span></span>|<span data-ttu-id="14532-119">Bloquear a área de transferência para compartilhar dados do host para o contêiner</span><span class="sxs-lookup"><span data-stu-id="14532-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="14532-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="14532-120">blockContainerToHost</span></span>|<span data-ttu-id="14532-121">3 </span><span class="sxs-lookup"><span data-stu-id="14532-121">3</span></span>|<span data-ttu-id="14532-122">Bloquear área de transferência para compartilhar dados de contêiner para host</span><span class="sxs-lookup"><span data-stu-id="14532-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="14532-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="14532-123">blockNone</span></span>|<span data-ttu-id="14532-124">4 </span><span class="sxs-lookup"><span data-stu-id="14532-124">4</span></span>|<span data-ttu-id="14532-125">Bloquear área de transferência para compartilhar dados que não sejam do host para o contêiner nem do contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="14532-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|









