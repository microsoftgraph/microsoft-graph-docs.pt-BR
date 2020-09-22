---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3d93ed616a73c69467a1a77cb27e6fb27a7ea553
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024294"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="3a0eb-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="3a0eb-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="3a0eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a0eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a0eb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a0eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a0eb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a0eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a0eb-107">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="3a0eb-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="3a0eb-108">Membros</span><span class="sxs-lookup"><span data-stu-id="3a0eb-108">Members</span></span>
|<span data-ttu-id="3a0eb-109">Membro</span><span class="sxs-lookup"><span data-stu-id="3a0eb-109">Member</span></span>|<span data-ttu-id="3a0eb-110">Valor</span><span class="sxs-lookup"><span data-stu-id="3a0eb-110">Value</span></span>|<span data-ttu-id="3a0eb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a0eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a0eb-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3a0eb-112">deviceDefault</span></span>|<span data-ttu-id="3a0eb-113">,0</span><span class="sxs-lookup"><span data-stu-id="3a0eb-113">0</span></span>|<span data-ttu-id="3a0eb-114">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="3a0eb-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="3a0eb-115">ordena</span><span class="sxs-lookup"><span data-stu-id="3a0eb-115">clean</span></span>|<span data-ttu-id="3a0eb-116">1 </span><span class="sxs-lookup"><span data-stu-id="3a0eb-116">1</span></span>|<span data-ttu-id="3a0eb-117">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="3a0eb-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="3a0eb-118">quarentena</span><span class="sxs-lookup"><span data-stu-id="3a0eb-118">quarantine</span></span>|<span data-ttu-id="3a0eb-119">2 </span><span class="sxs-lookup"><span data-stu-id="3a0eb-119">2</span></span>|<span data-ttu-id="3a0eb-120">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="3a0eb-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="3a0eb-121">remover</span><span class="sxs-lookup"><span data-stu-id="3a0eb-121">remove</span></span>|<span data-ttu-id="3a0eb-122">3 </span><span class="sxs-lookup"><span data-stu-id="3a0eb-122">3</span></span>|<span data-ttu-id="3a0eb-123">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="3a0eb-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="3a0eb-124">permitiu</span><span class="sxs-lookup"><span data-stu-id="3a0eb-124">allow</span></span>|<span data-ttu-id="3a0eb-125">4 </span><span class="sxs-lookup"><span data-stu-id="3a0eb-125">4</span></span>|<span data-ttu-id="3a0eb-126">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="3a0eb-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="3a0eb-127">UserDefined</span><span class="sxs-lookup"><span data-stu-id="3a0eb-127">userDefined</span></span>|<span data-ttu-id="3a0eb-128">5 </span><span class="sxs-lookup"><span data-stu-id="3a0eb-128">5</span></span>|<span data-ttu-id="3a0eb-129">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="3a0eb-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="3a0eb-130">Larga</span><span class="sxs-lookup"><span data-stu-id="3a0eb-130">block</span></span>|<span data-ttu-id="3a0eb-131">6 </span><span class="sxs-lookup"><span data-stu-id="3a0eb-131">6</span></span>|<span data-ttu-id="3a0eb-132">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="3a0eb-132">Block the detected threat.</span></span>|






