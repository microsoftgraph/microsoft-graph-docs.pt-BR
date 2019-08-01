---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0195176f322230b3164856575880b9dadc24bce0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031777"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="9e1f7-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="9e1f7-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="9e1f7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e1f7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e1f7-105">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="9e1f7-105">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="9e1f7-106">Membros</span><span class="sxs-lookup"><span data-stu-id="9e1f7-106">Members</span></span>
|<span data-ttu-id="9e1f7-107">Membro</span><span class="sxs-lookup"><span data-stu-id="9e1f7-107">Member</span></span>|<span data-ttu-id="9e1f7-108">Valor</span><span class="sxs-lookup"><span data-stu-id="9e1f7-108">Value</span></span>|<span data-ttu-id="9e1f7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e1f7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e1f7-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9e1f7-110">deviceDefault</span></span>|<span data-ttu-id="9e1f7-111">,0</span><span class="sxs-lookup"><span data-stu-id="9e1f7-111">0</span></span>|<span data-ttu-id="9e1f7-112">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="9e1f7-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="9e1f7-113">ordena</span><span class="sxs-lookup"><span data-stu-id="9e1f7-113">clean</span></span>|<span data-ttu-id="9e1f7-114">1</span><span class="sxs-lookup"><span data-stu-id="9e1f7-114">1</span></span>|<span data-ttu-id="9e1f7-115">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="9e1f7-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="9e1f7-116">quarentena</span><span class="sxs-lookup"><span data-stu-id="9e1f7-116">quarantine</span></span>|<span data-ttu-id="9e1f7-117">duas</span><span class="sxs-lookup"><span data-stu-id="9e1f7-117">2</span></span>|<span data-ttu-id="9e1f7-118">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="9e1f7-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="9e1f7-119">remover</span><span class="sxs-lookup"><span data-stu-id="9e1f7-119">remove</span></span>|<span data-ttu-id="9e1f7-120">3D</span><span class="sxs-lookup"><span data-stu-id="9e1f7-120">3</span></span>|<span data-ttu-id="9e1f7-121">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="9e1f7-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="9e1f7-122">permitiu</span><span class="sxs-lookup"><span data-stu-id="9e1f7-122">allow</span></span>|<span data-ttu-id="9e1f7-123">quatro</span><span class="sxs-lookup"><span data-stu-id="9e1f7-123">4</span></span>|<span data-ttu-id="9e1f7-124">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="9e1f7-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="9e1f7-125">UserDefined</span><span class="sxs-lookup"><span data-stu-id="9e1f7-125">userDefined</span></span>|<span data-ttu-id="9e1f7-126">0,5</span><span class="sxs-lookup"><span data-stu-id="9e1f7-126">5</span></span>|<span data-ttu-id="9e1f7-127">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="9e1f7-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="9e1f7-128">Larga</span><span class="sxs-lookup"><span data-stu-id="9e1f7-128">block</span></span>|<span data-ttu-id="9e1f7-129">6</span><span class="sxs-lookup"><span data-stu-id="9e1f7-129">6</span></span>|<span data-ttu-id="9e1f7-130">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="9e1f7-130">Block the detected threat.</span></span>|



