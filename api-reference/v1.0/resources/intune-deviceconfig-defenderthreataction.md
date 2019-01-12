---
title: tipo de enum defenderThreatAction
description: Ação de padrão do Defender assuma detectadas ameaças de Malware.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 51aa26483ac6b79d48567f7e5950733def31f01e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976643"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="8c3d7-103">tipo de enum defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="8c3d7-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="8c3d7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8c3d7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c3d7-105">Ação de padrão do Defender assuma detectadas ameaças de Malware.</span><span class="sxs-lookup"><span data-stu-id="8c3d7-105">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="8c3d7-106">Membros</span><span class="sxs-lookup"><span data-stu-id="8c3d7-106">Members</span></span>
|<span data-ttu-id="8c3d7-107">Membro</span><span class="sxs-lookup"><span data-stu-id="8c3d7-107">Member</span></span>|<span data-ttu-id="8c3d7-108">Valor</span><span class="sxs-lookup"><span data-stu-id="8c3d7-108">Value</span></span>|<span data-ttu-id="8c3d7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c3d7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c3d7-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="8c3d7-110">deviceDefault</span></span>|<span data-ttu-id="8c3d7-111">0</span><span class="sxs-lookup"><span data-stu-id="8c3d7-111">0</span></span>|<span data-ttu-id="8c3d7-112">Aplica a ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="8c3d7-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="8c3d7-113">clean</span><span class="sxs-lookup"><span data-stu-id="8c3d7-113">clean</span></span>|<span data-ttu-id="8c3d7-114">1</span><span class="sxs-lookup"><span data-stu-id="8c3d7-114">1</span></span>|<span data-ttu-id="8c3d7-115">Limpe ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="8c3d7-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="8c3d7-116">quarentena</span><span class="sxs-lookup"><span data-stu-id="8c3d7-116">quarantine</span></span>|<span data-ttu-id="8c3d7-117">2</span><span class="sxs-lookup"><span data-stu-id="8c3d7-117">2</span></span>|<span data-ttu-id="8c3d7-118">Quarentena ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="8c3d7-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="8c3d7-119">remover</span><span class="sxs-lookup"><span data-stu-id="8c3d7-119">remove</span></span>|<span data-ttu-id="8c3d7-120">3</span><span class="sxs-lookup"><span data-stu-id="8c3d7-120">3</span></span>|<span data-ttu-id="8c3d7-121">Remova ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="8c3d7-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="8c3d7-122">permitir</span><span class="sxs-lookup"><span data-stu-id="8c3d7-122">allow</span></span>|<span data-ttu-id="8c3d7-123">4</span><span class="sxs-lookup"><span data-stu-id="8c3d7-123">4</span></span>|<span data-ttu-id="8c3d7-124">Permitir ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="8c3d7-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="8c3d7-125">userDefined</span><span class="sxs-lookup"><span data-stu-id="8c3d7-125">userDefined</span></span>|<span data-ttu-id="8c3d7-126">5</span><span class="sxs-lookup"><span data-stu-id="8c3d7-126">5</span></span>|<span data-ttu-id="8c3d7-127">Permitir que o usuário determinar a ação a ser executada com ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="8c3d7-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="8c3d7-128">bloquear</span><span class="sxs-lookup"><span data-stu-id="8c3d7-128">block</span></span>|<span data-ttu-id="8c3d7-129">6</span><span class="sxs-lookup"><span data-stu-id="8c3d7-129">6</span></span>|<span data-ttu-id="8c3d7-130">Bloquear ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="8c3d7-130">Block the detected threat.</span></span>|



