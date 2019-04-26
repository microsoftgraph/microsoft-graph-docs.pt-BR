---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e16ea7734b61213286d15467701fa3512ebb7d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563816"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="4f68f-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="4f68f-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="4f68f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f68f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f68f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f68f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f68f-106">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="4f68f-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="4f68f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="4f68f-107">Members</span></span>
|<span data-ttu-id="4f68f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="4f68f-108">Member</span></span>|<span data-ttu-id="4f68f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="4f68f-109">Value</span></span>|<span data-ttu-id="4f68f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f68f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f68f-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="4f68f-111">deviceDefault</span></span>|<span data-ttu-id="4f68f-112">,0</span><span class="sxs-lookup"><span data-stu-id="4f68f-112">0</span></span>|<span data-ttu-id="4f68f-113">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="4f68f-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="4f68f-114">ordena</span><span class="sxs-lookup"><span data-stu-id="4f68f-114">clean</span></span>|<span data-ttu-id="4f68f-115">1 </span><span class="sxs-lookup"><span data-stu-id="4f68f-115">1</span></span>|<span data-ttu-id="4f68f-116">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4f68f-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="4f68f-117">quarentena</span><span class="sxs-lookup"><span data-stu-id="4f68f-117">quarantine</span></span>|<span data-ttu-id="4f68f-118">2 </span><span class="sxs-lookup"><span data-stu-id="4f68f-118">2</span></span>|<span data-ttu-id="4f68f-119">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4f68f-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="4f68f-120">remover</span><span class="sxs-lookup"><span data-stu-id="4f68f-120">remove</span></span>|<span data-ttu-id="4f68f-121">3 </span><span class="sxs-lookup"><span data-stu-id="4f68f-121">3</span></span>|<span data-ttu-id="4f68f-122">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4f68f-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="4f68f-123">permitiu</span><span class="sxs-lookup"><span data-stu-id="4f68f-123">allow</span></span>|<span data-ttu-id="4f68f-124">4 </span><span class="sxs-lookup"><span data-stu-id="4f68f-124">4</span></span>|<span data-ttu-id="4f68f-125">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4f68f-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="4f68f-126">userDefined</span><span class="sxs-lookup"><span data-stu-id="4f68f-126">userDefined</span></span>|<span data-ttu-id="4f68f-127">5 </span><span class="sxs-lookup"><span data-stu-id="4f68f-127">5</span></span>|<span data-ttu-id="4f68f-128">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4f68f-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="4f68f-129">Larga</span><span class="sxs-lookup"><span data-stu-id="4f68f-129">block</span></span>|<span data-ttu-id="4f68f-130">6 </span><span class="sxs-lookup"><span data-stu-id="4f68f-130">6</span></span>|<span data-ttu-id="4f68f-131">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="4f68f-131">Block the detected threat.</span></span>|





