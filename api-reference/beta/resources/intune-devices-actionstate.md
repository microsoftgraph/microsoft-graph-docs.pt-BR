---
title: tipo de número actionState
description: Estado da ação no dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 99b7b189ed0e3f8a66eeaa4c099421b3b13e0989
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612107"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="f9ee6-103">tipo de número actionState</span><span class="sxs-lookup"><span data-stu-id="f9ee6-103">actionState enum type</span></span>

<span data-ttu-id="f9ee6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9ee6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9ee6-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9ee6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9ee6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9ee6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9ee6-107">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="f9ee6-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="f9ee6-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f9ee6-108">Members</span></span>
|<span data-ttu-id="f9ee6-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f9ee6-109">Member</span></span>|<span data-ttu-id="f9ee6-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f9ee6-110">Value</span></span>|<span data-ttu-id="f9ee6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9ee6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9ee6-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="f9ee6-112">none</span></span>|<span data-ttu-id="f9ee6-113">0</span><span class="sxs-lookup"><span data-stu-id="f9ee6-113">0</span></span>|<span data-ttu-id="f9ee6-114">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="f9ee6-114">Not a valid action state</span></span>|
|<span data-ttu-id="f9ee6-115">pendente</span><span class="sxs-lookup"><span data-stu-id="f9ee6-115">pending</span></span>|<span data-ttu-id="f9ee6-116">1</span><span class="sxs-lookup"><span data-stu-id="f9ee6-116">1</span></span>|<span data-ttu-id="f9ee6-117">A ação está pendente</span><span class="sxs-lookup"><span data-stu-id="f9ee6-117">Action is pending</span></span>|
|<span data-ttu-id="f9ee6-118">cancelado</span><span class="sxs-lookup"><span data-stu-id="f9ee6-118">canceled</span></span>|<span data-ttu-id="f9ee6-119">2</span><span class="sxs-lookup"><span data-stu-id="f9ee6-119">2</span></span>|<span data-ttu-id="f9ee6-120">A ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="f9ee6-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="f9ee6-121">active</span><span class="sxs-lookup"><span data-stu-id="f9ee6-121">active</span></span>|<span data-ttu-id="f9ee6-122">3</span><span class="sxs-lookup"><span data-stu-id="f9ee6-122">3</span></span>|<span data-ttu-id="f9ee6-123">A ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="f9ee6-123">Action is active.</span></span>|
|<span data-ttu-id="f9ee6-124">done</span><span class="sxs-lookup"><span data-stu-id="f9ee6-124">done</span></span>|<span data-ttu-id="f9ee6-125">4 </span><span class="sxs-lookup"><span data-stu-id="f9ee6-125">4</span></span>|<span data-ttu-id="f9ee6-126">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="f9ee6-126">Action completed without errors.</span></span>|
|<span data-ttu-id="f9ee6-127">failed</span><span class="sxs-lookup"><span data-stu-id="f9ee6-127">failed</span></span>|<span data-ttu-id="f9ee6-128">5 </span><span class="sxs-lookup"><span data-stu-id="f9ee6-128">5</span></span>|<span data-ttu-id="f9ee6-129">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="f9ee6-129">Action failed</span></span>|
|<span data-ttu-id="f9ee6-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="f9ee6-130">notSupported</span></span>|<span data-ttu-id="f9ee6-131">6 </span><span class="sxs-lookup"><span data-stu-id="f9ee6-131">6</span></span>|<span data-ttu-id="f9ee6-132">Não há suporte para ação.</span><span class="sxs-lookup"><span data-stu-id="f9ee6-132">Action is not supported.</span></span>|




