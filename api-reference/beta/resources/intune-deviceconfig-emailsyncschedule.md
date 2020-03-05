---
title: tipo de enumeração emailSyncSchedule
description: Valores possíveis para agenda de sincronização de email.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c77a56b5dea371b4d91deb2258dad265b4d0433c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526462"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="08013-103">tipo de enumeração emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="08013-103">emailSyncSchedule enum type</span></span>

<span data-ttu-id="08013-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="08013-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08013-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="08013-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08013-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08013-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08013-107">Valores possíveis para agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="08013-107">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="08013-108">Membros</span><span class="sxs-lookup"><span data-stu-id="08013-108">Members</span></span>
|<span data-ttu-id="08013-109">Membro</span><span class="sxs-lookup"><span data-stu-id="08013-109">Member</span></span>|<span data-ttu-id="08013-110">Valor</span><span class="sxs-lookup"><span data-stu-id="08013-110">Value</span></span>|<span data-ttu-id="08013-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="08013-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08013-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="08013-112">userDefined</span></span>|<span data-ttu-id="08013-113">,0</span><span class="sxs-lookup"><span data-stu-id="08013-113">0</span></span>|<span data-ttu-id="08013-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="08013-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="08013-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="08013-115">asMessagesArrive</span></span>|<span data-ttu-id="08013-116">1 </span><span class="sxs-lookup"><span data-stu-id="08013-116">1</span></span>|<span data-ttu-id="08013-117">Sincronizar à medida que as mensagens chegam.</span><span class="sxs-lookup"><span data-stu-id="08013-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="08013-118">Manual</span><span class="sxs-lookup"><span data-stu-id="08013-118">manual</span></span>|<span data-ttu-id="08013-119">2 </span><span class="sxs-lookup"><span data-stu-id="08013-119">2</span></span>|<span data-ttu-id="08013-120">Sincronizar manualmente.</span><span class="sxs-lookup"><span data-stu-id="08013-120">Sync manually.</span></span>|
|<span data-ttu-id="08013-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="08013-121">fifteenMinutes</span></span>|<span data-ttu-id="08013-122">3 </span><span class="sxs-lookup"><span data-stu-id="08013-122">3</span></span>|<span data-ttu-id="08013-123">Sincronizar a cada quinze minutos.</span><span class="sxs-lookup"><span data-stu-id="08013-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="08013-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="08013-124">thirtyMinutes</span></span>|<span data-ttu-id="08013-125">4 </span><span class="sxs-lookup"><span data-stu-id="08013-125">4</span></span>|<span data-ttu-id="08013-126">Sincronizar a cada trinta minutos.</span><span class="sxs-lookup"><span data-stu-id="08013-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="08013-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="08013-127">sixtyMinutes</span></span>|<span data-ttu-id="08013-128">5 </span><span class="sxs-lookup"><span data-stu-id="08013-128">5</span></span>|<span data-ttu-id="08013-129">Sincronizar a cada 60 minutos.</span><span class="sxs-lookup"><span data-stu-id="08013-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="08013-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="08013-130">basedOnMyUsage</span></span>|<span data-ttu-id="08013-131">6 </span><span class="sxs-lookup"><span data-stu-id="08013-131">6</span></span>|<span data-ttu-id="08013-132">Sincronizar com base no meu uso.</span><span class="sxs-lookup"><span data-stu-id="08013-132">Sync based on my usage.</span></span>|



