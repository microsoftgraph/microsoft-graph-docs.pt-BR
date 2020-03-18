---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6549b16e325fd8830d0b96de7fd234a315319b8a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794407"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="54406-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="54406-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="54406-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54406-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54406-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54406-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54406-106">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="54406-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="54406-107">Membros</span><span class="sxs-lookup"><span data-stu-id="54406-107">Members</span></span>
|<span data-ttu-id="54406-108">Membro</span><span class="sxs-lookup"><span data-stu-id="54406-108">Member</span></span>|<span data-ttu-id="54406-109">Valor</span><span class="sxs-lookup"><span data-stu-id="54406-109">Value</span></span>|<span data-ttu-id="54406-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="54406-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54406-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="54406-111">deviceDefault</span></span>|<span data-ttu-id="54406-112">,0</span><span class="sxs-lookup"><span data-stu-id="54406-112">0</span></span>|<span data-ttu-id="54406-113">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="54406-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="54406-114">ordena</span><span class="sxs-lookup"><span data-stu-id="54406-114">clean</span></span>|<span data-ttu-id="54406-115">1</span><span class="sxs-lookup"><span data-stu-id="54406-115">1</span></span>|<span data-ttu-id="54406-116">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="54406-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="54406-117">quarentena</span><span class="sxs-lookup"><span data-stu-id="54406-117">quarantine</span></span>|<span data-ttu-id="54406-118">duas</span><span class="sxs-lookup"><span data-stu-id="54406-118">2</span></span>|<span data-ttu-id="54406-119">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="54406-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="54406-120">remover</span><span class="sxs-lookup"><span data-stu-id="54406-120">remove</span></span>|<span data-ttu-id="54406-121">3D</span><span class="sxs-lookup"><span data-stu-id="54406-121">3</span></span>|<span data-ttu-id="54406-122">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="54406-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="54406-123">permitiu</span><span class="sxs-lookup"><span data-stu-id="54406-123">allow</span></span>|<span data-ttu-id="54406-124">4 </span><span class="sxs-lookup"><span data-stu-id="54406-124">4</span></span>|<span data-ttu-id="54406-125">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="54406-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="54406-126">UserDefined</span><span class="sxs-lookup"><span data-stu-id="54406-126">userDefined</span></span>|<span data-ttu-id="54406-127">5 </span><span class="sxs-lookup"><span data-stu-id="54406-127">5</span></span>|<span data-ttu-id="54406-128">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="54406-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="54406-129">Larga</span><span class="sxs-lookup"><span data-stu-id="54406-129">block</span></span>|<span data-ttu-id="54406-130">6 </span><span class="sxs-lookup"><span data-stu-id="54406-130">6</span></span>|<span data-ttu-id="54406-131">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="54406-131">Block the detected threat.</span></span>|



