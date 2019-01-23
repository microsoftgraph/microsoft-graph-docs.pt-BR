---
title: tipo de enum emailSyncDuration
description: Valores possíveis para a duração de sincronização de email.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8bf62aea1904c0fd25867aef308ca5a269e3ea20
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399406"
---
# <a name="emailsyncduration-enum-type"></a><span data-ttu-id="b18f9-103">tipo de enum emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="b18f9-103">emailSyncDuration enum type</span></span>

> <span data-ttu-id="b18f9-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b18f9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b18f9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b18f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b18f9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b18f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b18f9-107">Valores possíveis para a duração de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="b18f9-107">Possible values for email sync duration.</span></span>

## <a name="members"></a><span data-ttu-id="b18f9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b18f9-108">Members</span></span>
|<span data-ttu-id="b18f9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b18f9-109">Member</span></span>|<span data-ttu-id="b18f9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b18f9-110">Value</span></span>|<span data-ttu-id="b18f9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b18f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b18f9-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="b18f9-112">userDefined</span></span>|<span data-ttu-id="b18f9-113">0</span><span class="sxs-lookup"><span data-stu-id="b18f9-113">0</span></span>|<span data-ttu-id="b18f9-114">Definido pelo usuário, valor padrão, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="b18f9-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b18f9-115">oneDay</span><span class="sxs-lookup"><span data-stu-id="b18f9-115">oneDay</span></span>|<span data-ttu-id="b18f9-116">1</span><span class="sxs-lookup"><span data-stu-id="b18f9-116">1</span></span>|<span data-ttu-id="b18f9-117">Sincronizar um dia de email.</span><span class="sxs-lookup"><span data-stu-id="b18f9-117">Sync one day of email.</span></span>|
|<span data-ttu-id="b18f9-118">threeDays</span><span class="sxs-lookup"><span data-stu-id="b18f9-118">threeDays</span></span>|<span data-ttu-id="b18f9-119">2</span><span class="sxs-lookup"><span data-stu-id="b18f9-119">2</span></span>|<span data-ttu-id="b18f9-120">Sincronizar três dias de email.</span><span class="sxs-lookup"><span data-stu-id="b18f9-120">Sync three days of email.</span></span>|
|<span data-ttu-id="b18f9-121">oneWeek</span><span class="sxs-lookup"><span data-stu-id="b18f9-121">oneWeek</span></span>|<span data-ttu-id="b18f9-122">3</span><span class="sxs-lookup"><span data-stu-id="b18f9-122">3</span></span>|<span data-ttu-id="b18f9-123">Sincronizar uma semana de email.</span><span class="sxs-lookup"><span data-stu-id="b18f9-123">Sync one week of email.</span></span>|
|<span data-ttu-id="b18f9-124">twoWeeks</span><span class="sxs-lookup"><span data-stu-id="b18f9-124">twoWeeks</span></span>|<span data-ttu-id="b18f9-125">4</span><span class="sxs-lookup"><span data-stu-id="b18f9-125">4</span></span>|<span data-ttu-id="b18f9-126">Sincronizar duas semanas de email.</span><span class="sxs-lookup"><span data-stu-id="b18f9-126">Sync two weeks of email.</span></span>|
|<span data-ttu-id="b18f9-127">oneMonth</span><span class="sxs-lookup"><span data-stu-id="b18f9-127">oneMonth</span></span>|<span data-ttu-id="b18f9-128">5</span><span class="sxs-lookup"><span data-stu-id="b18f9-128">5</span></span>|<span data-ttu-id="b18f9-129">Sincronizar um mês de email.</span><span class="sxs-lookup"><span data-stu-id="b18f9-129">Sync one month of email.</span></span>|
|<span data-ttu-id="b18f9-130">ilimitado</span><span class="sxs-lookup"><span data-stu-id="b18f9-130">unlimited</span></span>|<span data-ttu-id="b18f9-131">6</span><span class="sxs-lookup"><span data-stu-id="b18f9-131">6</span></span>|<span data-ttu-id="b18f9-132">Sincronize uma duração ilimitada de email.</span><span class="sxs-lookup"><span data-stu-id="b18f9-132">Sync an unlimited duration of email.</span></span>|




