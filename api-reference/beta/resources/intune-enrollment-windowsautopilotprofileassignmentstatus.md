---
title: tipo de enumeração windowsAutopilotProfileAssignmentStatus
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3be930f3289891235a1462d0322323eb9b44bf60
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989746"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="7a224-103">tipo de enumeração windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="7a224-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="7a224-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7a224-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a224-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a224-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a224-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7a224-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="7a224-107">Membros</span><span class="sxs-lookup"><span data-stu-id="7a224-107">Members</span></span>
|<span data-ttu-id="7a224-108">Membro</span><span class="sxs-lookup"><span data-stu-id="7a224-108">Member</span></span>|<span data-ttu-id="7a224-109">Valor</span><span class="sxs-lookup"><span data-stu-id="7a224-109">Value</span></span>|<span data-ttu-id="7a224-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a224-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a224-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="7a224-111">unknown</span></span>|<span data-ttu-id="7a224-112">,0</span><span class="sxs-lookup"><span data-stu-id="7a224-112">0</span></span>|<span data-ttu-id="7a224-113">Status de atribuição desconhecido</span><span class="sxs-lookup"><span data-stu-id="7a224-113">Unknown assignment status</span></span>|
|<span data-ttu-id="7a224-114">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="7a224-114">assignedInSync</span></span>|<span data-ttu-id="7a224-115">1</span><span class="sxs-lookup"><span data-stu-id="7a224-115">1</span></span>|<span data-ttu-id="7a224-116">Atribuído com êxito no Intune e em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="7a224-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="7a224-117">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="7a224-117">assignedOutOfSync</span></span>|<span data-ttu-id="7a224-118">duas</span><span class="sxs-lookup"><span data-stu-id="7a224-118">2</span></span>|<span data-ttu-id="7a224-119">Atribuído com êxito no Intune e não em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="7a224-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="7a224-120">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="7a224-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="7a224-121">3D</span><span class="sxs-lookup"><span data-stu-id="7a224-121">3</span></span>|<span data-ttu-id="7a224-122">Atribuído com êxito no Intune e em sincronia ou fora de sincronização com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="7a224-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="7a224-123">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="7a224-123">notAssigned</span></span>|<span data-ttu-id="7a224-124">quatro</span><span class="sxs-lookup"><span data-stu-id="7a224-124">4</span></span>|<span data-ttu-id="7a224-125">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="7a224-125">Not assigned</span></span>|
|<span data-ttu-id="7a224-126">função</span><span class="sxs-lookup"><span data-stu-id="7a224-126">pending</span></span>|<span data-ttu-id="7a224-127">0,5</span><span class="sxs-lookup"><span data-stu-id="7a224-127">5</span></span>|<span data-ttu-id="7a224-128">Atribuição pendente</span><span class="sxs-lookup"><span data-stu-id="7a224-128">Pending assignment</span></span>|
|<span data-ttu-id="7a224-129">falhou</span><span class="sxs-lookup"><span data-stu-id="7a224-129">failed</span></span>|<span data-ttu-id="7a224-130">6</span><span class="sxs-lookup"><span data-stu-id="7a224-130">6</span></span>| <span data-ttu-id="7a224-131">Falha de atribuição</span><span class="sxs-lookup"><span data-stu-id="7a224-131">Assignment failed</span></span>|





