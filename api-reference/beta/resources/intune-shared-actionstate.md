---
title: tipo de Enumeração ActionState
description: Estado da ação no dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35fccdc65eec7781f38d366e31ddb1a626005169
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996222"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="4986b-103">tipo de Enumeração ActionState</span><span class="sxs-lookup"><span data-stu-id="4986b-103">actionState enum type</span></span>

> <span data-ttu-id="4986b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4986b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4986b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4986b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4986b-106">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="4986b-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="4986b-107">Membros</span><span class="sxs-lookup"><span data-stu-id="4986b-107">Members</span></span>
|<span data-ttu-id="4986b-108">Membro</span><span class="sxs-lookup"><span data-stu-id="4986b-108">Member</span></span>|<span data-ttu-id="4986b-109">Valor</span><span class="sxs-lookup"><span data-stu-id="4986b-109">Value</span></span>|<span data-ttu-id="4986b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4986b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4986b-111">none</span><span class="sxs-lookup"><span data-stu-id="4986b-111">none</span></span>|<span data-ttu-id="4986b-112">,0</span><span class="sxs-lookup"><span data-stu-id="4986b-112">0</span></span>|<span data-ttu-id="4986b-113">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="4986b-113">Not a valid action state</span></span>|
|<span data-ttu-id="4986b-114">função</span><span class="sxs-lookup"><span data-stu-id="4986b-114">pending</span></span>|<span data-ttu-id="4986b-115">1</span><span class="sxs-lookup"><span data-stu-id="4986b-115">1</span></span>|<span data-ttu-id="4986b-116">Ação pendente</span><span class="sxs-lookup"><span data-stu-id="4986b-116">Action is pending</span></span>|
|<span data-ttu-id="4986b-117">foi</span><span class="sxs-lookup"><span data-stu-id="4986b-117">canceled</span></span>|<span data-ttu-id="4986b-118">duas</span><span class="sxs-lookup"><span data-stu-id="4986b-118">2</span></span>|<span data-ttu-id="4986b-119">A ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="4986b-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="4986b-120">active</span><span class="sxs-lookup"><span data-stu-id="4986b-120">active</span></span>|<span data-ttu-id="4986b-121">3D</span><span class="sxs-lookup"><span data-stu-id="4986b-121">3</span></span>|<span data-ttu-id="4986b-122">A ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="4986b-122">Action is active.</span></span>|
|<span data-ttu-id="4986b-123">done</span><span class="sxs-lookup"><span data-stu-id="4986b-123">done</span></span>|<span data-ttu-id="4986b-124">quatro</span><span class="sxs-lookup"><span data-stu-id="4986b-124">4</span></span>|<span data-ttu-id="4986b-125">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="4986b-125">Action completed without errors.</span></span>|
|<span data-ttu-id="4986b-126">falhou</span><span class="sxs-lookup"><span data-stu-id="4986b-126">failed</span></span>|<span data-ttu-id="4986b-127">0,5</span><span class="sxs-lookup"><span data-stu-id="4986b-127">5</span></span>|<span data-ttu-id="4986b-128">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="4986b-128">Action failed</span></span>|
|<span data-ttu-id="4986b-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="4986b-129">notSupported</span></span>|<span data-ttu-id="4986b-130">6</span><span class="sxs-lookup"><span data-stu-id="4986b-130">6</span></span>|<span data-ttu-id="4986b-131">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="4986b-131">Action is not supported.</span></span>|





