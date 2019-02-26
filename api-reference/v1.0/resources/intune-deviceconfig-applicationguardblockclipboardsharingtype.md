---
title: tipo de enumeração applicationGuardBlockClipboardSharingType
description: Valores possíveis para applicationGuardBlockClipboardSharingType
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3d1b5132773bb0bf92f35c39b660726d7a1ef66
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261856"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="3a40b-103">tipo de enumeração applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="3a40b-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="3a40b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a40b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a40b-105">Valores possíveis para applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="3a40b-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="3a40b-106">Membros</span><span class="sxs-lookup"><span data-stu-id="3a40b-106">Members</span></span>
|<span data-ttu-id="3a40b-107">Membro</span><span class="sxs-lookup"><span data-stu-id="3a40b-107">Member</span></span>|<span data-ttu-id="3a40b-108">Valor</span><span class="sxs-lookup"><span data-stu-id="3a40b-108">Value</span></span>|<span data-ttu-id="3a40b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a40b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a40b-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3a40b-110">notConfigured</span></span>|<span data-ttu-id="3a40b-111">,0</span><span class="sxs-lookup"><span data-stu-id="3a40b-111">0</span></span>|<span data-ttu-id="3a40b-112">Não configurado</span><span class="sxs-lookup"><span data-stu-id="3a40b-112">Not Configured</span></span>|
|<span data-ttu-id="3a40b-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="3a40b-113">blockBoth</span></span>|<span data-ttu-id="3a40b-114">1</span><span class="sxs-lookup"><span data-stu-id="3a40b-114">1</span></span>|<span data-ttu-id="3a40b-115">Bloquear a área de transferência para compartilhar dados do host para o contêiner e de contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="3a40b-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="3a40b-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="3a40b-116">blockHostToContainer</span></span>|<span data-ttu-id="3a40b-117">duas</span><span class="sxs-lookup"><span data-stu-id="3a40b-117">2</span></span>|<span data-ttu-id="3a40b-118">Bloquear a área de transferência para compartilhar dados do host para o contêiner</span><span class="sxs-lookup"><span data-stu-id="3a40b-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="3a40b-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="3a40b-119">blockContainerToHost</span></span>|<span data-ttu-id="3a40b-120">3D</span><span class="sxs-lookup"><span data-stu-id="3a40b-120">3</span></span>|<span data-ttu-id="3a40b-121">Bloquear área de transferência para compartilhar dados de contêiner para host</span><span class="sxs-lookup"><span data-stu-id="3a40b-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="3a40b-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="3a40b-122">blockNone</span></span>|<span data-ttu-id="3a40b-123">quatro</span><span class="sxs-lookup"><span data-stu-id="3a40b-123">4</span></span>|<span data-ttu-id="3a40b-124">Bloquear área de transferência para compartilhar dados que não sejam do host para o contêiner nem do contêiner para o host</span><span class="sxs-lookup"><span data-stu-id="3a40b-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



