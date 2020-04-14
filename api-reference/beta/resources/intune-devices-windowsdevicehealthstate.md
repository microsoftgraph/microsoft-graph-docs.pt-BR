---
title: tipo de enumeração windowsDeviceHealthState
description: Estado de proteção do ponto de extremidade do computador
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1ce06c1b6c52266bb7d052a4524c6f4439973bde
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401747"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="3f1f1-103">tipo de enumeração windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="3f1f1-103">windowsDeviceHealthState enum type</span></span>

<span data-ttu-id="3f1f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f1f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f1f1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3f1f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f1f1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f1f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f1f1-107">Estado de proteção do ponto de extremidade do computador</span><span class="sxs-lookup"><span data-stu-id="3f1f1-107">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="3f1f1-108">Membros</span><span class="sxs-lookup"><span data-stu-id="3f1f1-108">Members</span></span>
|<span data-ttu-id="3f1f1-109">Membro</span><span class="sxs-lookup"><span data-stu-id="3f1f1-109">Member</span></span>|<span data-ttu-id="3f1f1-110">Valor</span><span class="sxs-lookup"><span data-stu-id="3f1f1-110">Value</span></span>|<span data-ttu-id="3f1f1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f1f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f1f1-112">ordena</span><span class="sxs-lookup"><span data-stu-id="3f1f1-112">clean</span></span>|<span data-ttu-id="3f1f1-113">,0</span><span class="sxs-lookup"><span data-stu-id="3f1f1-113">0</span></span>|<span data-ttu-id="3f1f1-114">O computador está limpo e nenhuma ação é necessária</span><span class="sxs-lookup"><span data-stu-id="3f1f1-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="3f1f1-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="3f1f1-115">fullScanPending</span></span>|<span data-ttu-id="3f1f1-116">1</span><span class="sxs-lookup"><span data-stu-id="3f1f1-116">1</span></span>|<span data-ttu-id="3f1f1-117">O computador está em estado de verificação completa pendente</span><span class="sxs-lookup"><span data-stu-id="3f1f1-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="3f1f1-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="3f1f1-118">rebootPending</span></span>|<span data-ttu-id="3f1f1-119">duas</span><span class="sxs-lookup"><span data-stu-id="3f1f1-119">2</span></span>|<span data-ttu-id="3f1f1-120">O computador está em estado de reinicialização pendente</span><span class="sxs-lookup"><span data-stu-id="3f1f1-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="3f1f1-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="3f1f1-121">manualStepsPending</span></span>|<span data-ttu-id="3f1f1-122">4 </span><span class="sxs-lookup"><span data-stu-id="3f1f1-122">4</span></span>|<span data-ttu-id="3f1f1-123">O computador está em estado de etapas manuais pendentes</span><span class="sxs-lookup"><span data-stu-id="3f1f1-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="3f1f1-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="3f1f1-124">offlineScanPending</span></span>|<span data-ttu-id="3f1f1-125">8 </span><span class="sxs-lookup"><span data-stu-id="3f1f1-125">8</span></span>|<span data-ttu-id="3f1f1-126">O computador está em estado de verificação offline pendente</span><span class="sxs-lookup"><span data-stu-id="3f1f1-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="3f1f1-127">muito</span><span class="sxs-lookup"><span data-stu-id="3f1f1-127">critical</span></span>|<span data-ttu-id="3f1f1-128">16 </span><span class="sxs-lookup"><span data-stu-id="3f1f1-128">16</span></span>|<span data-ttu-id="3f1f1-129">O computador está em um estado de falha crítico</span><span class="sxs-lookup"><span data-stu-id="3f1f1-129">Computer is in critical failure state</span></span>|



