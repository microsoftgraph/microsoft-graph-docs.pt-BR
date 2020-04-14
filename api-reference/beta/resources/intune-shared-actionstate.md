---
title: tipo de Enumeração ActionState
description: Estado da ação no dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c213567b46c7aea2f91deae8bc8a27d4b0382c7d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453177"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="b0173-103">tipo de Enumeração ActionState</span><span class="sxs-lookup"><span data-stu-id="b0173-103">actionState enum type</span></span>

<span data-ttu-id="b0173-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0173-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0173-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0173-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0173-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0173-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0173-107">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="b0173-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="b0173-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b0173-108">Members</span></span>
|<span data-ttu-id="b0173-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b0173-109">Member</span></span>|<span data-ttu-id="b0173-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b0173-110">Value</span></span>|<span data-ttu-id="b0173-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0173-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0173-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="b0173-112">none</span></span>|<span data-ttu-id="b0173-113">,0</span><span class="sxs-lookup"><span data-stu-id="b0173-113">0</span></span>|<span data-ttu-id="b0173-114">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="b0173-114">Not a valid action state</span></span>|
|<span data-ttu-id="b0173-115">função</span><span class="sxs-lookup"><span data-stu-id="b0173-115">pending</span></span>|<span data-ttu-id="b0173-116">1</span><span class="sxs-lookup"><span data-stu-id="b0173-116">1</span></span>|<span data-ttu-id="b0173-117">Ação pendente</span><span class="sxs-lookup"><span data-stu-id="b0173-117">Action is pending</span></span>|
|<span data-ttu-id="b0173-118">foi</span><span class="sxs-lookup"><span data-stu-id="b0173-118">canceled</span></span>|<span data-ttu-id="b0173-119">duas</span><span class="sxs-lookup"><span data-stu-id="b0173-119">2</span></span>|<span data-ttu-id="b0173-120">A ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="b0173-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="b0173-121">active</span><span class="sxs-lookup"><span data-stu-id="b0173-121">active</span></span>|<span data-ttu-id="b0173-122">3D</span><span class="sxs-lookup"><span data-stu-id="b0173-122">3</span></span>|<span data-ttu-id="b0173-123">A ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="b0173-123">Action is active.</span></span>|
|<span data-ttu-id="b0173-124">done</span><span class="sxs-lookup"><span data-stu-id="b0173-124">done</span></span>|<span data-ttu-id="b0173-125">4 </span><span class="sxs-lookup"><span data-stu-id="b0173-125">4</span></span>|<span data-ttu-id="b0173-126">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="b0173-126">Action completed without errors.</span></span>|
|<span data-ttu-id="b0173-127">falhou</span><span class="sxs-lookup"><span data-stu-id="b0173-127">failed</span></span>|<span data-ttu-id="b0173-128">5 </span><span class="sxs-lookup"><span data-stu-id="b0173-128">5</span></span>|<span data-ttu-id="b0173-129">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="b0173-129">Action failed</span></span>|
|<span data-ttu-id="b0173-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="b0173-130">notSupported</span></span>|<span data-ttu-id="b0173-131">6 </span><span class="sxs-lookup"><span data-stu-id="b0173-131">6</span></span>|<span data-ttu-id="b0173-132">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="b0173-132">Action is not supported.</span></span>|



