---
title: tipo de Enumeração ActionState
description: Estado da ação no dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1188670476e911b01375598a2361aae326a98425
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566315"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="94707-103">tipo de Enumeração ActionState</span><span class="sxs-lookup"><span data-stu-id="94707-103">actionState enum type</span></span>

> <span data-ttu-id="94707-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94707-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94707-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94707-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94707-106">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="94707-106">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="94707-107">Membros</span><span class="sxs-lookup"><span data-stu-id="94707-107">Members</span></span>
|<span data-ttu-id="94707-108">Membro</span><span class="sxs-lookup"><span data-stu-id="94707-108">Member</span></span>|<span data-ttu-id="94707-109">Valor</span><span class="sxs-lookup"><span data-stu-id="94707-109">Value</span></span>|<span data-ttu-id="94707-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="94707-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94707-111">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="94707-111">none</span></span>|<span data-ttu-id="94707-112">,0</span><span class="sxs-lookup"><span data-stu-id="94707-112">0</span></span>|<span data-ttu-id="94707-113">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="94707-113">Not a valid action state</span></span>|
|<span data-ttu-id="94707-114">função</span><span class="sxs-lookup"><span data-stu-id="94707-114">pending</span></span>|<span data-ttu-id="94707-115">1 </span><span class="sxs-lookup"><span data-stu-id="94707-115">1</span></span>|<span data-ttu-id="94707-116">Ação pendente</span><span class="sxs-lookup"><span data-stu-id="94707-116">Action is pending</span></span>|
|<span data-ttu-id="94707-117">foi</span><span class="sxs-lookup"><span data-stu-id="94707-117">canceled</span></span>|<span data-ttu-id="94707-118">2 </span><span class="sxs-lookup"><span data-stu-id="94707-118">2</span></span>|<span data-ttu-id="94707-119">A ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="94707-119">Action has been cancelled.</span></span>|
|<span data-ttu-id="94707-120">active</span><span class="sxs-lookup"><span data-stu-id="94707-120">active</span></span>|<span data-ttu-id="94707-121">3 </span><span class="sxs-lookup"><span data-stu-id="94707-121">3</span></span>|<span data-ttu-id="94707-122">A ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="94707-122">Action is active.</span></span>|
|<span data-ttu-id="94707-123">done</span><span class="sxs-lookup"><span data-stu-id="94707-123">done</span></span>|<span data-ttu-id="94707-124">4 </span><span class="sxs-lookup"><span data-stu-id="94707-124">4</span></span>|<span data-ttu-id="94707-125">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="94707-125">Action completed without errors.</span></span>|
|<span data-ttu-id="94707-126">falhou</span><span class="sxs-lookup"><span data-stu-id="94707-126">failed</span></span>|<span data-ttu-id="94707-127">5 </span><span class="sxs-lookup"><span data-stu-id="94707-127">5</span></span>|<span data-ttu-id="94707-128">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="94707-128">Action failed</span></span>|
|<span data-ttu-id="94707-129">notSupported</span><span class="sxs-lookup"><span data-stu-id="94707-129">notSupported</span></span>|<span data-ttu-id="94707-130">6 </span><span class="sxs-lookup"><span data-stu-id="94707-130">6</span></span>|<span data-ttu-id="94707-131">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="94707-131">Action is not supported.</span></span>|





