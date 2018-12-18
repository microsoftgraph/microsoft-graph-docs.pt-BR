---
title: tipo de enum emailSyncSchedule
description: Valores possíveis para a agenda de sincronização de email.
author: tfitzmac
ms.openlocfilehash: f0e6673064f7e483756dfcfec8ce074e809dfcf4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308677"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="c5a37-103">tipo de enum emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="c5a37-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="c5a37-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c5a37-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5a37-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c5a37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5a37-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c5a37-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5a37-107">Valores possíveis para a agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="c5a37-107">Possible values for email sync schedule.</span></span>
## <a name="members"></a><span data-ttu-id="c5a37-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c5a37-108">Members</span></span>
|<span data-ttu-id="c5a37-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c5a37-109">Member</span></span>|<span data-ttu-id="c5a37-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c5a37-110">Value</span></span>|<span data-ttu-id="c5a37-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5a37-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5a37-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="c5a37-112">userDefined</span></span>|<span data-ttu-id="c5a37-113">0</span><span class="sxs-lookup"><span data-stu-id="c5a37-113">0</span></span>|<span data-ttu-id="c5a37-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="c5a37-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c5a37-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="c5a37-115">asMessagesArrive</span></span>|<span data-ttu-id="c5a37-116">1</span><span class="sxs-lookup"><span data-stu-id="c5a37-116">1</span></span>|<span data-ttu-id="c5a37-117">Sincronizar à medida que chegam mensagens.</span><span class="sxs-lookup"><span data-stu-id="c5a37-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="c5a37-118">Manual</span><span class="sxs-lookup"><span data-stu-id="c5a37-118">manual</span></span>|<span data-ttu-id="c5a37-119">2</span><span class="sxs-lookup"><span data-stu-id="c5a37-119">2</span></span>|<span data-ttu-id="c5a37-120">Sincronize manualmente.</span><span class="sxs-lookup"><span data-stu-id="c5a37-120">Sync manually.</span></span>|
|<span data-ttu-id="c5a37-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="c5a37-121">fifteenMinutes</span></span>|<span data-ttu-id="c5a37-122">3</span><span class="sxs-lookup"><span data-stu-id="c5a37-122">3</span></span>|<span data-ttu-id="c5a37-123">Sincronizar a cada 15 minutos.</span><span class="sxs-lookup"><span data-stu-id="c5a37-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="c5a37-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="c5a37-124">thirtyMinutes</span></span>|<span data-ttu-id="c5a37-125">4</span><span class="sxs-lookup"><span data-stu-id="c5a37-125">4</span></span>|<span data-ttu-id="c5a37-126">Sincronizar a cada 30 minutos.</span><span class="sxs-lookup"><span data-stu-id="c5a37-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="c5a37-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="c5a37-127">sixtyMinutes</span></span>|<span data-ttu-id="c5a37-128">5</span><span class="sxs-lookup"><span data-stu-id="c5a37-128">5</span></span>|<span data-ttu-id="c5a37-129">Sincronizar a cada 60 minutos.</span><span class="sxs-lookup"><span data-stu-id="c5a37-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="c5a37-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="c5a37-130">basedOnMyUsage</span></span>|<span data-ttu-id="c5a37-131">6</span><span class="sxs-lookup"><span data-stu-id="c5a37-131">6</span></span>|<span data-ttu-id="c5a37-132">Sincronizar com base no meu uso.</span><span class="sxs-lookup"><span data-stu-id="c5a37-132">Sync based on my usage.</span></span>|





