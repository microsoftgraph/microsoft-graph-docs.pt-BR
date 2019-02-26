---
title: tipo de enumeração windowsAutopilotProfileAssignmentStatus
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5d1af0e6c91dced1aa12ae72c22430d16674c21
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156375"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="bd922-103">tipo de enumeração windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="bd922-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="bd922-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bd922-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd922-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bd922-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd922-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bd922-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="bd922-107">Membros</span><span class="sxs-lookup"><span data-stu-id="bd922-107">Members</span></span>
|<span data-ttu-id="bd922-108">Membro</span><span class="sxs-lookup"><span data-stu-id="bd922-108">Member</span></span>|<span data-ttu-id="bd922-109">Valor</span><span class="sxs-lookup"><span data-stu-id="bd922-109">Value</span></span>|<span data-ttu-id="bd922-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd922-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd922-111">unknown</span><span class="sxs-lookup"><span data-stu-id="bd922-111">unknown</span></span>|<span data-ttu-id="bd922-112">,0</span><span class="sxs-lookup"><span data-stu-id="bd922-112">0</span></span>|<span data-ttu-id="bd922-113">Status de atribuição desconhecido</span><span class="sxs-lookup"><span data-stu-id="bd922-113">Unknown assignment status</span></span>|
|<span data-ttu-id="bd922-114">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="bd922-114">assignedInSync</span></span>|<span data-ttu-id="bd922-115">1</span><span class="sxs-lookup"><span data-stu-id="bd922-115">1</span></span>|<span data-ttu-id="bd922-116">Atribuído com êxito no Intune e em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="bd922-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="bd922-117">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="bd922-117">assignedOutOfSync</span></span>|<span data-ttu-id="bd922-118">duas</span><span class="sxs-lookup"><span data-stu-id="bd922-118">2</span></span>|<span data-ttu-id="bd922-119">Atribuído com êxito no Intune e não em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="bd922-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="bd922-120">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="bd922-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="bd922-121">3D</span><span class="sxs-lookup"><span data-stu-id="bd922-121">3</span></span>|<span data-ttu-id="bd922-122">Atribuído com êxito no Intune e em sincronia ou fora de sincronização com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="bd922-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="bd922-123">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="bd922-123">notAssigned</span></span>|<span data-ttu-id="bd922-124">quatro</span><span class="sxs-lookup"><span data-stu-id="bd922-124">4</span></span>|<span data-ttu-id="bd922-125">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="bd922-125">Not assigned</span></span>|
|<span data-ttu-id="bd922-126">função</span><span class="sxs-lookup"><span data-stu-id="bd922-126">pending</span></span>|<span data-ttu-id="bd922-127">0,5</span><span class="sxs-lookup"><span data-stu-id="bd922-127">5</span></span>|<span data-ttu-id="bd922-128">Atribuição pendente</span><span class="sxs-lookup"><span data-stu-id="bd922-128">Pending assignment</span></span>|
|<span data-ttu-id="bd922-129">falhou</span><span class="sxs-lookup"><span data-stu-id="bd922-129">failed</span></span>|<span data-ttu-id="bd922-130">6</span><span class="sxs-lookup"><span data-stu-id="bd922-130">6</span></span>| <span data-ttu-id="bd922-131">Falha de atribuição</span><span class="sxs-lookup"><span data-stu-id="bd922-131">Assignment failed</span></span>|




