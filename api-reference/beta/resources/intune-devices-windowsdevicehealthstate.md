---
title: tipo de enumeração windowsDeviceHealthState
description: Estado de proteção do ponto de extremidade do computador
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7da8a7cc01cef7ff410611e819739e226a4baee1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549475"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="2a555-103">tipo de enumeração windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="2a555-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="2a555-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2a555-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a555-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2a555-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a555-106">Estado de proteção do ponto de extremidade do computador</span><span class="sxs-lookup"><span data-stu-id="2a555-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="2a555-107">Membros</span><span class="sxs-lookup"><span data-stu-id="2a555-107">Members</span></span>
|<span data-ttu-id="2a555-108">Membro</span><span class="sxs-lookup"><span data-stu-id="2a555-108">Member</span></span>|<span data-ttu-id="2a555-109">Valor</span><span class="sxs-lookup"><span data-stu-id="2a555-109">Value</span></span>|<span data-ttu-id="2a555-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a555-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a555-111">ordena</span><span class="sxs-lookup"><span data-stu-id="2a555-111">clean</span></span>|<span data-ttu-id="2a555-112">,0</span><span class="sxs-lookup"><span data-stu-id="2a555-112">0</span></span>|<span data-ttu-id="2a555-113">O computador está limpo e nenhuma ação é necessária</span><span class="sxs-lookup"><span data-stu-id="2a555-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="2a555-114">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="2a555-114">fullScanPending</span></span>|<span data-ttu-id="2a555-115">1 </span><span class="sxs-lookup"><span data-stu-id="2a555-115">1</span></span>|<span data-ttu-id="2a555-116">O computador está em estado de verificação completa pendente</span><span class="sxs-lookup"><span data-stu-id="2a555-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="2a555-117">rebootPending</span><span class="sxs-lookup"><span data-stu-id="2a555-117">rebootPending</span></span>|<span data-ttu-id="2a555-118">2 </span><span class="sxs-lookup"><span data-stu-id="2a555-118">2</span></span>|<span data-ttu-id="2a555-119">O computador está em estado de reinicialização pendente</span><span class="sxs-lookup"><span data-stu-id="2a555-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="2a555-120">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="2a555-120">manualStepsPending</span></span>|<span data-ttu-id="2a555-121">4 </span><span class="sxs-lookup"><span data-stu-id="2a555-121">4</span></span>|<span data-ttu-id="2a555-122">O computador está em estado de etapas manuais pendentes</span><span class="sxs-lookup"><span data-stu-id="2a555-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="2a555-123">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="2a555-123">offlineScanPending</span></span>|<span data-ttu-id="2a555-124">8 </span><span class="sxs-lookup"><span data-stu-id="2a555-124">8</span></span>|<span data-ttu-id="2a555-125">O computador está em estado de verificação offline pendente</span><span class="sxs-lookup"><span data-stu-id="2a555-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="2a555-126">muito</span><span class="sxs-lookup"><span data-stu-id="2a555-126">critical</span></span>|<span data-ttu-id="2a555-127">16 </span><span class="sxs-lookup"><span data-stu-id="2a555-127">16</span></span>|<span data-ttu-id="2a555-128">O computador está em um estado de falha crítico</span><span class="sxs-lookup"><span data-stu-id="2a555-128">Computer is in critical failure state</span></span>|





