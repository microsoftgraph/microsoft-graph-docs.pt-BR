---
title: tipo de enum defenderThreatAction
description: Ação de padrão do Defender assuma detectadas ameaças de Malware.
ms.openlocfilehash: d6a4ccbc9725c230f6abc7bd9ee1e38a30d5d133
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033155"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="96d3b-103">tipo de enum defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="96d3b-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="96d3b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="96d3b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96d3b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="96d3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96d3b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="96d3b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96d3b-107">Ação de padrão do Defender assuma detectadas ameaças de Malware.</span><span class="sxs-lookup"><span data-stu-id="96d3b-107">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="96d3b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="96d3b-108">Members</span></span>
|<span data-ttu-id="96d3b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="96d3b-109">Member</span></span>|<span data-ttu-id="96d3b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="96d3b-110">Value</span></span>|<span data-ttu-id="96d3b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="96d3b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96d3b-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="96d3b-112">deviceDefault</span></span>|<span data-ttu-id="96d3b-113">0</span><span class="sxs-lookup"><span data-stu-id="96d3b-113">0</span></span>|<span data-ttu-id="96d3b-114">Aplica a ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="96d3b-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="96d3b-115">clean</span><span class="sxs-lookup"><span data-stu-id="96d3b-115">clean</span></span>|<span data-ttu-id="96d3b-116">1</span><span class="sxs-lookup"><span data-stu-id="96d3b-116">1</span></span>|<span data-ttu-id="96d3b-117">Limpe ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="96d3b-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="96d3b-118">quarentena</span><span class="sxs-lookup"><span data-stu-id="96d3b-118">quarantine</span></span>|<span data-ttu-id="96d3b-119">2</span><span class="sxs-lookup"><span data-stu-id="96d3b-119">2</span></span>|<span data-ttu-id="96d3b-120">Quarentena ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="96d3b-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="96d3b-121">remover</span><span class="sxs-lookup"><span data-stu-id="96d3b-121">remove</span></span>|<span data-ttu-id="96d3b-122">3</span><span class="sxs-lookup"><span data-stu-id="96d3b-122">3</span></span>|<span data-ttu-id="96d3b-123">Remova ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="96d3b-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="96d3b-124">permitir</span><span class="sxs-lookup"><span data-stu-id="96d3b-124">allow</span></span>|<span data-ttu-id="96d3b-125">4</span><span class="sxs-lookup"><span data-stu-id="96d3b-125">4</span></span>|<span data-ttu-id="96d3b-126">Permitir ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="96d3b-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="96d3b-127">userDefined</span><span class="sxs-lookup"><span data-stu-id="96d3b-127">userDefined</span></span>|<span data-ttu-id="96d3b-128">5</span><span class="sxs-lookup"><span data-stu-id="96d3b-128">5</span></span>|<span data-ttu-id="96d3b-129">Permitir que o usuário determinar a ação a ser executada com ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="96d3b-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="96d3b-130">bloquear</span><span class="sxs-lookup"><span data-stu-id="96d3b-130">block</span></span>|<span data-ttu-id="96d3b-131">6</span><span class="sxs-lookup"><span data-stu-id="96d3b-131">6</span></span>|<span data-ttu-id="96d3b-132">Bloquear ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="96d3b-132">Block the detected threat.</span></span>|





