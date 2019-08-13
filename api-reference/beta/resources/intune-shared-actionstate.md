---
title: tipo de Enumeração ActionState
description: Estado da ação no dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d78f74294ae6ed486681e4378665589722dd1aa5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308174"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="67fd4-103">tipo de Enumeração ActionState</span><span class="sxs-lookup"><span data-stu-id="67fd4-103">actionState enum type</span></span>

> <span data-ttu-id="67fd4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67fd4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67fd4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67fd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67fd4-106">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="67fd4-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="67fd4-107">Membros</span><span class="sxs-lookup"><span data-stu-id="67fd4-107">Members</span></span>
|<span data-ttu-id="67fd4-108">Membro</span><span class="sxs-lookup"><span data-stu-id="67fd4-108">Member</span></span>|<span data-ttu-id="67fd4-109">Valor</span><span class="sxs-lookup"><span data-stu-id="67fd4-109">Value</span></span>|<span data-ttu-id="67fd4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="67fd4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67fd4-111">none</span><span class="sxs-lookup"><span data-stu-id="67fd4-111">none</span></span>|<span data-ttu-id="67fd4-112">,0</span><span class="sxs-lookup"><span data-stu-id="67fd4-112">0</span></span>|<span data-ttu-id="67fd4-113">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="67fd4-113">Not a valid action state</span></span>|
|<span data-ttu-id="67fd4-114">função</span><span class="sxs-lookup"><span data-stu-id="67fd4-114">pending</span></span>|<span data-ttu-id="67fd4-115">1</span><span class="sxs-lookup"><span data-stu-id="67fd4-115">1</span></span>|<span data-ttu-id="67fd4-116">Ação pendente</span><span class="sxs-lookup"><span data-stu-id="67fd4-116">Action is pending</span></span>|
|<span data-ttu-id="67fd4-117">foi</span><span class="sxs-lookup"><span data-stu-id="67fd4-117">canceled</span></span>|<span data-ttu-id="67fd4-118">duas</span><span class="sxs-lookup"><span data-stu-id="67fd4-118">2</span></span>|<span data-ttu-id="67fd4-119">A ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="67fd4-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="67fd4-120">active</span><span class="sxs-lookup"><span data-stu-id="67fd4-120">active</span></span>|<span data-ttu-id="67fd4-121">3D</span><span class="sxs-lookup"><span data-stu-id="67fd4-121">3</span></span>|<span data-ttu-id="67fd4-122">A ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="67fd4-122">Action is active.</span></span>|
|<span data-ttu-id="67fd4-123">done</span><span class="sxs-lookup"><span data-stu-id="67fd4-123">done</span></span>|<span data-ttu-id="67fd4-124">quatro</span><span class="sxs-lookup"><span data-stu-id="67fd4-124">4</span></span>|<span data-ttu-id="67fd4-125">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="67fd4-125">Action completed without errors.</span></span>|
|<span data-ttu-id="67fd4-126">falhou</span><span class="sxs-lookup"><span data-stu-id="67fd4-126">failed</span></span>|<span data-ttu-id="67fd4-127">0,5</span><span class="sxs-lookup"><span data-stu-id="67fd4-127">5</span></span>|<span data-ttu-id="67fd4-128">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="67fd4-128">Action failed</span></span>|
|<span data-ttu-id="67fd4-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="67fd4-129">notSupported</span></span>|<span data-ttu-id="67fd4-130">6</span><span class="sxs-lookup"><span data-stu-id="67fd4-130">6</span></span>|<span data-ttu-id="67fd4-131">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="67fd4-131">Action is not supported.</span></span>|



