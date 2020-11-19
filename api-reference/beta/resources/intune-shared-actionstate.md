---
title: tipo de Enumeração ActionState
description: Estado da ação no dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 99b7b189ed0e3f8a66eeaa4c099421b3b13e0989
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271972"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="3bd3a-103">tipo de Enumeração ActionState</span><span class="sxs-lookup"><span data-stu-id="3bd3a-103">actionState enum type</span></span>

<span data-ttu-id="3bd3a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bd3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3bd3a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3bd3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bd3a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3bd3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bd3a-107">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="3bd3a-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="3bd3a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="3bd3a-108">Members</span></span>
|<span data-ttu-id="3bd3a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="3bd3a-109">Member</span></span>|<span data-ttu-id="3bd3a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="3bd3a-110">Value</span></span>|<span data-ttu-id="3bd3a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bd3a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bd3a-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="3bd3a-112">none</span></span>|<span data-ttu-id="3bd3a-113">,0</span><span class="sxs-lookup"><span data-stu-id="3bd3a-113">0</span></span>|<span data-ttu-id="3bd3a-114">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="3bd3a-114">Not a valid action state</span></span>|
|<span data-ttu-id="3bd3a-115">função</span><span class="sxs-lookup"><span data-stu-id="3bd3a-115">pending</span></span>|<span data-ttu-id="3bd3a-116">1</span><span class="sxs-lookup"><span data-stu-id="3bd3a-116">1</span></span>|<span data-ttu-id="3bd3a-117">Ação pendente</span><span class="sxs-lookup"><span data-stu-id="3bd3a-117">Action is pending</span></span>|
|<span data-ttu-id="3bd3a-118">foi</span><span class="sxs-lookup"><span data-stu-id="3bd3a-118">canceled</span></span>|<span data-ttu-id="3bd3a-119">duas</span><span class="sxs-lookup"><span data-stu-id="3bd3a-119">2</span></span>|<span data-ttu-id="3bd3a-120">A ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="3bd3a-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="3bd3a-121">active</span><span class="sxs-lookup"><span data-stu-id="3bd3a-121">active</span></span>|<span data-ttu-id="3bd3a-122">3D</span><span class="sxs-lookup"><span data-stu-id="3bd3a-122">3</span></span>|<span data-ttu-id="3bd3a-123">A ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="3bd3a-123">Action is active.</span></span>|
|<span data-ttu-id="3bd3a-124">done</span><span class="sxs-lookup"><span data-stu-id="3bd3a-124">done</span></span>|<span data-ttu-id="3bd3a-125">4 </span><span class="sxs-lookup"><span data-stu-id="3bd3a-125">4</span></span>|<span data-ttu-id="3bd3a-126">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="3bd3a-126">Action completed without errors.</span></span>|
|<span data-ttu-id="3bd3a-127">falhou</span><span class="sxs-lookup"><span data-stu-id="3bd3a-127">failed</span></span>|<span data-ttu-id="3bd3a-128">5 </span><span class="sxs-lookup"><span data-stu-id="3bd3a-128">5</span></span>|<span data-ttu-id="3bd3a-129">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="3bd3a-129">Action failed</span></span>|
|<span data-ttu-id="3bd3a-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="3bd3a-130">notSupported</span></span>|<span data-ttu-id="3bd3a-131">6 </span><span class="sxs-lookup"><span data-stu-id="3bd3a-131">6</span></span>|<span data-ttu-id="3bd3a-132">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="3bd3a-132">Action is not supported.</span></span>|




