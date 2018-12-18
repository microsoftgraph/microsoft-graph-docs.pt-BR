---
title: tipo de enum windowsAutopilotProfileAssignmentStatus
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 255aab9770305baa29e73278b3bfceec1079351a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320997"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="018ca-103">tipo de enum windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="018ca-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="018ca-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="018ca-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="018ca-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="018ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="018ca-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="018ca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="018ca-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="018ca-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="018ca-108">Membros</span><span class="sxs-lookup"><span data-stu-id="018ca-108">Members</span></span>
|<span data-ttu-id="018ca-109">Membro</span><span class="sxs-lookup"><span data-stu-id="018ca-109">Member</span></span>|<span data-ttu-id="018ca-110">Valor</span><span class="sxs-lookup"><span data-stu-id="018ca-110">Value</span></span>|<span data-ttu-id="018ca-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="018ca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="018ca-112">unknown</span><span class="sxs-lookup"><span data-stu-id="018ca-112">unknown</span></span>|<span data-ttu-id="018ca-113">0</span><span class="sxs-lookup"><span data-stu-id="018ca-113">0</span></span>|<span data-ttu-id="018ca-114">Status da atribuição desconhecido</span><span class="sxs-lookup"><span data-stu-id="018ca-114">Unknown assignment status</span></span>|
|<span data-ttu-id="018ca-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="018ca-115">assignedInSync</span></span>|<span data-ttu-id="018ca-116">1</span><span class="sxs-lookup"><span data-stu-id="018ca-116">1</span></span>|<span data-ttu-id="018ca-117">Em sincronia com o programa piloto do Windows automático e atribuídos com êxito no Intune</span><span class="sxs-lookup"><span data-stu-id="018ca-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="018ca-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="018ca-118">assignedOutOfSync</span></span>|<span data-ttu-id="018ca-119">2</span><span class="sxs-lookup"><span data-stu-id="018ca-119">2</span></span>|<span data-ttu-id="018ca-120">Não em sincronia com o programa piloto do Windows automático e atribuídos com êxito no Intune</span><span class="sxs-lookup"><span data-stu-id="018ca-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="018ca-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="018ca-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="018ca-122">3</span><span class="sxs-lookup"><span data-stu-id="018ca-122">3</span></span>|<span data-ttu-id="018ca-123">Atribuídos com êxito no Intune e qualquer em sincronia ou sair de sincronia com o programa piloto do Windows automático</span><span class="sxs-lookup"><span data-stu-id="018ca-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="018ca-124">não atribuído</span><span class="sxs-lookup"><span data-stu-id="018ca-124">notAssigned</span></span>|<span data-ttu-id="018ca-125">4</span><span class="sxs-lookup"><span data-stu-id="018ca-125">4</span></span>|<span data-ttu-id="018ca-126">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="018ca-126">Not assigned</span></span>|
|<span data-ttu-id="018ca-127">pendente</span><span class="sxs-lookup"><span data-stu-id="018ca-127">pending</span></span>|<span data-ttu-id="018ca-128">5</span><span class="sxs-lookup"><span data-stu-id="018ca-128">5</span></span>|<span data-ttu-id="018ca-129">Atribuição pendente</span><span class="sxs-lookup"><span data-stu-id="018ca-129">Pending assignment</span></span>|
|<span data-ttu-id="018ca-130">Falha</span><span class="sxs-lookup"><span data-stu-id="018ca-130">failed</span></span>|<span data-ttu-id="018ca-131">6</span><span class="sxs-lookup"><span data-stu-id="018ca-131">6</span></span>| <span data-ttu-id="018ca-132">Falha de atribuição</span><span class="sxs-lookup"><span data-stu-id="018ca-132">Assignment failed</span></span>|





