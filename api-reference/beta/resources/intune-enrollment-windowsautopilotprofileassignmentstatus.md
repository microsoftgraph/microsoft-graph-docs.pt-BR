---
title: tipo de enumeração windowsAutopilotProfileAssignmentStatus
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a6ac21decb96434d7392e0d647ad4e9c2e07621f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288646"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="3c2f1-103">tipo de enumeração windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="3c2f1-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

<span data-ttu-id="3c2f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c2f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c2f1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c2f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c2f1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c2f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c2f1-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3c2f1-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="3c2f1-108">Membros</span><span class="sxs-lookup"><span data-stu-id="3c2f1-108">Members</span></span>
|<span data-ttu-id="3c2f1-109">Membro</span><span class="sxs-lookup"><span data-stu-id="3c2f1-109">Member</span></span>|<span data-ttu-id="3c2f1-110">Valor</span><span class="sxs-lookup"><span data-stu-id="3c2f1-110">Value</span></span>|<span data-ttu-id="3c2f1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c2f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c2f1-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="3c2f1-112">unknown</span></span>|<span data-ttu-id="3c2f1-113">,0</span><span class="sxs-lookup"><span data-stu-id="3c2f1-113">0</span></span>|<span data-ttu-id="3c2f1-114">Status de atribuição desconhecido</span><span class="sxs-lookup"><span data-stu-id="3c2f1-114">Unknown assignment status</span></span>|
|<span data-ttu-id="3c2f1-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="3c2f1-115">assignedInSync</span></span>|<span data-ttu-id="3c2f1-116">1</span><span class="sxs-lookup"><span data-stu-id="3c2f1-116">1</span></span>|<span data-ttu-id="3c2f1-117">Atribuído com êxito no Intune e em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="3c2f1-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="3c2f1-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="3c2f1-118">assignedOutOfSync</span></span>|<span data-ttu-id="3c2f1-119">duas</span><span class="sxs-lookup"><span data-stu-id="3c2f1-119">2</span></span>|<span data-ttu-id="3c2f1-120">Atribuído com êxito no Intune e não em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="3c2f1-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="3c2f1-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="3c2f1-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="3c2f1-122">3D</span><span class="sxs-lookup"><span data-stu-id="3c2f1-122">3</span></span>|<span data-ttu-id="3c2f1-123">Atribuído com êxito no Intune e em sincronia ou fora de sincronização com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="3c2f1-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="3c2f1-124">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="3c2f1-124">notAssigned</span></span>|<span data-ttu-id="3c2f1-125">4 </span><span class="sxs-lookup"><span data-stu-id="3c2f1-125">4</span></span>|<span data-ttu-id="3c2f1-126">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="3c2f1-126">Not assigned</span></span>|
|<span data-ttu-id="3c2f1-127">função</span><span class="sxs-lookup"><span data-stu-id="3c2f1-127">pending</span></span>|<span data-ttu-id="3c2f1-128">5 </span><span class="sxs-lookup"><span data-stu-id="3c2f1-128">5</span></span>|<span data-ttu-id="3c2f1-129">Atribuição pendente</span><span class="sxs-lookup"><span data-stu-id="3c2f1-129">Pending assignment</span></span>|
|<span data-ttu-id="3c2f1-130">falhou</span><span class="sxs-lookup"><span data-stu-id="3c2f1-130">failed</span></span>|<span data-ttu-id="3c2f1-131">6 </span><span class="sxs-lookup"><span data-stu-id="3c2f1-131">6</span></span>| <span data-ttu-id="3c2f1-132">Falha de atribuição</span><span class="sxs-lookup"><span data-stu-id="3c2f1-132">Assignment failed</span></span>|




