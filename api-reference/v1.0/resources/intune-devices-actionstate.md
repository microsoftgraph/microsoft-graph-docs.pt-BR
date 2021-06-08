---
title: tipo de número actionState
description: Estado da ação no dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7f805b39ac3954981c368ac79e566d3dc4fc218c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760213"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="7df86-103">tipo de número actionState</span><span class="sxs-lookup"><span data-stu-id="7df86-103">actionState enum type</span></span>

<span data-ttu-id="7df86-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7df86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7df86-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7df86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7df86-106">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="7df86-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="7df86-107">Membros</span><span class="sxs-lookup"><span data-stu-id="7df86-107">Members</span></span>
|<span data-ttu-id="7df86-108">Membro</span><span class="sxs-lookup"><span data-stu-id="7df86-108">Member</span></span>|<span data-ttu-id="7df86-109">Valor</span><span class="sxs-lookup"><span data-stu-id="7df86-109">Value</span></span>|<span data-ttu-id="7df86-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7df86-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7df86-111">nenhuma</span><span class="sxs-lookup"><span data-stu-id="7df86-111">none</span></span>|<span data-ttu-id="7df86-112">0</span><span class="sxs-lookup"><span data-stu-id="7df86-112">0</span></span>|<span data-ttu-id="7df86-113">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="7df86-113">Not a valid action state</span></span>|
|<span data-ttu-id="7df86-114">pendente</span><span class="sxs-lookup"><span data-stu-id="7df86-114">pending</span></span>|<span data-ttu-id="7df86-115">1</span><span class="sxs-lookup"><span data-stu-id="7df86-115">1</span></span>|<span data-ttu-id="7df86-116">A ação está pendente</span><span class="sxs-lookup"><span data-stu-id="7df86-116">Action is pending</span></span>|
|<span data-ttu-id="7df86-117">cancelado</span><span class="sxs-lookup"><span data-stu-id="7df86-117">canceled</span></span>|<span data-ttu-id="7df86-118">2</span><span class="sxs-lookup"><span data-stu-id="7df86-118">2</span></span>|<span data-ttu-id="7df86-119">A ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="7df86-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="7df86-120">active</span><span class="sxs-lookup"><span data-stu-id="7df86-120">active</span></span>|<span data-ttu-id="7df86-121">3</span><span class="sxs-lookup"><span data-stu-id="7df86-121">3</span></span>|<span data-ttu-id="7df86-122">A ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="7df86-122">Action is active.</span></span>|
|<span data-ttu-id="7df86-123">done</span><span class="sxs-lookup"><span data-stu-id="7df86-123">done</span></span>|<span data-ttu-id="7df86-124">4 </span><span class="sxs-lookup"><span data-stu-id="7df86-124">4</span></span>|<span data-ttu-id="7df86-125">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="7df86-125">Action completed without errors.</span></span>|
|<span data-ttu-id="7df86-126">failed</span><span class="sxs-lookup"><span data-stu-id="7df86-126">failed</span></span>|<span data-ttu-id="7df86-127">5 </span><span class="sxs-lookup"><span data-stu-id="7df86-127">5</span></span>|<span data-ttu-id="7df86-128">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="7df86-128">Action failed</span></span>|
|<span data-ttu-id="7df86-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="7df86-129">notSupported</span></span>|<span data-ttu-id="7df86-130">6 </span><span class="sxs-lookup"><span data-stu-id="7df86-130">6</span></span>|<span data-ttu-id="7df86-131">Não há suporte para ação.</span><span class="sxs-lookup"><span data-stu-id="7df86-131">Action is not supported.</span></span>|




