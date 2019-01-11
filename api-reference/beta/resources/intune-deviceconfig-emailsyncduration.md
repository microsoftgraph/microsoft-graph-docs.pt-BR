---
title: tipo de enum emailSyncDuration
description: Valores possíveis para a duração de sincronização de email.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d83a1ceb82820ddc44d8753e8ed05e00de09e36e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819378"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="7e11d-103">tipo de enum emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="7e11d-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="7e11d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7e11d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e11d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7e11d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e11d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7e11d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e11d-107">Valores possíveis para a duração de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="7e11d-107">Possible values for email sync duration.</span></span>
## <a name="members"></a><span data-ttu-id="7e11d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="7e11d-108">Members</span></span>
|<span data-ttu-id="7e11d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="7e11d-109">Member</span></span>|<span data-ttu-id="7e11d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="7e11d-110">Value</span></span>|<span data-ttu-id="7e11d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e11d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e11d-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="7e11d-112">userDefined</span></span>|<span data-ttu-id="7e11d-113">0</span><span class="sxs-lookup"><span data-stu-id="7e11d-113">0</span></span>|<span data-ttu-id="7e11d-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="7e11d-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="7e11d-115">oneDay</span><span class="sxs-lookup"><span data-stu-id="7e11d-115">oneDay</span></span>|<span data-ttu-id="7e11d-116">1</span><span class="sxs-lookup"><span data-stu-id="7e11d-116">1</span></span>|<span data-ttu-id="7e11d-117">Sincronizar um dia de email.</span><span class="sxs-lookup"><span data-stu-id="7e11d-117">Sync one day of email.</span></span>|
|<span data-ttu-id="7e11d-118">threeDays</span><span class="sxs-lookup"><span data-stu-id="7e11d-118">threeDays</span></span>|<span data-ttu-id="7e11d-119">2</span><span class="sxs-lookup"><span data-stu-id="7e11d-119">2</span></span>|<span data-ttu-id="7e11d-120">Sincronizar três dias de email.</span><span class="sxs-lookup"><span data-stu-id="7e11d-120">Sync three days of email.</span></span>|
|<span data-ttu-id="7e11d-121">oneWeek</span><span class="sxs-lookup"><span data-stu-id="7e11d-121">oneWeek</span></span>|<span data-ttu-id="7e11d-122">3</span><span class="sxs-lookup"><span data-stu-id="7e11d-122">3</span></span>|<span data-ttu-id="7e11d-123">Sincronizar uma semana de email.</span><span class="sxs-lookup"><span data-stu-id="7e11d-123">Sync one week of email.</span></span>|
|<span data-ttu-id="7e11d-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="7e11d-124">twoWeeks</span></span>|<span data-ttu-id="7e11d-125">4</span><span class="sxs-lookup"><span data-stu-id="7e11d-125">4</span></span>|<span data-ttu-id="7e11d-126">Sincronizar duas semanas de email.</span><span class="sxs-lookup"><span data-stu-id="7e11d-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="7e11d-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="7e11d-127">oneMonth</span></span>|<span data-ttu-id="7e11d-128">5</span><span class="sxs-lookup"><span data-stu-id="7e11d-128">5</span></span>|<span data-ttu-id="7e11d-129">Sincronizar um mês de email.</span><span class="sxs-lookup"><span data-stu-id="7e11d-129">Sync one month of email.</span></span>|
|<span data-ttu-id="7e11d-130">ilimitado</span><span class="sxs-lookup"><span data-stu-id="7e11d-130">unlimited</span></span>|<span data-ttu-id="7e11d-131">6</span><span class="sxs-lookup"><span data-stu-id="7e11d-131">6</span></span>|<span data-ttu-id="7e11d-132">Sincronize uma duração ilimitada de email.</span><span class="sxs-lookup"><span data-stu-id="7e11d-132">Sync an unlimited duration of email.</span></span>|





