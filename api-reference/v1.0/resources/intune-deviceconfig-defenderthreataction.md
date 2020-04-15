---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 24c2b0c60f0451b58e624558fd44f3628c92e3cc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448985"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="fab9b-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="fab9b-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="fab9b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fab9b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fab9b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fab9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fab9b-106">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="fab9b-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="fab9b-107">Membros</span><span class="sxs-lookup"><span data-stu-id="fab9b-107">Members</span></span>
|<span data-ttu-id="fab9b-108">Membro</span><span class="sxs-lookup"><span data-stu-id="fab9b-108">Member</span></span>|<span data-ttu-id="fab9b-109">Valor</span><span class="sxs-lookup"><span data-stu-id="fab9b-109">Value</span></span>|<span data-ttu-id="fab9b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fab9b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fab9b-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="fab9b-111">deviceDefault</span></span>|<span data-ttu-id="fab9b-112">,0</span><span class="sxs-lookup"><span data-stu-id="fab9b-112">0</span></span>|<span data-ttu-id="fab9b-113">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="fab9b-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="fab9b-114">ordena</span><span class="sxs-lookup"><span data-stu-id="fab9b-114">clean</span></span>|<span data-ttu-id="fab9b-115">1</span><span class="sxs-lookup"><span data-stu-id="fab9b-115">1</span></span>|<span data-ttu-id="fab9b-116">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="fab9b-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="fab9b-117">quarentena</span><span class="sxs-lookup"><span data-stu-id="fab9b-117">quarantine</span></span>|<span data-ttu-id="fab9b-118">duas</span><span class="sxs-lookup"><span data-stu-id="fab9b-118">2</span></span>|<span data-ttu-id="fab9b-119">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="fab9b-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="fab9b-120">remover</span><span class="sxs-lookup"><span data-stu-id="fab9b-120">remove</span></span>|<span data-ttu-id="fab9b-121">3D</span><span class="sxs-lookup"><span data-stu-id="fab9b-121">3</span></span>|<span data-ttu-id="fab9b-122">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="fab9b-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="fab9b-123">permitiu</span><span class="sxs-lookup"><span data-stu-id="fab9b-123">allow</span></span>|<span data-ttu-id="fab9b-124">4 </span><span class="sxs-lookup"><span data-stu-id="fab9b-124">4</span></span>|<span data-ttu-id="fab9b-125">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="fab9b-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="fab9b-126">UserDefined</span><span class="sxs-lookup"><span data-stu-id="fab9b-126">userDefined</span></span>|<span data-ttu-id="fab9b-127">5 </span><span class="sxs-lookup"><span data-stu-id="fab9b-127">5</span></span>|<span data-ttu-id="fab9b-128">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="fab9b-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="fab9b-129">Larga</span><span class="sxs-lookup"><span data-stu-id="fab9b-129">block</span></span>|<span data-ttu-id="fab9b-130">6 </span><span class="sxs-lookup"><span data-stu-id="fab9b-130">6</span></span>|<span data-ttu-id="fab9b-131">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="fab9b-131">Block the detected threat.</span></span>|







