---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 472670b58115d9887ae44a2fb191f1338d058fb4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269361"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="2af04-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="2af04-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="2af04-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2af04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2af04-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2af04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2af04-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2af04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2af04-107">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="2af04-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="2af04-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2af04-108">Members</span></span>
|<span data-ttu-id="2af04-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2af04-109">Member</span></span>|<span data-ttu-id="2af04-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2af04-110">Value</span></span>|<span data-ttu-id="2af04-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2af04-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2af04-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="2af04-112">deviceDefault</span></span>|<span data-ttu-id="2af04-113">,0</span><span class="sxs-lookup"><span data-stu-id="2af04-113">0</span></span>|<span data-ttu-id="2af04-114">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="2af04-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="2af04-115">ordena</span><span class="sxs-lookup"><span data-stu-id="2af04-115">clean</span></span>|<span data-ttu-id="2af04-116">1</span><span class="sxs-lookup"><span data-stu-id="2af04-116">1</span></span>|<span data-ttu-id="2af04-117">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="2af04-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="2af04-118">quarentena</span><span class="sxs-lookup"><span data-stu-id="2af04-118">quarantine</span></span>|<span data-ttu-id="2af04-119">duas</span><span class="sxs-lookup"><span data-stu-id="2af04-119">2</span></span>|<span data-ttu-id="2af04-120">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="2af04-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="2af04-121">remover</span><span class="sxs-lookup"><span data-stu-id="2af04-121">remove</span></span>|<span data-ttu-id="2af04-122">3D</span><span class="sxs-lookup"><span data-stu-id="2af04-122">3</span></span>|<span data-ttu-id="2af04-123">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="2af04-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="2af04-124">permitiu</span><span class="sxs-lookup"><span data-stu-id="2af04-124">allow</span></span>|<span data-ttu-id="2af04-125">4 </span><span class="sxs-lookup"><span data-stu-id="2af04-125">4</span></span>|<span data-ttu-id="2af04-126">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="2af04-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="2af04-127">UserDefined</span><span class="sxs-lookup"><span data-stu-id="2af04-127">userDefined</span></span>|<span data-ttu-id="2af04-128">5 </span><span class="sxs-lookup"><span data-stu-id="2af04-128">5</span></span>|<span data-ttu-id="2af04-129">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="2af04-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="2af04-130">Larga</span><span class="sxs-lookup"><span data-stu-id="2af04-130">block</span></span>|<span data-ttu-id="2af04-131">6 </span><span class="sxs-lookup"><span data-stu-id="2af04-131">6</span></span>|<span data-ttu-id="2af04-132">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="2af04-132">Block the detected threat.</span></span>|




