---
title: tipo de enum emailSyncSchedule
description: Valores possíveis para a agenda de sincronização de email.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8285b9a34e208b86b7c53c38e6aa015fd8c37560
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425180"
---
# <a name="emailsyncschedule-enum-type"></a><span data-ttu-id="2d6cf-103">tipo de enum emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="2d6cf-103">emailSyncSchedule enum type</span></span>

> <span data-ttu-id="2d6cf-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2d6cf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2d6cf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2d6cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2d6cf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2d6cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d6cf-107">Valores possíveis para a agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="2d6cf-107">Possible values for email sync schedule.</span></span>

## <a name="members"></a><span data-ttu-id="2d6cf-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2d6cf-108">Members</span></span>
|<span data-ttu-id="2d6cf-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2d6cf-109">Member</span></span>|<span data-ttu-id="2d6cf-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2d6cf-110">Value</span></span>|<span data-ttu-id="2d6cf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d6cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d6cf-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="2d6cf-112">userDefined</span></span>|<span data-ttu-id="2d6cf-113">0</span><span class="sxs-lookup"><span data-stu-id="2d6cf-113">0</span></span>|<span data-ttu-id="2d6cf-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="2d6cf-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="2d6cf-115">asMessagesArrive</span><span class="sxs-lookup"><span data-stu-id="2d6cf-115">asMessagesArrive</span></span>|<span data-ttu-id="2d6cf-116">1</span><span class="sxs-lookup"><span data-stu-id="2d6cf-116">1</span></span>|<span data-ttu-id="2d6cf-117">Sincronizar à medida que chegam mensagens.</span><span class="sxs-lookup"><span data-stu-id="2d6cf-117">Sync as messages arrive.</span></span>|
|<span data-ttu-id="2d6cf-118">Manual</span><span class="sxs-lookup"><span data-stu-id="2d6cf-118">manual</span></span>|<span data-ttu-id="2d6cf-119">2</span><span class="sxs-lookup"><span data-stu-id="2d6cf-119">2</span></span>|<span data-ttu-id="2d6cf-120">Sincronize manualmente.</span><span class="sxs-lookup"><span data-stu-id="2d6cf-120">Sync manually.</span></span>|
|<span data-ttu-id="2d6cf-121">fifteenMinutes</span><span class="sxs-lookup"><span data-stu-id="2d6cf-121">fifteenMinutes</span></span>|<span data-ttu-id="2d6cf-122">3</span><span class="sxs-lookup"><span data-stu-id="2d6cf-122">3</span></span>|<span data-ttu-id="2d6cf-123">Sincronizar a cada 15 minutos.</span><span class="sxs-lookup"><span data-stu-id="2d6cf-123">Sync every fifteen minutes.</span></span>|
|<span data-ttu-id="2d6cf-124">thirtyMinutes</span><span class="sxs-lookup"><span data-stu-id="2d6cf-124">thirtyMinutes</span></span>|<span data-ttu-id="2d6cf-125">4</span><span class="sxs-lookup"><span data-stu-id="2d6cf-125">4</span></span>|<span data-ttu-id="2d6cf-126">Sincronizar a cada 30 minutos.</span><span class="sxs-lookup"><span data-stu-id="2d6cf-126">Sync every thirty minutes.</span></span>|
|<span data-ttu-id="2d6cf-127">sixtyMinutes</span><span class="sxs-lookup"><span data-stu-id="2d6cf-127">sixtyMinutes</span></span>|<span data-ttu-id="2d6cf-128">5</span><span class="sxs-lookup"><span data-stu-id="2d6cf-128">5</span></span>|<span data-ttu-id="2d6cf-129">Sincronizar a cada 60 minutos.</span><span class="sxs-lookup"><span data-stu-id="2d6cf-129">Sync every sixty minutes.</span></span>|
|<span data-ttu-id="2d6cf-130">basedOnMyUsage</span><span class="sxs-lookup"><span data-stu-id="2d6cf-130">basedOnMyUsage</span></span>|<span data-ttu-id="2d6cf-131">6</span><span class="sxs-lookup"><span data-stu-id="2d6cf-131">6</span></span>|<span data-ttu-id="2d6cf-132">Sincronizar com base no meu uso.</span><span class="sxs-lookup"><span data-stu-id="2d6cf-132">Sync based on my usage.</span></span>|




