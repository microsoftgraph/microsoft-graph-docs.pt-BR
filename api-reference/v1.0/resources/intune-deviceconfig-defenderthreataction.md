---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e4c9edcd596d6dcd40b2cfe873b660651f74bb3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530857"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="9c834-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="9c834-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="9c834-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c834-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c834-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c834-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c834-106">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="9c834-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="9c834-107">Membros</span><span class="sxs-lookup"><span data-stu-id="9c834-107">Members</span></span>
|<span data-ttu-id="9c834-108">Membro</span><span class="sxs-lookup"><span data-stu-id="9c834-108">Member</span></span>|<span data-ttu-id="9c834-109">Valor</span><span class="sxs-lookup"><span data-stu-id="9c834-109">Value</span></span>|<span data-ttu-id="9c834-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c834-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c834-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9c834-111">deviceDefault</span></span>|<span data-ttu-id="9c834-112">,0</span><span class="sxs-lookup"><span data-stu-id="9c834-112">0</span></span>|<span data-ttu-id="9c834-113">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="9c834-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="9c834-114">ordena</span><span class="sxs-lookup"><span data-stu-id="9c834-114">clean</span></span>|<span data-ttu-id="9c834-115">1 </span><span class="sxs-lookup"><span data-stu-id="9c834-115">1</span></span>|<span data-ttu-id="9c834-116">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="9c834-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="9c834-117">quarentena</span><span class="sxs-lookup"><span data-stu-id="9c834-117">quarantine</span></span>|<span data-ttu-id="9c834-118">2 </span><span class="sxs-lookup"><span data-stu-id="9c834-118">2</span></span>|<span data-ttu-id="9c834-119">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="9c834-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="9c834-120">remover</span><span class="sxs-lookup"><span data-stu-id="9c834-120">remove</span></span>|<span data-ttu-id="9c834-121">3 </span><span class="sxs-lookup"><span data-stu-id="9c834-121">3</span></span>|<span data-ttu-id="9c834-122">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="9c834-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="9c834-123">permitiu</span><span class="sxs-lookup"><span data-stu-id="9c834-123">allow</span></span>|<span data-ttu-id="9c834-124">4 </span><span class="sxs-lookup"><span data-stu-id="9c834-124">4</span></span>|<span data-ttu-id="9c834-125">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="9c834-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="9c834-126">UserDefined</span><span class="sxs-lookup"><span data-stu-id="9c834-126">userDefined</span></span>|<span data-ttu-id="9c834-127">5 </span><span class="sxs-lookup"><span data-stu-id="9c834-127">5</span></span>|<span data-ttu-id="9c834-128">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="9c834-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="9c834-129">Larga</span><span class="sxs-lookup"><span data-stu-id="9c834-129">block</span></span>|<span data-ttu-id="9c834-130">6 </span><span class="sxs-lookup"><span data-stu-id="9c834-130">6</span></span>|<span data-ttu-id="9c834-131">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="9c834-131">Block the detected threat.</span></span>|




