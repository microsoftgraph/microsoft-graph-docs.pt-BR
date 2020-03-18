---
title: tipo de enumeração windowsAutopilotProfileAssignmentStatus
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7100e5881049900bb474e20060ac916ec1199a29
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783365"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="e0650-103">tipo de enumeração windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="e0650-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="e0650-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0650-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0650-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0650-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0650-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e0650-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="e0650-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e0650-107">Members</span></span>
|<span data-ttu-id="e0650-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e0650-108">Member</span></span>|<span data-ttu-id="e0650-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e0650-109">Value</span></span>|<span data-ttu-id="e0650-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0650-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0650-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="e0650-111">unknown</span></span>|<span data-ttu-id="e0650-112">,0</span><span class="sxs-lookup"><span data-stu-id="e0650-112">0</span></span>|<span data-ttu-id="e0650-113">Status de atribuição desconhecido</span><span class="sxs-lookup"><span data-stu-id="e0650-113">Unknown assignment status</span></span>|
|<span data-ttu-id="e0650-114">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="e0650-114">assignedInSync</span></span>|<span data-ttu-id="e0650-115">1</span><span class="sxs-lookup"><span data-stu-id="e0650-115">1</span></span>|<span data-ttu-id="e0650-116">Atribuído com êxito no Intune e em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="e0650-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="e0650-117">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="e0650-117">assignedOutOfSync</span></span>|<span data-ttu-id="e0650-118">duas</span><span class="sxs-lookup"><span data-stu-id="e0650-118">2</span></span>|<span data-ttu-id="e0650-119">Atribuído com êxito no Intune e não em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="e0650-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="e0650-120">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="e0650-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="e0650-121">3D</span><span class="sxs-lookup"><span data-stu-id="e0650-121">3</span></span>|<span data-ttu-id="e0650-122">Atribuído com êxito no Intune e em sincronia ou fora de sincronização com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="e0650-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="e0650-123">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="e0650-123">notAssigned</span></span>|<span data-ttu-id="e0650-124">4 </span><span class="sxs-lookup"><span data-stu-id="e0650-124">4</span></span>|<span data-ttu-id="e0650-125">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="e0650-125">Not assigned</span></span>|
|<span data-ttu-id="e0650-126">função</span><span class="sxs-lookup"><span data-stu-id="e0650-126">pending</span></span>|<span data-ttu-id="e0650-127">5 </span><span class="sxs-lookup"><span data-stu-id="e0650-127">5</span></span>|<span data-ttu-id="e0650-128">Atribuição pendente</span><span class="sxs-lookup"><span data-stu-id="e0650-128">Pending assignment</span></span>|
|<span data-ttu-id="e0650-129">falhou</span><span class="sxs-lookup"><span data-stu-id="e0650-129">failed</span></span>|<span data-ttu-id="e0650-130">6 </span><span class="sxs-lookup"><span data-stu-id="e0650-130">6</span></span>| <span data-ttu-id="e0650-131">Falha de atribuição</span><span class="sxs-lookup"><span data-stu-id="e0650-131">Assignment failed</span></span>|



