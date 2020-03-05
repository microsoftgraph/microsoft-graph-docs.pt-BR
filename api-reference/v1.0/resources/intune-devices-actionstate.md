---
title: tipo de Enumeração ActionState
description: Estado da ação no dispositivo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e11fc186dcfe16005e3ceaab5c6306f5893a8598
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418164"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="fc9e9-103">tipo de Enumeração ActionState</span><span class="sxs-lookup"><span data-stu-id="fc9e9-103">actionState enum type</span></span>

<span data-ttu-id="fc9e9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fc9e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc9e9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc9e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc9e9-106">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="fc9e9-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="fc9e9-107">Membros</span><span class="sxs-lookup"><span data-stu-id="fc9e9-107">Members</span></span>
|<span data-ttu-id="fc9e9-108">Membro</span><span class="sxs-lookup"><span data-stu-id="fc9e9-108">Member</span></span>|<span data-ttu-id="fc9e9-109">Valor</span><span class="sxs-lookup"><span data-stu-id="fc9e9-109">Value</span></span>|<span data-ttu-id="fc9e9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc9e9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc9e9-111">nenhuma</span><span class="sxs-lookup"><span data-stu-id="fc9e9-111">none</span></span>|<span data-ttu-id="fc9e9-112">,0</span><span class="sxs-lookup"><span data-stu-id="fc9e9-112">0</span></span>|<span data-ttu-id="fc9e9-113">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="fc9e9-113">Not a valid action state</span></span>|
|<span data-ttu-id="fc9e9-114">função</span><span class="sxs-lookup"><span data-stu-id="fc9e9-114">pending</span></span>|<span data-ttu-id="fc9e9-115">1 </span><span class="sxs-lookup"><span data-stu-id="fc9e9-115">1</span></span>|<span data-ttu-id="fc9e9-116">Ação pendente</span><span class="sxs-lookup"><span data-stu-id="fc9e9-116">Action is pending</span></span>|
|<span data-ttu-id="fc9e9-117">foi</span><span class="sxs-lookup"><span data-stu-id="fc9e9-117">canceled</span></span>|<span data-ttu-id="fc9e9-118">2 </span><span class="sxs-lookup"><span data-stu-id="fc9e9-118">2</span></span>|<span data-ttu-id="fc9e9-119">A ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="fc9e9-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="fc9e9-120">active</span><span class="sxs-lookup"><span data-stu-id="fc9e9-120">active</span></span>|<span data-ttu-id="fc9e9-121">3 </span><span class="sxs-lookup"><span data-stu-id="fc9e9-121">3</span></span>|<span data-ttu-id="fc9e9-122">A ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="fc9e9-122">Action is active.</span></span>|
|<span data-ttu-id="fc9e9-123">done</span><span class="sxs-lookup"><span data-stu-id="fc9e9-123">done</span></span>|<span data-ttu-id="fc9e9-124">4 </span><span class="sxs-lookup"><span data-stu-id="fc9e9-124">4</span></span>|<span data-ttu-id="fc9e9-125">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="fc9e9-125">Action completed without errors.</span></span>|
|<span data-ttu-id="fc9e9-126">falhou</span><span class="sxs-lookup"><span data-stu-id="fc9e9-126">failed</span></span>|<span data-ttu-id="fc9e9-127">5 </span><span class="sxs-lookup"><span data-stu-id="fc9e9-127">5</span></span>|<span data-ttu-id="fc9e9-128">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="fc9e9-128">Action failed</span></span>|
|<span data-ttu-id="fc9e9-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="fc9e9-129">notSupported</span></span>|<span data-ttu-id="fc9e9-130">6 </span><span class="sxs-lookup"><span data-stu-id="fc9e9-130">6</span></span>|<span data-ttu-id="fc9e9-131">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="fc9e9-131">Action is not supported.</span></span>|




