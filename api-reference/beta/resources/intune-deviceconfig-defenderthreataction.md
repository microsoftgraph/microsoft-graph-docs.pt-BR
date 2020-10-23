---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bd71ee742ba7d7b5a98c5f3bbf90496bb52392be
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696262"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="dbe4e-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="dbe4e-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="dbe4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbe4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbe4e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dbe4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbe4e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dbe4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbe4e-107">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="dbe4e-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="dbe4e-108">Membros</span><span class="sxs-lookup"><span data-stu-id="dbe4e-108">Members</span></span>
|<span data-ttu-id="dbe4e-109">Membro</span><span class="sxs-lookup"><span data-stu-id="dbe4e-109">Member</span></span>|<span data-ttu-id="dbe4e-110">Valor</span><span class="sxs-lookup"><span data-stu-id="dbe4e-110">Value</span></span>|<span data-ttu-id="dbe4e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbe4e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbe4e-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="dbe4e-112">deviceDefault</span></span>|<span data-ttu-id="dbe4e-113">,0</span><span class="sxs-lookup"><span data-stu-id="dbe4e-113">0</span></span>|<span data-ttu-id="dbe4e-114">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="dbe4e-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="dbe4e-115">ordena</span><span class="sxs-lookup"><span data-stu-id="dbe4e-115">clean</span></span>|<span data-ttu-id="dbe4e-116">1</span><span class="sxs-lookup"><span data-stu-id="dbe4e-116">1</span></span>|<span data-ttu-id="dbe4e-117">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="dbe4e-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="dbe4e-118">quarentena</span><span class="sxs-lookup"><span data-stu-id="dbe4e-118">quarantine</span></span>|<span data-ttu-id="dbe4e-119">duas</span><span class="sxs-lookup"><span data-stu-id="dbe4e-119">2</span></span>|<span data-ttu-id="dbe4e-120">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="dbe4e-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="dbe4e-121">remover</span><span class="sxs-lookup"><span data-stu-id="dbe4e-121">remove</span></span>|<span data-ttu-id="dbe4e-122">3D</span><span class="sxs-lookup"><span data-stu-id="dbe4e-122">3</span></span>|<span data-ttu-id="dbe4e-123">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="dbe4e-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="dbe4e-124">permitiu</span><span class="sxs-lookup"><span data-stu-id="dbe4e-124">allow</span></span>|<span data-ttu-id="dbe4e-125">4 </span><span class="sxs-lookup"><span data-stu-id="dbe4e-125">4</span></span>|<span data-ttu-id="dbe4e-126">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="dbe4e-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="dbe4e-127">UserDefined</span><span class="sxs-lookup"><span data-stu-id="dbe4e-127">userDefined</span></span>|<span data-ttu-id="dbe4e-128">5 </span><span class="sxs-lookup"><span data-stu-id="dbe4e-128">5</span></span>|<span data-ttu-id="dbe4e-129">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="dbe4e-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="dbe4e-130">Larga</span><span class="sxs-lookup"><span data-stu-id="dbe4e-130">block</span></span>|<span data-ttu-id="dbe4e-131">6 </span><span class="sxs-lookup"><span data-stu-id="dbe4e-131">6</span></span>|<span data-ttu-id="dbe4e-132">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="dbe4e-132">Block the detected threat.</span></span>|





