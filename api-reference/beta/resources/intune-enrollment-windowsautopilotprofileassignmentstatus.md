---
title: tipo de enumeração windowsAutopilotProfileAssignmentStatus
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d241d93924de254af3cb76adfab27b49291b97f2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941391"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="c7e32-103">tipo de enumeração windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="c7e32-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="c7e32-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7e32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7e32-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7e32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7e32-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c7e32-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="c7e32-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c7e32-107">Members</span></span>
|<span data-ttu-id="c7e32-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c7e32-108">Member</span></span>|<span data-ttu-id="c7e32-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c7e32-109">Value</span></span>|<span data-ttu-id="c7e32-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7e32-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7e32-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="c7e32-111">unknown</span></span>|<span data-ttu-id="c7e32-112">,0</span><span class="sxs-lookup"><span data-stu-id="c7e32-112">0</span></span>|<span data-ttu-id="c7e32-113">Status de atribuição desconhecido</span><span class="sxs-lookup"><span data-stu-id="c7e32-113">Unknown assignment status</span></span>|
|<span data-ttu-id="c7e32-114">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="c7e32-114">assignedInSync</span></span>|<span data-ttu-id="c7e32-115">1</span><span class="sxs-lookup"><span data-stu-id="c7e32-115">1</span></span>|<span data-ttu-id="c7e32-116">Atribuído com êxito no Intune e em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="c7e32-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="c7e32-117">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="c7e32-117">assignedOutOfSync</span></span>|<span data-ttu-id="c7e32-118">duas</span><span class="sxs-lookup"><span data-stu-id="c7e32-118">2</span></span>|<span data-ttu-id="c7e32-119">Atribuído com êxito no Intune e não em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="c7e32-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="c7e32-120">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="c7e32-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="c7e32-121">3D</span><span class="sxs-lookup"><span data-stu-id="c7e32-121">3</span></span>|<span data-ttu-id="c7e32-122">Atribuído com êxito no Intune e em sincronia ou fora de sincronização com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="c7e32-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="c7e32-123">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="c7e32-123">notAssigned</span></span>|<span data-ttu-id="c7e32-124">quatro</span><span class="sxs-lookup"><span data-stu-id="c7e32-124">4</span></span>|<span data-ttu-id="c7e32-125">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="c7e32-125">Not assigned</span></span>|
|<span data-ttu-id="c7e32-126">função</span><span class="sxs-lookup"><span data-stu-id="c7e32-126">pending</span></span>|<span data-ttu-id="c7e32-127">0,5</span><span class="sxs-lookup"><span data-stu-id="c7e32-127">5</span></span>|<span data-ttu-id="c7e32-128">Atribuição pendente</span><span class="sxs-lookup"><span data-stu-id="c7e32-128">Pending assignment</span></span>|
|<span data-ttu-id="c7e32-129">falhou</span><span class="sxs-lookup"><span data-stu-id="c7e32-129">failed</span></span>|<span data-ttu-id="c7e32-130">6</span><span class="sxs-lookup"><span data-stu-id="c7e32-130">6</span></span>| <span data-ttu-id="c7e32-131">Falha de atribuição</span><span class="sxs-lookup"><span data-stu-id="c7e32-131">Assignment failed</span></span>|




