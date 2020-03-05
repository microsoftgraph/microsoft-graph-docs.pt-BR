---
title: tipo de enumeração windowsDeviceHealthState
description: Estado de proteção do ponto de extremidade do computador
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c5b4c042b93271632df933892ff8296c19c0585b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528420"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="42827-103">tipo de enumeração windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="42827-103">windowsDeviceHealthState enum type</span></span>

<span data-ttu-id="42827-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="42827-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42827-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42827-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42827-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42827-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42827-107">Estado de proteção do ponto de extremidade do computador</span><span class="sxs-lookup"><span data-stu-id="42827-107">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="42827-108">Membros</span><span class="sxs-lookup"><span data-stu-id="42827-108">Members</span></span>
|<span data-ttu-id="42827-109">Membro</span><span class="sxs-lookup"><span data-stu-id="42827-109">Member</span></span>|<span data-ttu-id="42827-110">Valor</span><span class="sxs-lookup"><span data-stu-id="42827-110">Value</span></span>|<span data-ttu-id="42827-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="42827-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42827-112">ordena</span><span class="sxs-lookup"><span data-stu-id="42827-112">clean</span></span>|<span data-ttu-id="42827-113">,0</span><span class="sxs-lookup"><span data-stu-id="42827-113">0</span></span>|<span data-ttu-id="42827-114">O computador está limpo e nenhuma ação é necessária</span><span class="sxs-lookup"><span data-stu-id="42827-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="42827-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="42827-115">fullScanPending</span></span>|<span data-ttu-id="42827-116">1 </span><span class="sxs-lookup"><span data-stu-id="42827-116">1</span></span>|<span data-ttu-id="42827-117">O computador está em estado de verificação completa pendente</span><span class="sxs-lookup"><span data-stu-id="42827-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="42827-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="42827-118">rebootPending</span></span>|<span data-ttu-id="42827-119">2 </span><span class="sxs-lookup"><span data-stu-id="42827-119">2</span></span>|<span data-ttu-id="42827-120">O computador está em estado de reinicialização pendente</span><span class="sxs-lookup"><span data-stu-id="42827-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="42827-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="42827-121">manualStepsPending</span></span>|<span data-ttu-id="42827-122">4 </span><span class="sxs-lookup"><span data-stu-id="42827-122">4</span></span>|<span data-ttu-id="42827-123">O computador está em estado de etapas manuais pendentes</span><span class="sxs-lookup"><span data-stu-id="42827-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="42827-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="42827-124">offlineScanPending</span></span>|<span data-ttu-id="42827-125">8 </span><span class="sxs-lookup"><span data-stu-id="42827-125">8</span></span>|<span data-ttu-id="42827-126">O computador está em estado de verificação offline pendente</span><span class="sxs-lookup"><span data-stu-id="42827-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="42827-127">muito</span><span class="sxs-lookup"><span data-stu-id="42827-127">critical</span></span>|<span data-ttu-id="42827-128">16 </span><span class="sxs-lookup"><span data-stu-id="42827-128">16</span></span>|<span data-ttu-id="42827-129">O computador está em um estado de falha crítico</span><span class="sxs-lookup"><span data-stu-id="42827-129">Computer is in critical failure state</span></span>|



