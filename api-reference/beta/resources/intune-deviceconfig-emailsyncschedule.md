---
title: tipo de enumeração emailSyncSchedule
description: Valores possíveis para agenda de sincronização de email.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fa1dfa4455a39c9d7fffff1ee95a739632cd49cd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705922"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="8288b-103">tipo de enumeração emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="8288b-103">emailSyncSchedule enum type</span></span>

<span data-ttu-id="8288b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8288b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8288b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8288b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8288b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8288b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8288b-107">Valores possíveis para agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="8288b-107">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="8288b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="8288b-108">Members</span></span>
|<span data-ttu-id="8288b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="8288b-109">Member</span></span>|<span data-ttu-id="8288b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="8288b-110">Value</span></span>|<span data-ttu-id="8288b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8288b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8288b-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="8288b-112">userDefined</span></span>|<span data-ttu-id="8288b-113">,0</span><span class="sxs-lookup"><span data-stu-id="8288b-113">0</span></span>|<span data-ttu-id="8288b-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="8288b-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="8288b-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="8288b-115">asMessagesArrive</span></span>|<span data-ttu-id="8288b-116">1</span><span class="sxs-lookup"><span data-stu-id="8288b-116">1</span></span>|<span data-ttu-id="8288b-117">Sincronizar à medida que as mensagens chegam.</span><span class="sxs-lookup"><span data-stu-id="8288b-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="8288b-118">Manual</span><span class="sxs-lookup"><span data-stu-id="8288b-118">manual</span></span>|<span data-ttu-id="8288b-119">duas</span><span class="sxs-lookup"><span data-stu-id="8288b-119">2</span></span>|<span data-ttu-id="8288b-120">Sincronizar manualmente.</span><span class="sxs-lookup"><span data-stu-id="8288b-120">Sync manually.</span></span>|
|<span data-ttu-id="8288b-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="8288b-121">fifteenMinutes</span></span>|<span data-ttu-id="8288b-122">3D</span><span class="sxs-lookup"><span data-stu-id="8288b-122">3</span></span>|<span data-ttu-id="8288b-123">Sincronizar a cada quinze minutos.</span><span class="sxs-lookup"><span data-stu-id="8288b-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="8288b-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="8288b-124">thirtyMinutes</span></span>|<span data-ttu-id="8288b-125">4 </span><span class="sxs-lookup"><span data-stu-id="8288b-125">4</span></span>|<span data-ttu-id="8288b-126">Sincronizar a cada trinta minutos.</span><span class="sxs-lookup"><span data-stu-id="8288b-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="8288b-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="8288b-127">sixtyMinutes</span></span>|<span data-ttu-id="8288b-128">5 </span><span class="sxs-lookup"><span data-stu-id="8288b-128">5</span></span>|<span data-ttu-id="8288b-129">Sincronizar a cada 60 minutos.</span><span class="sxs-lookup"><span data-stu-id="8288b-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="8288b-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="8288b-130">basedOnMyUsage</span></span>|<span data-ttu-id="8288b-131">6 </span><span class="sxs-lookup"><span data-stu-id="8288b-131">6</span></span>|<span data-ttu-id="8288b-132">Sincronizar com base no meu uso.</span><span class="sxs-lookup"><span data-stu-id="8288b-132">Sync based on my usage.</span></span>|





