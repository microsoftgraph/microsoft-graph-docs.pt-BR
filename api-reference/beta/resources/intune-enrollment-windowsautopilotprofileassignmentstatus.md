---
title: tipo de enum windowsAutopilotProfileAssignmentStatus
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 68612e2f4ccee46612c82237630efafda484b7e9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419118"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="e6085-103">tipo de enum windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="e6085-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="e6085-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e6085-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e6085-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e6085-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6085-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e6085-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6085-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e6085-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="e6085-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e6085-108">Members</span></span>
|<span data-ttu-id="e6085-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e6085-109">Member</span></span>|<span data-ttu-id="e6085-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e6085-110">Value</span></span>|<span data-ttu-id="e6085-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6085-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6085-112">unknown</span><span class="sxs-lookup"><span data-stu-id="e6085-112">unknown</span></span>|<span data-ttu-id="e6085-113">0</span><span class="sxs-lookup"><span data-stu-id="e6085-113">0</span></span>|<span data-ttu-id="e6085-114">Status da atribuição desconhecido</span><span class="sxs-lookup"><span data-stu-id="e6085-114">Unknown assignment status</span></span>|
|<span data-ttu-id="e6085-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="e6085-115">assignedInSync</span></span>|<span data-ttu-id="e6085-116">1</span><span class="sxs-lookup"><span data-stu-id="e6085-116">1</span></span>|<span data-ttu-id="e6085-117">Em sincronia com o programa piloto do Windows automático e atribuídos com êxito no Intune</span><span class="sxs-lookup"><span data-stu-id="e6085-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="e6085-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="e6085-118">assignedOutOfSync</span></span>|<span data-ttu-id="e6085-119">2</span><span class="sxs-lookup"><span data-stu-id="e6085-119">2</span></span>|<span data-ttu-id="e6085-120">Não em sincronia com o programa piloto do Windows automático e atribuídos com êxito no Intune</span><span class="sxs-lookup"><span data-stu-id="e6085-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="e6085-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="e6085-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="e6085-122">3</span><span class="sxs-lookup"><span data-stu-id="e6085-122">3</span></span>|<span data-ttu-id="e6085-123">Atribuídos com êxito no Intune e qualquer em sincronia ou sair de sincronia com o programa piloto do Windows automático</span><span class="sxs-lookup"><span data-stu-id="e6085-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="e6085-124">não atribuído</span><span class="sxs-lookup"><span data-stu-id="e6085-124">notAssigned</span></span>|<span data-ttu-id="e6085-125">4</span><span class="sxs-lookup"><span data-stu-id="e6085-125">4</span></span>|<span data-ttu-id="e6085-126">Não atribuído</span><span class="sxs-lookup"><span data-stu-id="e6085-126">Not assigned</span></span>|
|<span data-ttu-id="e6085-127">pendente</span><span class="sxs-lookup"><span data-stu-id="e6085-127">pending</span></span>|<span data-ttu-id="e6085-128">5</span><span class="sxs-lookup"><span data-stu-id="e6085-128">5</span></span>|<span data-ttu-id="e6085-129">Atribuição pendente</span><span class="sxs-lookup"><span data-stu-id="e6085-129">Pending assignment</span></span>|
|<span data-ttu-id="e6085-130">Falha</span><span class="sxs-lookup"><span data-stu-id="e6085-130">failed</span></span>|<span data-ttu-id="e6085-131">6</span><span class="sxs-lookup"><span data-stu-id="e6085-131">6</span></span>| <span data-ttu-id="e6085-132">Falha de atribuição</span><span class="sxs-lookup"><span data-stu-id="e6085-132">Assignment failed</span></span>|




