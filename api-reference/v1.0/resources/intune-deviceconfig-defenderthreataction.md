---
title: Tipo de número defenderThreatAction
description: Ação padrão do Defender para assumir ameaças de Malware detectadas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 636d20b3c71b62157946e77230cd8945dd9957cd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758887"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="4ea4e-103">Tipo de número defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="4ea4e-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="4ea4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ea4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ea4e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ea4e-106">Ação padrão do Defender para assumir ameaças de Malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="4ea4e-107">Membros</span><span class="sxs-lookup"><span data-stu-id="4ea4e-107">Members</span></span>
|<span data-ttu-id="4ea4e-108">Membro</span><span class="sxs-lookup"><span data-stu-id="4ea4e-108">Member</span></span>|<span data-ttu-id="4ea4e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="4ea4e-109">Value</span></span>|<span data-ttu-id="4ea4e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ea4e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ea4e-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="4ea4e-111">deviceDefault</span></span>|<span data-ttu-id="4ea4e-112">0</span><span class="sxs-lookup"><span data-stu-id="4ea4e-112">0</span></span>|<span data-ttu-id="4ea4e-113">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="4ea4e-114">clean</span><span class="sxs-lookup"><span data-stu-id="4ea4e-114">clean</span></span>|<span data-ttu-id="4ea4e-115">1</span><span class="sxs-lookup"><span data-stu-id="4ea4e-115">1</span></span>|<span data-ttu-id="4ea4e-116">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="4ea4e-117">quarantine</span><span class="sxs-lookup"><span data-stu-id="4ea4e-117">quarantine</span></span>|<span data-ttu-id="4ea4e-118">2</span><span class="sxs-lookup"><span data-stu-id="4ea4e-118">2</span></span>|<span data-ttu-id="4ea4e-119">Coloque em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="4ea4e-120">remove</span><span class="sxs-lookup"><span data-stu-id="4ea4e-120">remove</span></span>|<span data-ttu-id="4ea4e-121">3</span><span class="sxs-lookup"><span data-stu-id="4ea4e-121">3</span></span>|<span data-ttu-id="4ea4e-122">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="4ea4e-123">allow</span><span class="sxs-lookup"><span data-stu-id="4ea4e-123">allow</span></span>|<span data-ttu-id="4ea4e-124">4 </span><span class="sxs-lookup"><span data-stu-id="4ea4e-124">4</span></span>|<span data-ttu-id="4ea4e-125">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="4ea4e-126">userDefined</span><span class="sxs-lookup"><span data-stu-id="4ea4e-126">userDefined</span></span>|<span data-ttu-id="4ea4e-127">5 </span><span class="sxs-lookup"><span data-stu-id="4ea4e-127">5</span></span>|<span data-ttu-id="4ea4e-128">Permita que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="4ea4e-129">block</span><span class="sxs-lookup"><span data-stu-id="4ea4e-129">block</span></span>|<span data-ttu-id="4ea4e-130">6 </span><span class="sxs-lookup"><span data-stu-id="4ea4e-130">6</span></span>|<span data-ttu-id="4ea4e-131">Bloqueie a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4ea4e-131">Block the detected threat.</span></span>|




