---
title: tipo de enumeração windowsDeviceHealthState
description: Estado de proteção do ponto de extremidade do computador
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ebe11f91b90074839a1a03dab2ce79788f259358
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208055"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="8f0c7-103">tipo de enumeração windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="8f0c7-103">windowsDeviceHealthState enum type</span></span>

<span data-ttu-id="8f0c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f0c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f0c7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8f0c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f0c7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8f0c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f0c7-107">Estado de proteção do ponto de extremidade do computador</span><span class="sxs-lookup"><span data-stu-id="8f0c7-107">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="8f0c7-108">Membros</span><span class="sxs-lookup"><span data-stu-id="8f0c7-108">Members</span></span>
|<span data-ttu-id="8f0c7-109">Membro</span><span class="sxs-lookup"><span data-stu-id="8f0c7-109">Member</span></span>|<span data-ttu-id="8f0c7-110">Valor</span><span class="sxs-lookup"><span data-stu-id="8f0c7-110">Value</span></span>|<span data-ttu-id="8f0c7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f0c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f0c7-112">ordena</span><span class="sxs-lookup"><span data-stu-id="8f0c7-112">clean</span></span>|<span data-ttu-id="8f0c7-113">,0</span><span class="sxs-lookup"><span data-stu-id="8f0c7-113">0</span></span>|<span data-ttu-id="8f0c7-114">O computador está limpo e nenhuma ação é necessária</span><span class="sxs-lookup"><span data-stu-id="8f0c7-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="8f0c7-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="8f0c7-115">fullScanPending</span></span>|<span data-ttu-id="8f0c7-116">1</span><span class="sxs-lookup"><span data-stu-id="8f0c7-116">1</span></span>|<span data-ttu-id="8f0c7-117">O computador está em estado de verificação completa pendente</span><span class="sxs-lookup"><span data-stu-id="8f0c7-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="8f0c7-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="8f0c7-118">rebootPending</span></span>|<span data-ttu-id="8f0c7-119">duas</span><span class="sxs-lookup"><span data-stu-id="8f0c7-119">2</span></span>|<span data-ttu-id="8f0c7-120">O computador está em estado de reinicialização pendente</span><span class="sxs-lookup"><span data-stu-id="8f0c7-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="8f0c7-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="8f0c7-121">manualStepsPending</span></span>|<span data-ttu-id="8f0c7-122">4 </span><span class="sxs-lookup"><span data-stu-id="8f0c7-122">4</span></span>|<span data-ttu-id="8f0c7-123">O computador está em estado de etapas manuais pendentes</span><span class="sxs-lookup"><span data-stu-id="8f0c7-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="8f0c7-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="8f0c7-124">offlineScanPending</span></span>|<span data-ttu-id="8f0c7-125">8 </span><span class="sxs-lookup"><span data-stu-id="8f0c7-125">8</span></span>|<span data-ttu-id="8f0c7-126">O computador está em estado de verificação offline pendente</span><span class="sxs-lookup"><span data-stu-id="8f0c7-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="8f0c7-127">muito</span><span class="sxs-lookup"><span data-stu-id="8f0c7-127">critical</span></span>|<span data-ttu-id="8f0c7-128">16 </span><span class="sxs-lookup"><span data-stu-id="8f0c7-128">16</span></span>|<span data-ttu-id="8f0c7-129">O computador está em um estado de falha crítico</span><span class="sxs-lookup"><span data-stu-id="8f0c7-129">Computer is in critical failure state</span></span>|




