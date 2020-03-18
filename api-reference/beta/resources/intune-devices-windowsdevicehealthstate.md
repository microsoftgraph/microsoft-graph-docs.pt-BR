---
title: tipo de enumeração windowsDeviceHealthState
description: Estado de proteção do ponto de extremidade do computador
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 69d20e06ba23390ff912251bb99980c4a945704c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783708"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="f1005-103">tipo de enumeração windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="f1005-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="f1005-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f1005-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1005-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1005-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1005-106">Estado de proteção do ponto de extremidade do computador</span><span class="sxs-lookup"><span data-stu-id="f1005-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="f1005-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f1005-107">Members</span></span>
|<span data-ttu-id="f1005-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f1005-108">Member</span></span>|<span data-ttu-id="f1005-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f1005-109">Value</span></span>|<span data-ttu-id="f1005-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1005-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1005-111">ordena</span><span class="sxs-lookup"><span data-stu-id="f1005-111">clean</span></span>|<span data-ttu-id="f1005-112">,0</span><span class="sxs-lookup"><span data-stu-id="f1005-112">0</span></span>|<span data-ttu-id="f1005-113">O computador está limpo e nenhuma ação é necessária</span><span class="sxs-lookup"><span data-stu-id="f1005-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="f1005-114">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="f1005-114">fullScanPending</span></span>|<span data-ttu-id="f1005-115">1</span><span class="sxs-lookup"><span data-stu-id="f1005-115">1</span></span>|<span data-ttu-id="f1005-116">O computador está em estado de verificação completa pendente</span><span class="sxs-lookup"><span data-stu-id="f1005-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="f1005-117">rebootPending</span><span class="sxs-lookup"><span data-stu-id="f1005-117">rebootPending</span></span>|<span data-ttu-id="f1005-118">duas</span><span class="sxs-lookup"><span data-stu-id="f1005-118">2</span></span>|<span data-ttu-id="f1005-119">O computador está em estado de reinicialização pendente</span><span class="sxs-lookup"><span data-stu-id="f1005-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="f1005-120">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="f1005-120">manualStepsPending</span></span>|<span data-ttu-id="f1005-121">4 </span><span class="sxs-lookup"><span data-stu-id="f1005-121">4</span></span>|<span data-ttu-id="f1005-122">O computador está em estado de etapas manuais pendentes</span><span class="sxs-lookup"><span data-stu-id="f1005-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="f1005-123">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="f1005-123">offlineScanPending</span></span>|<span data-ttu-id="f1005-124">8 </span><span class="sxs-lookup"><span data-stu-id="f1005-124">8</span></span>|<span data-ttu-id="f1005-125">O computador está em estado de verificação offline pendente</span><span class="sxs-lookup"><span data-stu-id="f1005-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="f1005-126">muito</span><span class="sxs-lookup"><span data-stu-id="f1005-126">critical</span></span>|<span data-ttu-id="f1005-127">16 </span><span class="sxs-lookup"><span data-stu-id="f1005-127">16</span></span>|<span data-ttu-id="f1005-128">O computador está em um estado de falha crítico</span><span class="sxs-lookup"><span data-stu-id="f1005-128">Computer is in critical failure state</span></span>|



