---
title: tipo de enumeração emailSyncSchedule
description: Valores possíveis para agenda de sincronização de email.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 63e0c1ffaed029ca5ba010181c70ab0588135a36
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49198871"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="a4d18-103">tipo de enumeração emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="a4d18-103">emailSyncSchedule enum type</span></span>

<span data-ttu-id="a4d18-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4d18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4d18-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a4d18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4d18-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a4d18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4d18-107">Valores possíveis para agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="a4d18-107">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="a4d18-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a4d18-108">Members</span></span>
|<span data-ttu-id="a4d18-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a4d18-109">Member</span></span>|<span data-ttu-id="a4d18-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a4d18-110">Value</span></span>|<span data-ttu-id="a4d18-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4d18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4d18-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="a4d18-112">userDefined</span></span>|<span data-ttu-id="a4d18-113">,0</span><span class="sxs-lookup"><span data-stu-id="a4d18-113">0</span></span>|<span data-ttu-id="a4d18-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="a4d18-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="a4d18-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="a4d18-115">asMessagesArrive</span></span>|<span data-ttu-id="a4d18-116">1</span><span class="sxs-lookup"><span data-stu-id="a4d18-116">1</span></span>|<span data-ttu-id="a4d18-117">Sincronizar à medida que as mensagens chegam.</span><span class="sxs-lookup"><span data-stu-id="a4d18-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="a4d18-118">Manual</span><span class="sxs-lookup"><span data-stu-id="a4d18-118">manual</span></span>|<span data-ttu-id="a4d18-119">duas</span><span class="sxs-lookup"><span data-stu-id="a4d18-119">2</span></span>|<span data-ttu-id="a4d18-120">Sincronizar manualmente.</span><span class="sxs-lookup"><span data-stu-id="a4d18-120">Sync manually.</span></span>|
|<span data-ttu-id="a4d18-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="a4d18-121">fifteenMinutes</span></span>|<span data-ttu-id="a4d18-122">3D</span><span class="sxs-lookup"><span data-stu-id="a4d18-122">3</span></span>|<span data-ttu-id="a4d18-123">Sincronizar a cada quinze minutos.</span><span class="sxs-lookup"><span data-stu-id="a4d18-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="a4d18-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="a4d18-124">thirtyMinutes</span></span>|<span data-ttu-id="a4d18-125">4 </span><span class="sxs-lookup"><span data-stu-id="a4d18-125">4</span></span>|<span data-ttu-id="a4d18-126">Sincronizar a cada trinta minutos.</span><span class="sxs-lookup"><span data-stu-id="a4d18-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="a4d18-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="a4d18-127">sixtyMinutes</span></span>|<span data-ttu-id="a4d18-128">5 </span><span class="sxs-lookup"><span data-stu-id="a4d18-128">5</span></span>|<span data-ttu-id="a4d18-129">Sincronizar a cada 60 minutos.</span><span class="sxs-lookup"><span data-stu-id="a4d18-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="a4d18-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="a4d18-130">basedOnMyUsage</span></span>|<span data-ttu-id="a4d18-131">6 </span><span class="sxs-lookup"><span data-stu-id="a4d18-131">6</span></span>|<span data-ttu-id="a4d18-132">Sincronizar com base no meu uso.</span><span class="sxs-lookup"><span data-stu-id="a4d18-132">Sync based on my usage.</span></span>|




