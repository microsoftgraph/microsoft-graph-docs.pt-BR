---
title: tipo de Enumeração ActionState
description: Estado da ação no dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f75622021616ac0d65dd305c75d73af738f3446c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733165"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="0f320-103">tipo de Enumeração ActionState</span><span class="sxs-lookup"><span data-stu-id="0f320-103">actionState enum type</span></span>

<span data-ttu-id="0f320-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f320-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f320-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f320-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f320-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f320-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f320-107">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="0f320-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="0f320-108">Membros</span><span class="sxs-lookup"><span data-stu-id="0f320-108">Members</span></span>
|<span data-ttu-id="0f320-109">Membro</span><span class="sxs-lookup"><span data-stu-id="0f320-109">Member</span></span>|<span data-ttu-id="0f320-110">Valor</span><span class="sxs-lookup"><span data-stu-id="0f320-110">Value</span></span>|<span data-ttu-id="0f320-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f320-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f320-112">none</span><span class="sxs-lookup"><span data-stu-id="0f320-112">none</span></span>|<span data-ttu-id="0f320-113">,0</span><span class="sxs-lookup"><span data-stu-id="0f320-113">0</span></span>|<span data-ttu-id="0f320-114">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="0f320-114">Not a valid action state</span></span>|
|<span data-ttu-id="0f320-115">função</span><span class="sxs-lookup"><span data-stu-id="0f320-115">pending</span></span>|<span data-ttu-id="0f320-116">1</span><span class="sxs-lookup"><span data-stu-id="0f320-116">1</span></span>|<span data-ttu-id="0f320-117">Ação pendente</span><span class="sxs-lookup"><span data-stu-id="0f320-117">Action is pending</span></span>|
|<span data-ttu-id="0f320-118">foi</span><span class="sxs-lookup"><span data-stu-id="0f320-118">canceled</span></span>|<span data-ttu-id="0f320-119">duas</span><span class="sxs-lookup"><span data-stu-id="0f320-119">2</span></span>|<span data-ttu-id="0f320-120">A ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="0f320-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="0f320-121">active</span><span class="sxs-lookup"><span data-stu-id="0f320-121">active</span></span>|<span data-ttu-id="0f320-122">3D</span><span class="sxs-lookup"><span data-stu-id="0f320-122">3</span></span>|<span data-ttu-id="0f320-123">A ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="0f320-123">Action is active.</span></span>|
|<span data-ttu-id="0f320-124">done</span><span class="sxs-lookup"><span data-stu-id="0f320-124">done</span></span>|<span data-ttu-id="0f320-125">4 </span><span class="sxs-lookup"><span data-stu-id="0f320-125">4</span></span>|<span data-ttu-id="0f320-126">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="0f320-126">Action completed without errors.</span></span>|
|<span data-ttu-id="0f320-127">falhou</span><span class="sxs-lookup"><span data-stu-id="0f320-127">failed</span></span>|<span data-ttu-id="0f320-128">5 </span><span class="sxs-lookup"><span data-stu-id="0f320-128">5</span></span>|<span data-ttu-id="0f320-129">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="0f320-129">Action failed</span></span>|
|<span data-ttu-id="0f320-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="0f320-130">notSupported</span></span>|<span data-ttu-id="0f320-131">6 </span><span class="sxs-lookup"><span data-stu-id="0f320-131">6</span></span>|<span data-ttu-id="0f320-132">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="0f320-132">Action is not supported.</span></span>|





