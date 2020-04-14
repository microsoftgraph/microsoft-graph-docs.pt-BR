---
title: tipo de enumeração emailSyncSchedule
description: Valores possíveis para agenda de sincronização de email.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 565cde82689fb8e208f0b7c6463e9a7b647a4d75
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460084"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="83f06-103">tipo de enumeração emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="83f06-103">emailSyncSchedule enum type</span></span>

<span data-ttu-id="83f06-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83f06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83f06-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83f06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83f06-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83f06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83f06-107">Valores possíveis para agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="83f06-107">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="83f06-108">Membros</span><span class="sxs-lookup"><span data-stu-id="83f06-108">Members</span></span>
|<span data-ttu-id="83f06-109">Membro</span><span class="sxs-lookup"><span data-stu-id="83f06-109">Member</span></span>|<span data-ttu-id="83f06-110">Valor</span><span class="sxs-lookup"><span data-stu-id="83f06-110">Value</span></span>|<span data-ttu-id="83f06-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="83f06-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83f06-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="83f06-112">userDefined</span></span>|<span data-ttu-id="83f06-113">,0</span><span class="sxs-lookup"><span data-stu-id="83f06-113">0</span></span>|<span data-ttu-id="83f06-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="83f06-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="83f06-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="83f06-115">asMessagesArrive</span></span>|<span data-ttu-id="83f06-116">1</span><span class="sxs-lookup"><span data-stu-id="83f06-116">1</span></span>|<span data-ttu-id="83f06-117">Sincronizar à medida que as mensagens chegam.</span><span class="sxs-lookup"><span data-stu-id="83f06-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="83f06-118">Manual</span><span class="sxs-lookup"><span data-stu-id="83f06-118">manual</span></span>|<span data-ttu-id="83f06-119">duas</span><span class="sxs-lookup"><span data-stu-id="83f06-119">2</span></span>|<span data-ttu-id="83f06-120">Sincronizar manualmente.</span><span class="sxs-lookup"><span data-stu-id="83f06-120">Sync manually.</span></span>|
|<span data-ttu-id="83f06-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="83f06-121">fifteenMinutes</span></span>|<span data-ttu-id="83f06-122">3D</span><span class="sxs-lookup"><span data-stu-id="83f06-122">3</span></span>|<span data-ttu-id="83f06-123">Sincronizar a cada quinze minutos.</span><span class="sxs-lookup"><span data-stu-id="83f06-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="83f06-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="83f06-124">thirtyMinutes</span></span>|<span data-ttu-id="83f06-125">4 </span><span class="sxs-lookup"><span data-stu-id="83f06-125">4</span></span>|<span data-ttu-id="83f06-126">Sincronizar a cada trinta minutos.</span><span class="sxs-lookup"><span data-stu-id="83f06-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="83f06-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="83f06-127">sixtyMinutes</span></span>|<span data-ttu-id="83f06-128">5 </span><span class="sxs-lookup"><span data-stu-id="83f06-128">5</span></span>|<span data-ttu-id="83f06-129">Sincronizar a cada 60 minutos.</span><span class="sxs-lookup"><span data-stu-id="83f06-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="83f06-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="83f06-130">basedOnMyUsage</span></span>|<span data-ttu-id="83f06-131">6 </span><span class="sxs-lookup"><span data-stu-id="83f06-131">6</span></span>|<span data-ttu-id="83f06-132">Sincronizar com base no meu uso.</span><span class="sxs-lookup"><span data-stu-id="83f06-132">Sync based on my usage.</span></span>|



