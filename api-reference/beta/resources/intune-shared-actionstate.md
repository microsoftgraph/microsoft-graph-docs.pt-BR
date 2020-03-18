---
title: tipo de Enumeração ActionState
description: Estado da ação no dispositivo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 734fa5b7920c64ed2f649f78a2e81de068e3e0db
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772255"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="294b6-103">tipo de Enumeração ActionState</span><span class="sxs-lookup"><span data-stu-id="294b6-103">actionState enum type</span></span>

> <span data-ttu-id="294b6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="294b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="294b6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="294b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="294b6-106">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="294b6-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="294b6-107">Membros</span><span class="sxs-lookup"><span data-stu-id="294b6-107">Members</span></span>
|<span data-ttu-id="294b6-108">Membro</span><span class="sxs-lookup"><span data-stu-id="294b6-108">Member</span></span>|<span data-ttu-id="294b6-109">Valor</span><span class="sxs-lookup"><span data-stu-id="294b6-109">Value</span></span>|<span data-ttu-id="294b6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="294b6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="294b6-111">none</span><span class="sxs-lookup"><span data-stu-id="294b6-111">none</span></span>|<span data-ttu-id="294b6-112">,0</span><span class="sxs-lookup"><span data-stu-id="294b6-112">0</span></span>|<span data-ttu-id="294b6-113">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="294b6-113">Not a valid action state</span></span>|
|<span data-ttu-id="294b6-114">função</span><span class="sxs-lookup"><span data-stu-id="294b6-114">pending</span></span>|<span data-ttu-id="294b6-115">1</span><span class="sxs-lookup"><span data-stu-id="294b6-115">1</span></span>|<span data-ttu-id="294b6-116">Ação pendente</span><span class="sxs-lookup"><span data-stu-id="294b6-116">Action is pending</span></span>|
|<span data-ttu-id="294b6-117">foi</span><span class="sxs-lookup"><span data-stu-id="294b6-117">canceled</span></span>|<span data-ttu-id="294b6-118">duas</span><span class="sxs-lookup"><span data-stu-id="294b6-118">2</span></span>|<span data-ttu-id="294b6-119">A ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="294b6-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="294b6-120">active</span><span class="sxs-lookup"><span data-stu-id="294b6-120">active</span></span>|<span data-ttu-id="294b6-121">3D</span><span class="sxs-lookup"><span data-stu-id="294b6-121">3</span></span>|<span data-ttu-id="294b6-122">A ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="294b6-122">Action is active.</span></span>|
|<span data-ttu-id="294b6-123">done</span><span class="sxs-lookup"><span data-stu-id="294b6-123">done</span></span>|<span data-ttu-id="294b6-124">4 </span><span class="sxs-lookup"><span data-stu-id="294b6-124">4</span></span>|<span data-ttu-id="294b6-125">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="294b6-125">Action completed without errors.</span></span>|
|<span data-ttu-id="294b6-126">falhou</span><span class="sxs-lookup"><span data-stu-id="294b6-126">failed</span></span>|<span data-ttu-id="294b6-127">5 </span><span class="sxs-lookup"><span data-stu-id="294b6-127">5</span></span>|<span data-ttu-id="294b6-128">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="294b6-128">Action failed</span></span>|
|<span data-ttu-id="294b6-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="294b6-129">notSupported</span></span>|<span data-ttu-id="294b6-130">6 </span><span class="sxs-lookup"><span data-stu-id="294b6-130">6</span></span>|<span data-ttu-id="294b6-131">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="294b6-131">Action is not supported.</span></span>|



