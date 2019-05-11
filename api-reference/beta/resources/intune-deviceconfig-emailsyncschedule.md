---
title: tipo de enumeração emailSyncSchedule
description: Valores possíveis para agenda de sincronização de email.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3801fa0a49d2121b31d91f1f4cc5a03af7fb0571
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946613"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="51304-103">tipo de enumeração emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="51304-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="51304-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="51304-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51304-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51304-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51304-106">Valores possíveis para agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="51304-106">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="51304-107">Membros</span><span class="sxs-lookup"><span data-stu-id="51304-107">Members</span></span>
|<span data-ttu-id="51304-108">Membro</span><span class="sxs-lookup"><span data-stu-id="51304-108">Member</span></span>|<span data-ttu-id="51304-109">Valor</span><span class="sxs-lookup"><span data-stu-id="51304-109">Value</span></span>|<span data-ttu-id="51304-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="51304-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51304-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="51304-111">userDefined</span></span>|<span data-ttu-id="51304-112">,0</span><span class="sxs-lookup"><span data-stu-id="51304-112">0</span></span>|<span data-ttu-id="51304-113">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="51304-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="51304-114">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="51304-114">asMessagesArrive</span></span>|<span data-ttu-id="51304-115">1</span><span class="sxs-lookup"><span data-stu-id="51304-115">1</span></span>|<span data-ttu-id="51304-116">Sincronizar à medida que as mensagens chegam.</span><span class="sxs-lookup"><span data-stu-id="51304-116">Sync as messages arrive.</span></span>|
|<span data-ttu-id="51304-117">Manual</span><span class="sxs-lookup"><span data-stu-id="51304-117">manual</span></span>|<span data-ttu-id="51304-118">duas</span><span class="sxs-lookup"><span data-stu-id="51304-118">2</span></span>|<span data-ttu-id="51304-119">Sincronizar manualmente.</span><span class="sxs-lookup"><span data-stu-id="51304-119">Sync manually.</span></span>|
|<span data-ttu-id="51304-120">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="51304-120">fifteenMinutes</span></span>|<span data-ttu-id="51304-121">3D</span><span class="sxs-lookup"><span data-stu-id="51304-121">3</span></span>|<span data-ttu-id="51304-122">Sincronizar a cada quinze minutos.</span><span class="sxs-lookup"><span data-stu-id="51304-122">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="51304-123">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="51304-123">thirtyMinutes</span></span>|<span data-ttu-id="51304-124">quatro</span><span class="sxs-lookup"><span data-stu-id="51304-124">4</span></span>|<span data-ttu-id="51304-125">Sincronizar a cada trinta minutos.</span><span class="sxs-lookup"><span data-stu-id="51304-125">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="51304-126">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="51304-126">sixtyMinutes</span></span>|<span data-ttu-id="51304-127">0,5</span><span class="sxs-lookup"><span data-stu-id="51304-127">5</span></span>|<span data-ttu-id="51304-128">Sincronizar a cada 60 minutos.</span><span class="sxs-lookup"><span data-stu-id="51304-128">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="51304-129">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="51304-129">basedOnMyUsage</span></span>|<span data-ttu-id="51304-130">6</span><span class="sxs-lookup"><span data-stu-id="51304-130">6</span></span>|<span data-ttu-id="51304-131">Sincronizar com base no meu uso.</span><span class="sxs-lookup"><span data-stu-id="51304-131">Sync based on my usage.</span></span>|




