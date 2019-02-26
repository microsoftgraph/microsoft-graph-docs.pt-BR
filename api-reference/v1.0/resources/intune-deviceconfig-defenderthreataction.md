---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d3d48415e55ad246f75ca9b32bd169ee102fc67
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252312"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="e6dda-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="e6dda-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="e6dda-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6dda-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6dda-105">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="e6dda-105">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="e6dda-106">Membros</span><span class="sxs-lookup"><span data-stu-id="e6dda-106">Members</span></span>
|<span data-ttu-id="e6dda-107">Membro</span><span class="sxs-lookup"><span data-stu-id="e6dda-107">Member</span></span>|<span data-ttu-id="e6dda-108">Valor</span><span class="sxs-lookup"><span data-stu-id="e6dda-108">Value</span></span>|<span data-ttu-id="e6dda-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6dda-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6dda-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="e6dda-110">deviceDefault</span></span>|<span data-ttu-id="e6dda-111">,0</span><span class="sxs-lookup"><span data-stu-id="e6dda-111">0</span></span>|<span data-ttu-id="e6dda-112">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="e6dda-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="e6dda-113">clean</span><span class="sxs-lookup"><span data-stu-id="e6dda-113">clean</span></span>|<span data-ttu-id="e6dda-114">1</span><span class="sxs-lookup"><span data-stu-id="e6dda-114">1</span></span>|<span data-ttu-id="e6dda-115">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="e6dda-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="e6dda-116">quarentena</span><span class="sxs-lookup"><span data-stu-id="e6dda-116">quarantine</span></span>|<span data-ttu-id="e6dda-117">duas</span><span class="sxs-lookup"><span data-stu-id="e6dda-117">2</span></span>|<span data-ttu-id="e6dda-118">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="e6dda-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="e6dda-119">remover</span><span class="sxs-lookup"><span data-stu-id="e6dda-119">remove</span></span>|<span data-ttu-id="e6dda-120">3D</span><span class="sxs-lookup"><span data-stu-id="e6dda-120">3</span></span>|<span data-ttu-id="e6dda-121">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="e6dda-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="e6dda-122">permitiu</span><span class="sxs-lookup"><span data-stu-id="e6dda-122">allow</span></span>|<span data-ttu-id="e6dda-123">quatro</span><span class="sxs-lookup"><span data-stu-id="e6dda-123">4</span></span>|<span data-ttu-id="e6dda-124">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="e6dda-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="e6dda-125">userDefined</span><span class="sxs-lookup"><span data-stu-id="e6dda-125">userDefined</span></span>|<span data-ttu-id="e6dda-126">0,5</span><span class="sxs-lookup"><span data-stu-id="e6dda-126">5</span></span>|<span data-ttu-id="e6dda-127">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="e6dda-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="e6dda-128">Larga</span><span class="sxs-lookup"><span data-stu-id="e6dda-128">block</span></span>|<span data-ttu-id="e6dda-129">6</span><span class="sxs-lookup"><span data-stu-id="e6dda-129">6</span></span>|<span data-ttu-id="e6dda-130">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="e6dda-130">Block the detected threat.</span></span>|



