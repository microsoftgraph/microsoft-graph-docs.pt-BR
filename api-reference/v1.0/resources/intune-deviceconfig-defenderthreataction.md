---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d057cf5d052f1fc3043a0b55f4f3ca822f244a7b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041453"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="04b64-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="04b64-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="04b64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04b64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04b64-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04b64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04b64-106">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="04b64-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="04b64-107">Membros</span><span class="sxs-lookup"><span data-stu-id="04b64-107">Members</span></span>
|<span data-ttu-id="04b64-108">Membro</span><span class="sxs-lookup"><span data-stu-id="04b64-108">Member</span></span>|<span data-ttu-id="04b64-109">Valor</span><span class="sxs-lookup"><span data-stu-id="04b64-109">Value</span></span>|<span data-ttu-id="04b64-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="04b64-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04b64-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="04b64-111">deviceDefault</span></span>|<span data-ttu-id="04b64-112">,0</span><span class="sxs-lookup"><span data-stu-id="04b64-112">0</span></span>|<span data-ttu-id="04b64-113">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="04b64-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="04b64-114">ordena</span><span class="sxs-lookup"><span data-stu-id="04b64-114">clean</span></span>|<span data-ttu-id="04b64-115">1 </span><span class="sxs-lookup"><span data-stu-id="04b64-115">1</span></span>|<span data-ttu-id="04b64-116">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="04b64-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="04b64-117">quarentena</span><span class="sxs-lookup"><span data-stu-id="04b64-117">quarantine</span></span>|<span data-ttu-id="04b64-118">2 </span><span class="sxs-lookup"><span data-stu-id="04b64-118">2</span></span>|<span data-ttu-id="04b64-119">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="04b64-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="04b64-120">remover</span><span class="sxs-lookup"><span data-stu-id="04b64-120">remove</span></span>|<span data-ttu-id="04b64-121">3 </span><span class="sxs-lookup"><span data-stu-id="04b64-121">3</span></span>|<span data-ttu-id="04b64-122">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="04b64-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="04b64-123">permitiu</span><span class="sxs-lookup"><span data-stu-id="04b64-123">allow</span></span>|<span data-ttu-id="04b64-124">4 </span><span class="sxs-lookup"><span data-stu-id="04b64-124">4</span></span>|<span data-ttu-id="04b64-125">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="04b64-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="04b64-126">UserDefined</span><span class="sxs-lookup"><span data-stu-id="04b64-126">userDefined</span></span>|<span data-ttu-id="04b64-127">5 </span><span class="sxs-lookup"><span data-stu-id="04b64-127">5</span></span>|<span data-ttu-id="04b64-128">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="04b64-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="04b64-129">Larga</span><span class="sxs-lookup"><span data-stu-id="04b64-129">block</span></span>|<span data-ttu-id="04b64-130">6 </span><span class="sxs-lookup"><span data-stu-id="04b64-130">6</span></span>|<span data-ttu-id="04b64-131">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="04b64-131">Block the detected threat.</span></span>|









