---
title: tipo de enum emailSyncSchedule
description: Valores possíveis para a agenda de sincronização de email.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 178cba9e226b7f20e3fd917145e7bbd06f6c3a1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838392"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="4ebc3-103">tipo de enum emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="4ebc3-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="4ebc3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4ebc3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ebc3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4ebc3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ebc3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4ebc3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ebc3-107">Valores possíveis para a agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="4ebc3-107">Possible values for email sync schedule.</span></span>
## <a name="members"></a><span data-ttu-id="4ebc3-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4ebc3-108">Members</span></span>
|<span data-ttu-id="4ebc3-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4ebc3-109">Member</span></span>|<span data-ttu-id="4ebc3-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4ebc3-110">Value</span></span>|<span data-ttu-id="4ebc3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ebc3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ebc3-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="4ebc3-112">userDefined</span></span>|<span data-ttu-id="4ebc3-113">0</span><span class="sxs-lookup"><span data-stu-id="4ebc3-113">0</span></span>|<span data-ttu-id="4ebc3-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="4ebc3-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="4ebc3-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="4ebc3-115">asMessagesArrive</span></span>|<span data-ttu-id="4ebc3-116">1</span><span class="sxs-lookup"><span data-stu-id="4ebc3-116">1</span></span>|<span data-ttu-id="4ebc3-117">Sincronizar à medida que chegam mensagens.</span><span class="sxs-lookup"><span data-stu-id="4ebc3-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="4ebc3-118">Manual</span><span class="sxs-lookup"><span data-stu-id="4ebc3-118">manual</span></span>|<span data-ttu-id="4ebc3-119">2</span><span class="sxs-lookup"><span data-stu-id="4ebc3-119">2</span></span>|<span data-ttu-id="4ebc3-120">Sincronize manualmente.</span><span class="sxs-lookup"><span data-stu-id="4ebc3-120">Sync manually.</span></span>|
|<span data-ttu-id="4ebc3-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="4ebc3-121">fifteenMinutes</span></span>|<span data-ttu-id="4ebc3-122">3</span><span class="sxs-lookup"><span data-stu-id="4ebc3-122">3</span></span>|<span data-ttu-id="4ebc3-123">Sincronizar a cada 15 minutos.</span><span class="sxs-lookup"><span data-stu-id="4ebc3-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="4ebc3-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="4ebc3-124">thirtyMinutes</span></span>|<span data-ttu-id="4ebc3-125">4</span><span class="sxs-lookup"><span data-stu-id="4ebc3-125">4</span></span>|<span data-ttu-id="4ebc3-126">Sincronizar a cada 30 minutos.</span><span class="sxs-lookup"><span data-stu-id="4ebc3-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="4ebc3-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="4ebc3-127">sixtyMinutes</span></span>|<span data-ttu-id="4ebc3-128">5</span><span class="sxs-lookup"><span data-stu-id="4ebc3-128">5</span></span>|<span data-ttu-id="4ebc3-129">Sincronizar a cada 60 minutos.</span><span class="sxs-lookup"><span data-stu-id="4ebc3-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="4ebc3-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="4ebc3-130">basedOnMyUsage</span></span>|<span data-ttu-id="4ebc3-131">6</span><span class="sxs-lookup"><span data-stu-id="4ebc3-131">6</span></span>|<span data-ttu-id="4ebc3-132">Sincronizar com base no meu uso.</span><span class="sxs-lookup"><span data-stu-id="4ebc3-132">Sync based on my usage.</span></span>|





