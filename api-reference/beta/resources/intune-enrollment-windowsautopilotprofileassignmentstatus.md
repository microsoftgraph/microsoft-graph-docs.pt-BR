---
title: tipo de enumeração windowsAutopilotProfileAssignmentStatus
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 93a956fa874fb50257da62fc9dbea59768e7a3cb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728904"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="4919f-103">tipo de enumeração windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="4919f-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

<span data-ttu-id="4919f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4919f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4919f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4919f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4919f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4919f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4919f-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4919f-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="4919f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4919f-108">Members</span></span>
|<span data-ttu-id="4919f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4919f-109">Member</span></span>|<span data-ttu-id="4919f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4919f-110">Value</span></span>|<span data-ttu-id="4919f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4919f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4919f-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="4919f-112">unknown</span></span>|<span data-ttu-id="4919f-113">,0</span><span class="sxs-lookup"><span data-stu-id="4919f-113">0</span></span>|<span data-ttu-id="4919f-114">Status de atribuição desconhecido</span><span class="sxs-lookup"><span data-stu-id="4919f-114">Unknown assignment status</span></span>|
|<span data-ttu-id="4919f-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="4919f-115">assignedInSync</span></span>|<span data-ttu-id="4919f-116">1</span><span class="sxs-lookup"><span data-stu-id="4919f-116">1</span></span>|<span data-ttu-id="4919f-117">Atribuído com êxito no Intune e em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="4919f-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="4919f-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="4919f-118">assignedOutOfSync</span></span>|<span data-ttu-id="4919f-119">duas</span><span class="sxs-lookup"><span data-stu-id="4919f-119">2</span></span>|<span data-ttu-id="4919f-120">Atribuído com êxito no Intune e não em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="4919f-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="4919f-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="4919f-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="4919f-122">3D</span><span class="sxs-lookup"><span data-stu-id="4919f-122">3</span></span>|<span data-ttu-id="4919f-123">Atribuído com êxito no Intune e em sincronia ou fora de sincronização com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="4919f-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="4919f-124">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="4919f-124">notAssigned</span></span>|<span data-ttu-id="4919f-125">4 </span><span class="sxs-lookup"><span data-stu-id="4919f-125">4</span></span>|<span data-ttu-id="4919f-126">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="4919f-126">Not assigned</span></span>|
|<span data-ttu-id="4919f-127">função</span><span class="sxs-lookup"><span data-stu-id="4919f-127">pending</span></span>|<span data-ttu-id="4919f-128">5 </span><span class="sxs-lookup"><span data-stu-id="4919f-128">5</span></span>|<span data-ttu-id="4919f-129">Atribuição pendente</span><span class="sxs-lookup"><span data-stu-id="4919f-129">Pending assignment</span></span>|
|<span data-ttu-id="4919f-130">falhou</span><span class="sxs-lookup"><span data-stu-id="4919f-130">failed</span></span>|<span data-ttu-id="4919f-131">6 </span><span class="sxs-lookup"><span data-stu-id="4919f-131">6</span></span>| <span data-ttu-id="4919f-132">Falha de atribuição</span><span class="sxs-lookup"><span data-stu-id="4919f-132">Assignment failed</span></span>|





