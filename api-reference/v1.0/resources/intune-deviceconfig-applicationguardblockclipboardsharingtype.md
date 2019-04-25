---
title: tipo de enumeração applicationGuardBlockClipboardSharingType
description: Valores possíveis para applicationGuardBlockClipboardSharingType
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3d1b5132773bb0bf92f35c39b660726d7a1ef66
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575076"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="f7552-103">tipo de enumeração applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="f7552-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="f7552-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7552-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7552-105">Valores possíveis para applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="f7552-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="f7552-106">Membros</span><span class="sxs-lookup"><span data-stu-id="f7552-106">Members</span></span>
|<span data-ttu-id="f7552-107">Membro</span><span class="sxs-lookup"><span data-stu-id="f7552-107">Member</span></span>|<span data-ttu-id="f7552-108">Valor</span><span class="sxs-lookup"><span data-stu-id="f7552-108">Value</span></span>|<span data-ttu-id="f7552-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7552-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7552-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f7552-110">notConfigured</span></span>|<span data-ttu-id="f7552-111">,0</span><span class="sxs-lookup"><span data-stu-id="f7552-111">0</span></span>|<span data-ttu-id="f7552-112">Não configurado</span><span class="sxs-lookup"><span data-stu-id="f7552-112">Not Configured</span></span>|
|<span data-ttu-id="f7552-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="f7552-113">blockBoth</span></span>|<span data-ttu-id="f7552-114">1 </span><span class="sxs-lookup"><span data-stu-id="f7552-114">1</span></span>|<span data-ttu-id="f7552-115">Bloquear a área de transferência para compartilhar dados do host para o contêiner e de contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="f7552-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="f7552-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="f7552-116">blockHostToContainer</span></span>|<span data-ttu-id="f7552-117">2 </span><span class="sxs-lookup"><span data-stu-id="f7552-117">2</span></span>|<span data-ttu-id="f7552-118">Bloquear a área de transferência para compartilhar dados do host para o contêiner</span><span class="sxs-lookup"><span data-stu-id="f7552-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="f7552-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="f7552-119">blockContainerToHost</span></span>|<span data-ttu-id="f7552-120">3 </span><span class="sxs-lookup"><span data-stu-id="f7552-120">3</span></span>|<span data-ttu-id="f7552-121">Bloquear área de transferência para compartilhar dados de contêiner para host</span><span class="sxs-lookup"><span data-stu-id="f7552-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="f7552-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="f7552-122">blockNone</span></span>|<span data-ttu-id="f7552-123">4 </span><span class="sxs-lookup"><span data-stu-id="f7552-123">4</span></span>|<span data-ttu-id="f7552-124">Bloquear área de transferência para compartilhar dados que não sejam do host para o contêiner nem do contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="f7552-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



