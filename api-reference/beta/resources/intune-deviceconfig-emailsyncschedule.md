---
title: tipo de enum emailSyncSchedule
description: Valores possíveis para a agenda de sincronização de email.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9dc93bce19262d0b1aad1d1cc8f28ea4db56ce9f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924038"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="2742f-103">tipo de enum emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="2742f-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="2742f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2742f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2742f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2742f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2742f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2742f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2742f-107">Valores possíveis para a agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="2742f-107">Possible values for email sync schedule.</span></span>
## <a name="members"></a><span data-ttu-id="2742f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2742f-108">Members</span></span>
|<span data-ttu-id="2742f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2742f-109">Member</span></span>|<span data-ttu-id="2742f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2742f-110">Value</span></span>|<span data-ttu-id="2742f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2742f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2742f-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="2742f-112">userDefined</span></span>|<span data-ttu-id="2742f-113">0</span><span class="sxs-lookup"><span data-stu-id="2742f-113">0</span></span>|<span data-ttu-id="2742f-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="2742f-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="2742f-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="2742f-115">asMessagesArrive</span></span>|<span data-ttu-id="2742f-116">1</span><span class="sxs-lookup"><span data-stu-id="2742f-116">1</span></span>|<span data-ttu-id="2742f-117">Sincronizar à medida que chegam mensagens.</span><span class="sxs-lookup"><span data-stu-id="2742f-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="2742f-118">Manual</span><span class="sxs-lookup"><span data-stu-id="2742f-118">manual</span></span>|<span data-ttu-id="2742f-119">2</span><span class="sxs-lookup"><span data-stu-id="2742f-119">2</span></span>|<span data-ttu-id="2742f-120">Sincronize manualmente.</span><span class="sxs-lookup"><span data-stu-id="2742f-120">Sync manually.</span></span>|
|<span data-ttu-id="2742f-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="2742f-121">fifteenMinutes</span></span>|<span data-ttu-id="2742f-122">3</span><span class="sxs-lookup"><span data-stu-id="2742f-122">3</span></span>|<span data-ttu-id="2742f-123">Sincronizar a cada 15 minutos.</span><span class="sxs-lookup"><span data-stu-id="2742f-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="2742f-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="2742f-124">thirtyMinutes</span></span>|<span data-ttu-id="2742f-125">4</span><span class="sxs-lookup"><span data-stu-id="2742f-125">4</span></span>|<span data-ttu-id="2742f-126">Sincronizar a cada 30 minutos.</span><span class="sxs-lookup"><span data-stu-id="2742f-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="2742f-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="2742f-127">sixtyMinutes</span></span>|<span data-ttu-id="2742f-128">5</span><span class="sxs-lookup"><span data-stu-id="2742f-128">5</span></span>|<span data-ttu-id="2742f-129">Sincronizar a cada 60 minutos.</span><span class="sxs-lookup"><span data-stu-id="2742f-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="2742f-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="2742f-130">basedOnMyUsage</span></span>|<span data-ttu-id="2742f-131">6</span><span class="sxs-lookup"><span data-stu-id="2742f-131">6</span></span>|<span data-ttu-id="2742f-132">Sincronizar com base no meu uso.</span><span class="sxs-lookup"><span data-stu-id="2742f-132">Sync based on my usage.</span></span>|





