---
title: tipo de enum windowsAutopilotProfileAssignmentStatus
description: Ainda não documentado
ms.openlocfilehash: 0ec6dfaa6dbc87fe1d38a495ac177a84e70796a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033279"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="5b66a-103">tipo de enum windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="5b66a-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="5b66a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5b66a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b66a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5b66a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b66a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5b66a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b66a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5b66a-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="5b66a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5b66a-108">Members</span></span>
|<span data-ttu-id="5b66a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5b66a-109">Member</span></span>|<span data-ttu-id="5b66a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5b66a-110">Value</span></span>|<span data-ttu-id="5b66a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b66a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b66a-112">unknown</span><span class="sxs-lookup"><span data-stu-id="5b66a-112">unknown</span></span>|<span data-ttu-id="5b66a-113">0</span><span class="sxs-lookup"><span data-stu-id="5b66a-113">0</span></span>|<span data-ttu-id="5b66a-114">Status da atribuição desconhecido</span><span class="sxs-lookup"><span data-stu-id="5b66a-114">Unknown assignment status</span></span>|
|<span data-ttu-id="5b66a-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="5b66a-115">assignedInSync</span></span>|<span data-ttu-id="5b66a-116">1</span><span class="sxs-lookup"><span data-stu-id="5b66a-116">1</span></span>|<span data-ttu-id="5b66a-117">Em sincronia com o programa piloto do Windows automático e atribuídos com êxito no Intune</span><span class="sxs-lookup"><span data-stu-id="5b66a-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="5b66a-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="5b66a-118">assignedOutOfSync</span></span>|<span data-ttu-id="5b66a-119">2</span><span class="sxs-lookup"><span data-stu-id="5b66a-119">2</span></span>|<span data-ttu-id="5b66a-120">Não em sincronia com o programa piloto do Windows automático e atribuídos com êxito no Intune</span><span class="sxs-lookup"><span data-stu-id="5b66a-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="5b66a-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="5b66a-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="5b66a-122">3</span><span class="sxs-lookup"><span data-stu-id="5b66a-122">3</span></span>|<span data-ttu-id="5b66a-123">Atribuídos com êxito no Intune e qualquer em sincronia ou sair de sincronia com o programa piloto do Windows automático</span><span class="sxs-lookup"><span data-stu-id="5b66a-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="5b66a-124">não atribuído</span><span class="sxs-lookup"><span data-stu-id="5b66a-124">notAssigned</span></span>|<span data-ttu-id="5b66a-125">4</span><span class="sxs-lookup"><span data-stu-id="5b66a-125">4</span></span>|<span data-ttu-id="5b66a-126">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="5b66a-126">Not assigned</span></span>|
|<span data-ttu-id="5b66a-127">pendente</span><span class="sxs-lookup"><span data-stu-id="5b66a-127">pending</span></span>|<span data-ttu-id="5b66a-128">5</span><span class="sxs-lookup"><span data-stu-id="5b66a-128">5</span></span>|<span data-ttu-id="5b66a-129">Atribuição pendente</span><span class="sxs-lookup"><span data-stu-id="5b66a-129">Pending assignment</span></span>|
|<span data-ttu-id="5b66a-130">Falha</span><span class="sxs-lookup"><span data-stu-id="5b66a-130">failed</span></span>|<span data-ttu-id="5b66a-131">6</span><span class="sxs-lookup"><span data-stu-id="5b66a-131">6</span></span>| <span data-ttu-id="5b66a-132">Falha de atribuição</span><span class="sxs-lookup"><span data-stu-id="5b66a-132">Assignment failed</span></span>|





