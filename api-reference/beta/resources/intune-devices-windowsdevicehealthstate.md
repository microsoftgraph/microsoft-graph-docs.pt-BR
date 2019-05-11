---
title: tipo de enumeração windowsDeviceHealthState
description: Estado de proteção do ponto de extremidade do computador
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6086dc05d204e4c9cb23c77f79f98c3a207de35c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941888"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="a63f5-103">tipo de enumeração windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="a63f5-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="a63f5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a63f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a63f5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a63f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a63f5-106">Estado de proteção do ponto de extremidade do computador</span><span class="sxs-lookup"><span data-stu-id="a63f5-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="a63f5-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a63f5-107">Members</span></span>
|<span data-ttu-id="a63f5-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a63f5-108">Member</span></span>|<span data-ttu-id="a63f5-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a63f5-109">Value</span></span>|<span data-ttu-id="a63f5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a63f5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a63f5-111">ordena</span><span class="sxs-lookup"><span data-stu-id="a63f5-111">clean</span></span>|<span data-ttu-id="a63f5-112">,0</span><span class="sxs-lookup"><span data-stu-id="a63f5-112">0</span></span>|<span data-ttu-id="a63f5-113">O computador está limpo e nenhuma ação é necessária</span><span class="sxs-lookup"><span data-stu-id="a63f5-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="a63f5-114">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="a63f5-114">fullScanPending</span></span>|<span data-ttu-id="a63f5-115">1</span><span class="sxs-lookup"><span data-stu-id="a63f5-115">1</span></span>|<span data-ttu-id="a63f5-116">O computador está em estado de verificação completa pendente</span><span class="sxs-lookup"><span data-stu-id="a63f5-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="a63f5-117">rebootPending</span><span class="sxs-lookup"><span data-stu-id="a63f5-117">rebootPending</span></span>|<span data-ttu-id="a63f5-118">duas</span><span class="sxs-lookup"><span data-stu-id="a63f5-118">2</span></span>|<span data-ttu-id="a63f5-119">O computador está em estado de reinicialização pendente</span><span class="sxs-lookup"><span data-stu-id="a63f5-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="a63f5-120">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="a63f5-120">manualStepsPending</span></span>|<span data-ttu-id="a63f5-121">quatro</span><span class="sxs-lookup"><span data-stu-id="a63f5-121">4</span></span>|<span data-ttu-id="a63f5-122">O computador está em estado de etapas manuais pendentes</span><span class="sxs-lookup"><span data-stu-id="a63f5-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="a63f5-123">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="a63f5-123">offlineScanPending</span></span>|<span data-ttu-id="a63f5-124">8 </span><span class="sxs-lookup"><span data-stu-id="a63f5-124">8</span></span>|<span data-ttu-id="a63f5-125">O computador está em estado de verificação offline pendente</span><span class="sxs-lookup"><span data-stu-id="a63f5-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="a63f5-126">muito</span><span class="sxs-lookup"><span data-stu-id="a63f5-126">critical</span></span>|<span data-ttu-id="a63f5-127">dezesseis</span><span class="sxs-lookup"><span data-stu-id="a63f5-127">16</span></span>|<span data-ttu-id="a63f5-128">O computador está em um estado de falha crítico</span><span class="sxs-lookup"><span data-stu-id="a63f5-128">Computer is in critical failure state</span></span>|




