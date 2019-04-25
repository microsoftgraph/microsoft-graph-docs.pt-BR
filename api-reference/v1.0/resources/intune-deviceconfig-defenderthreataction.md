---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d3d48415e55ad246f75ca9b32bd169ee102fc67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534315"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="4fa1f-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="4fa1f-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="4fa1f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4fa1f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fa1f-105">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="4fa1f-105">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="4fa1f-106">Membros</span><span class="sxs-lookup"><span data-stu-id="4fa1f-106">Members</span></span>
|<span data-ttu-id="4fa1f-107">Membro</span><span class="sxs-lookup"><span data-stu-id="4fa1f-107">Member</span></span>|<span data-ttu-id="4fa1f-108">Valor</span><span class="sxs-lookup"><span data-stu-id="4fa1f-108">Value</span></span>|<span data-ttu-id="4fa1f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fa1f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fa1f-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="4fa1f-110">deviceDefault</span></span>|<span data-ttu-id="4fa1f-111">,0</span><span class="sxs-lookup"><span data-stu-id="4fa1f-111">0</span></span>|<span data-ttu-id="4fa1f-112">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="4fa1f-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="4fa1f-113">ordena</span><span class="sxs-lookup"><span data-stu-id="4fa1f-113">clean</span></span>|<span data-ttu-id="4fa1f-114">1 </span><span class="sxs-lookup"><span data-stu-id="4fa1f-114">1</span></span>|<span data-ttu-id="4fa1f-115">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4fa1f-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="4fa1f-116">quarentena</span><span class="sxs-lookup"><span data-stu-id="4fa1f-116">quarantine</span></span>|<span data-ttu-id="4fa1f-117">2 </span><span class="sxs-lookup"><span data-stu-id="4fa1f-117">2</span></span>|<span data-ttu-id="4fa1f-118">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4fa1f-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="4fa1f-119">remover</span><span class="sxs-lookup"><span data-stu-id="4fa1f-119">remove</span></span>|<span data-ttu-id="4fa1f-120">3 </span><span class="sxs-lookup"><span data-stu-id="4fa1f-120">3</span></span>|<span data-ttu-id="4fa1f-121">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4fa1f-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="4fa1f-122">permitiu</span><span class="sxs-lookup"><span data-stu-id="4fa1f-122">allow</span></span>|<span data-ttu-id="4fa1f-123">4 </span><span class="sxs-lookup"><span data-stu-id="4fa1f-123">4</span></span>|<span data-ttu-id="4fa1f-124">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4fa1f-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="4fa1f-125">userDefined</span><span class="sxs-lookup"><span data-stu-id="4fa1f-125">userDefined</span></span>|<span data-ttu-id="4fa1f-126">5 </span><span class="sxs-lookup"><span data-stu-id="4fa1f-126">5</span></span>|<span data-ttu-id="4fa1f-127">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4fa1f-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="4fa1f-128">Larga</span><span class="sxs-lookup"><span data-stu-id="4fa1f-128">block</span></span>|<span data-ttu-id="4fa1f-129">6 </span><span class="sxs-lookup"><span data-stu-id="4fa1f-129">6</span></span>|<span data-ttu-id="4fa1f-130">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4fa1f-130">Block the detected threat.</span></span>|



