---
title: tipo de enumeração windowsDeviceHealthState
description: Estado de proteção do ponto de extremidade do computador
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9b37f441a1ded71d3f299d6d38b58543aac130ed
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366446"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="95b2f-103">tipo de enumeração windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="95b2f-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="95b2f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="95b2f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95b2f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95b2f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95b2f-106">Estado de proteção do ponto de extremidade do computador</span><span class="sxs-lookup"><span data-stu-id="95b2f-106">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="95b2f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="95b2f-107">Members</span></span>
|<span data-ttu-id="95b2f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="95b2f-108">Member</span></span>|<span data-ttu-id="95b2f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="95b2f-109">Value</span></span>|<span data-ttu-id="95b2f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="95b2f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95b2f-111">ordena</span><span class="sxs-lookup"><span data-stu-id="95b2f-111">clean</span></span>|<span data-ttu-id="95b2f-112">,0</span><span class="sxs-lookup"><span data-stu-id="95b2f-112">0</span></span>|<span data-ttu-id="95b2f-113">O computador está limpo e nenhuma ação é necessária</span><span class="sxs-lookup"><span data-stu-id="95b2f-113">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="95b2f-114">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="95b2f-114">fullScanPending</span></span>|<span data-ttu-id="95b2f-115">1</span><span class="sxs-lookup"><span data-stu-id="95b2f-115">1</span></span>|<span data-ttu-id="95b2f-116">O computador está em estado de verificação completa pendente</span><span class="sxs-lookup"><span data-stu-id="95b2f-116">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="95b2f-117">rebootPending</span><span class="sxs-lookup"><span data-stu-id="95b2f-117">rebootPending</span></span>|<span data-ttu-id="95b2f-118">duas</span><span class="sxs-lookup"><span data-stu-id="95b2f-118">2</span></span>|<span data-ttu-id="95b2f-119">O computador está em estado de reinicialização pendente</span><span class="sxs-lookup"><span data-stu-id="95b2f-119">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="95b2f-120">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="95b2f-120">manualStepsPending</span></span>|<span data-ttu-id="95b2f-121">quatro</span><span class="sxs-lookup"><span data-stu-id="95b2f-121">4</span></span>|<span data-ttu-id="95b2f-122">O computador está em estado de etapas manuais pendentes</span><span class="sxs-lookup"><span data-stu-id="95b2f-122">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="95b2f-123">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="95b2f-123">offlineScanPending</span></span>|<span data-ttu-id="95b2f-124">8 </span><span class="sxs-lookup"><span data-stu-id="95b2f-124">8</span></span>|<span data-ttu-id="95b2f-125">O computador está em estado de verificação offline pendente</span><span class="sxs-lookup"><span data-stu-id="95b2f-125">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="95b2f-126">muito</span><span class="sxs-lookup"><span data-stu-id="95b2f-126">critical</span></span>|<span data-ttu-id="95b2f-127">dezesseis</span><span class="sxs-lookup"><span data-stu-id="95b2f-127">16</span></span>|<span data-ttu-id="95b2f-128">O computador está em um estado de falha crítico</span><span class="sxs-lookup"><span data-stu-id="95b2f-128">Computer is in critical failure state</span></span>|



