---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bd72afa1d49e39486454304ce27517e9433a137a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420798"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="c2885-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="c2885-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="c2885-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2885-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2885-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c2885-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2885-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c2885-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2885-107">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="c2885-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="c2885-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c2885-108">Members</span></span>
|<span data-ttu-id="c2885-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c2885-109">Member</span></span>|<span data-ttu-id="c2885-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c2885-110">Value</span></span>|<span data-ttu-id="c2885-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2885-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2885-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c2885-112">deviceDefault</span></span>|<span data-ttu-id="c2885-113">,0</span><span class="sxs-lookup"><span data-stu-id="c2885-113">0</span></span>|<span data-ttu-id="c2885-114">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="c2885-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="c2885-115">ordena</span><span class="sxs-lookup"><span data-stu-id="c2885-115">clean</span></span>|<span data-ttu-id="c2885-116">1</span><span class="sxs-lookup"><span data-stu-id="c2885-116">1</span></span>|<span data-ttu-id="c2885-117">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="c2885-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="c2885-118">quarentena</span><span class="sxs-lookup"><span data-stu-id="c2885-118">quarantine</span></span>|<span data-ttu-id="c2885-119">duas</span><span class="sxs-lookup"><span data-stu-id="c2885-119">2</span></span>|<span data-ttu-id="c2885-120">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="c2885-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="c2885-121">remover</span><span class="sxs-lookup"><span data-stu-id="c2885-121">remove</span></span>|<span data-ttu-id="c2885-122">3D</span><span class="sxs-lookup"><span data-stu-id="c2885-122">3</span></span>|<span data-ttu-id="c2885-123">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="c2885-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="c2885-124">permitiu</span><span class="sxs-lookup"><span data-stu-id="c2885-124">allow</span></span>|<span data-ttu-id="c2885-125">4 </span><span class="sxs-lookup"><span data-stu-id="c2885-125">4</span></span>|<span data-ttu-id="c2885-126">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="c2885-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="c2885-127">UserDefined</span><span class="sxs-lookup"><span data-stu-id="c2885-127">userDefined</span></span>|<span data-ttu-id="c2885-128">5 </span><span class="sxs-lookup"><span data-stu-id="c2885-128">5</span></span>|<span data-ttu-id="c2885-129">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="c2885-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="c2885-130">Larga</span><span class="sxs-lookup"><span data-stu-id="c2885-130">block</span></span>|<span data-ttu-id="c2885-131">6 </span><span class="sxs-lookup"><span data-stu-id="c2885-131">6</span></span>|<span data-ttu-id="c2885-132">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="c2885-132">Block the detected threat.</span></span>|



