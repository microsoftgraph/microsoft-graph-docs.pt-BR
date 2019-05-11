---
title: tipo de enumeração emailSyncDuration
description: Valores possíveis para duração da sincronização de email.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c6296178a8cd9bb987965944ba02c96aa44a534
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946771"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="b1b8f-103">tipo de enumeração emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="b1b8f-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="b1b8f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1b8f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1b8f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1b8f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1b8f-106">Valores possíveis para duração da sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="b1b8f-106">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="b1b8f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b1b8f-107">Members</span></span>
|<span data-ttu-id="b1b8f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b1b8f-108">Member</span></span>|<span data-ttu-id="b1b8f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b1b8f-109">Value</span></span>|<span data-ttu-id="b1b8f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1b8f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1b8f-111">UserDefined</span><span class="sxs-lookup"><span data-stu-id="b1b8f-111">userDefined</span></span>|<span data-ttu-id="b1b8f-112">,0</span><span class="sxs-lookup"><span data-stu-id="b1b8f-112">0</span></span>|<span data-ttu-id="b1b8f-113">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="b1b8f-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b1b8f-114">oneDay</span><span class="sxs-lookup"><span data-stu-id="b1b8f-114">oneDay</span></span>|<span data-ttu-id="b1b8f-115">1</span><span class="sxs-lookup"><span data-stu-id="b1b8f-115">1</span></span>|<span data-ttu-id="b1b8f-116">Sincronizar um dia de email.</span><span class="sxs-lookup"><span data-stu-id="b1b8f-116">Sync one day of email.</span></span>|
|<span data-ttu-id="b1b8f-117">threeDays</span><span class="sxs-lookup"><span data-stu-id="b1b8f-117">threeDays</span></span>|<span data-ttu-id="b1b8f-118">duas</span><span class="sxs-lookup"><span data-stu-id="b1b8f-118">2</span></span>|<span data-ttu-id="b1b8f-119">Sincronizar três dias de email.</span><span class="sxs-lookup"><span data-stu-id="b1b8f-119">Sync three days of email.</span></span>|
|<span data-ttu-id="b1b8f-120">oneWeek</span><span class="sxs-lookup"><span data-stu-id="b1b8f-120">oneWeek</span></span>|<span data-ttu-id="b1b8f-121">3D</span><span class="sxs-lookup"><span data-stu-id="b1b8f-121">3</span></span>|<span data-ttu-id="b1b8f-122">Sincronizar uma semana de email.</span><span class="sxs-lookup"><span data-stu-id="b1b8f-122">Sync one week of email.</span></span>|
|<span data-ttu-id="b1b8f-123">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="b1b8f-123">twoWeeks</span></span>|<span data-ttu-id="b1b8f-124">quatro</span><span class="sxs-lookup"><span data-stu-id="b1b8f-124">4</span></span>|<span data-ttu-id="b1b8f-125">Sincronize duas semanas de email.</span><span class="sxs-lookup"><span data-stu-id="b1b8f-125">Sync two weeks of email.</span></span>|
|<span data-ttu-id="b1b8f-126">oneMonth</span><span class="sxs-lookup"><span data-stu-id="b1b8f-126">oneMonth</span></span>|<span data-ttu-id="b1b8f-127">0,5</span><span class="sxs-lookup"><span data-stu-id="b1b8f-127">5</span></span>|<span data-ttu-id="b1b8f-128">Sincronizar um mês de email.</span><span class="sxs-lookup"><span data-stu-id="b1b8f-128">Sync one month of email.</span></span>|
|<span data-ttu-id="b1b8f-129">ilimitado</span><span class="sxs-lookup"><span data-stu-id="b1b8f-129">unlimited</span></span>|<span data-ttu-id="b1b8f-130">6</span><span class="sxs-lookup"><span data-stu-id="b1b8f-130">6</span></span>|<span data-ttu-id="b1b8f-131">Sincronizar uma duração ilimitada de email.</span><span class="sxs-lookup"><span data-stu-id="b1b8f-131">Sync an unlimited duration of email.</span></span>|




