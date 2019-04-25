---
title: tipo de enumeração windowsAutopilotProfileAssignmentStatus
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f4c6fbfcbefd88af31f2875cf33755b3be21e06
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525275"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="9ab93-103">tipo de enumeração windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="9ab93-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="9ab93-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ab93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ab93-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ab93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ab93-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9ab93-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="9ab93-107">Membros</span><span class="sxs-lookup"><span data-stu-id="9ab93-107">Members</span></span>
|<span data-ttu-id="9ab93-108">Membro</span><span class="sxs-lookup"><span data-stu-id="9ab93-108">Member</span></span>|<span data-ttu-id="9ab93-109">Valor</span><span class="sxs-lookup"><span data-stu-id="9ab93-109">Value</span></span>|<span data-ttu-id="9ab93-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ab93-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ab93-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="9ab93-111">unknown</span></span>|<span data-ttu-id="9ab93-112">,0</span><span class="sxs-lookup"><span data-stu-id="9ab93-112">0</span></span>|<span data-ttu-id="9ab93-113">Status de atribuição desconhecido</span><span class="sxs-lookup"><span data-stu-id="9ab93-113">Unknown assignment status</span></span>|
|<span data-ttu-id="9ab93-114">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="9ab93-114">assignedInSync</span></span>|<span data-ttu-id="9ab93-115">1 </span><span class="sxs-lookup"><span data-stu-id="9ab93-115">1</span></span>|<span data-ttu-id="9ab93-116">Atribuído com êxito no Intune e em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="9ab93-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="9ab93-117">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="9ab93-117">assignedOutOfSync</span></span>|<span data-ttu-id="9ab93-118">2 </span><span class="sxs-lookup"><span data-stu-id="9ab93-118">2</span></span>|<span data-ttu-id="9ab93-119">Atribuído com êxito no Intune e não em sincronia com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="9ab93-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="9ab93-120">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="9ab93-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="9ab93-121">3 </span><span class="sxs-lookup"><span data-stu-id="9ab93-121">3</span></span>|<span data-ttu-id="9ab93-122">Atribuído com êxito no Intune e em sincronia ou fora de sincronização com o programa piloto automático do Windows</span><span class="sxs-lookup"><span data-stu-id="9ab93-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="9ab93-123">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="9ab93-123">notAssigned</span></span>|<span data-ttu-id="9ab93-124">4 </span><span class="sxs-lookup"><span data-stu-id="9ab93-124">4</span></span>|<span data-ttu-id="9ab93-125">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="9ab93-125">Not assigned</span></span>|
|<span data-ttu-id="9ab93-126">função</span><span class="sxs-lookup"><span data-stu-id="9ab93-126">pending</span></span>|<span data-ttu-id="9ab93-127">5 </span><span class="sxs-lookup"><span data-stu-id="9ab93-127">5</span></span>|<span data-ttu-id="9ab93-128">Atribuição pendente</span><span class="sxs-lookup"><span data-stu-id="9ab93-128">Pending assignment</span></span>|
|<span data-ttu-id="9ab93-129">falhou</span><span class="sxs-lookup"><span data-stu-id="9ab93-129">failed</span></span>|<span data-ttu-id="9ab93-130">6 </span><span class="sxs-lookup"><span data-stu-id="9ab93-130">6</span></span>| <span data-ttu-id="9ab93-131">Falha de atribuição</span><span class="sxs-lookup"><span data-stu-id="9ab93-131">Assignment failed</span></span>|





