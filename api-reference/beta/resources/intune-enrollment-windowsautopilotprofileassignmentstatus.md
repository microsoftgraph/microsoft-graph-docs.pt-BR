---
title: tipo de enumeração windowsAutopilotProfileAssignmentStatus
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ce8fe0a165d46e9dd59ac88759093e12b60d2028
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031575"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="32556-103">tipo de enumeração windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="32556-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

<span data-ttu-id="32556-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32556-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32556-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="32556-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32556-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32556-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32556-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="32556-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="32556-108">Membros</span><span class="sxs-lookup"><span data-stu-id="32556-108">Members</span></span>
|<span data-ttu-id="32556-109">Membro</span><span class="sxs-lookup"><span data-stu-id="32556-109">Member</span></span>|<span data-ttu-id="32556-110">Valor</span><span class="sxs-lookup"><span data-stu-id="32556-110">Value</span></span>|<span data-ttu-id="32556-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="32556-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32556-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="32556-112">unknown</span></span>|<span data-ttu-id="32556-113">,0</span><span class="sxs-lookup"><span data-stu-id="32556-113">0</span></span>|<span data-ttu-id="32556-114">Status de atribuição desconhecido</span><span class="sxs-lookup"><span data-stu-id="32556-114">Unknown assignment status</span></span>|
|<span data-ttu-id="32556-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="32556-115">assignedInSync</span></span>|<span data-ttu-id="32556-116">1 </span><span class="sxs-lookup"><span data-stu-id="32556-116">1</span></span>|<span data-ttu-id="32556-117">Atribuído com êxito no Intune e em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="32556-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="32556-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="32556-118">assignedOutOfSync</span></span>|<span data-ttu-id="32556-119">2 </span><span class="sxs-lookup"><span data-stu-id="32556-119">2</span></span>|<span data-ttu-id="32556-120">Atribuído com êxito no Intune e não em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="32556-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="32556-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="32556-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="32556-122">3 </span><span class="sxs-lookup"><span data-stu-id="32556-122">3</span></span>|<span data-ttu-id="32556-123">Atribuído com êxito no Intune e em sincronia ou fora de sincronização com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="32556-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="32556-124">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="32556-124">notAssigned</span></span>|<span data-ttu-id="32556-125">4 </span><span class="sxs-lookup"><span data-stu-id="32556-125">4</span></span>|<span data-ttu-id="32556-126">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="32556-126">Not assigned</span></span>|
|<span data-ttu-id="32556-127">função</span><span class="sxs-lookup"><span data-stu-id="32556-127">pending</span></span>|<span data-ttu-id="32556-128">5 </span><span class="sxs-lookup"><span data-stu-id="32556-128">5</span></span>|<span data-ttu-id="32556-129">Atribuição pendente</span><span class="sxs-lookup"><span data-stu-id="32556-129">Pending assignment</span></span>|
|<span data-ttu-id="32556-130">falhou</span><span class="sxs-lookup"><span data-stu-id="32556-130">failed</span></span>|<span data-ttu-id="32556-131">6 </span><span class="sxs-lookup"><span data-stu-id="32556-131">6</span></span>| <span data-ttu-id="32556-132">Falha de atribuição</span><span class="sxs-lookup"><span data-stu-id="32556-132">Assignment failed</span></span>|






