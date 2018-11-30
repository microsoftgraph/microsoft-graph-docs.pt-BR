---
title: tipo de enum defenderThreatAction
description: Ação de padrão do Defender assuma detectadas ameaças de Malware.
ms.openlocfilehash: a5eb108a3ab26596eec9abe838e3bbfe853d96d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006319"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="c58a0-103">tipo de enum defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="c58a0-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="c58a0-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c58a0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c58a0-105">Ação de padrão do Defender assuma detectadas ameaças de Malware.</span><span class="sxs-lookup"><span data-stu-id="c58a0-105">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="c58a0-106">Membros</span><span class="sxs-lookup"><span data-stu-id="c58a0-106">Members</span></span>
|<span data-ttu-id="c58a0-107">Membro</span><span class="sxs-lookup"><span data-stu-id="c58a0-107">Member</span></span>|<span data-ttu-id="c58a0-108">Valor</span><span class="sxs-lookup"><span data-stu-id="c58a0-108">Value</span></span>|<span data-ttu-id="c58a0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c58a0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c58a0-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c58a0-110">deviceDefault</span></span>|<span data-ttu-id="c58a0-111">0</span><span class="sxs-lookup"><span data-stu-id="c58a0-111">0</span></span>|<span data-ttu-id="c58a0-112">Aplica a ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="c58a0-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="c58a0-113">clean</span><span class="sxs-lookup"><span data-stu-id="c58a0-113">clean</span></span>|<span data-ttu-id="c58a0-114">1</span><span class="sxs-lookup"><span data-stu-id="c58a0-114">1</span></span>|<span data-ttu-id="c58a0-115">Limpe ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="c58a0-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="c58a0-116">quarentena</span><span class="sxs-lookup"><span data-stu-id="c58a0-116">quarantine</span></span>|<span data-ttu-id="c58a0-117">2</span><span class="sxs-lookup"><span data-stu-id="c58a0-117">2</span></span>|<span data-ttu-id="c58a0-118">Quarentena ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="c58a0-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="c58a0-119">remover</span><span class="sxs-lookup"><span data-stu-id="c58a0-119">remove</span></span>|<span data-ttu-id="c58a0-120">3</span><span class="sxs-lookup"><span data-stu-id="c58a0-120">3</span></span>|<span data-ttu-id="c58a0-121">Remova ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="c58a0-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="c58a0-122">permitir</span><span class="sxs-lookup"><span data-stu-id="c58a0-122">allow</span></span>|<span data-ttu-id="c58a0-123">4</span><span class="sxs-lookup"><span data-stu-id="c58a0-123">4</span></span>|<span data-ttu-id="c58a0-124">Permitir ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="c58a0-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="c58a0-125">userDefined</span><span class="sxs-lookup"><span data-stu-id="c58a0-125">userDefined</span></span>|<span data-ttu-id="c58a0-126">5</span><span class="sxs-lookup"><span data-stu-id="c58a0-126">5</span></span>|<span data-ttu-id="c58a0-127">Permitir que o usuário determinar a ação a ser executada com ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="c58a0-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="c58a0-128">bloquear</span><span class="sxs-lookup"><span data-stu-id="c58a0-128">block</span></span>|<span data-ttu-id="c58a0-129">6</span><span class="sxs-lookup"><span data-stu-id="c58a0-129">6</span></span>|<span data-ttu-id="c58a0-130">Bloquear ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="c58a0-130">Block the detected threat.</span></span>|



