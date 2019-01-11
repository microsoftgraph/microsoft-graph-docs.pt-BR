---
title: tipo de enum defenderThreatAction
description: Ação de padrão do Defender assuma detectadas ameaças de Malware.
localization_priority: Normal
ms.openlocfilehash: ed84a16dbac493a3e962e37ba246d8d418782a91
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852817"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="15d29-103">tipo de enum defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="15d29-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="15d29-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="15d29-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15d29-105">Ação de padrão do Defender assuma detectadas ameaças de Malware.</span><span class="sxs-lookup"><span data-stu-id="15d29-105">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="15d29-106">Membros</span><span class="sxs-lookup"><span data-stu-id="15d29-106">Members</span></span>
|<span data-ttu-id="15d29-107">Membro</span><span class="sxs-lookup"><span data-stu-id="15d29-107">Member</span></span>|<span data-ttu-id="15d29-108">Valor</span><span class="sxs-lookup"><span data-stu-id="15d29-108">Value</span></span>|<span data-ttu-id="15d29-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="15d29-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15d29-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="15d29-110">deviceDefault</span></span>|<span data-ttu-id="15d29-111">0</span><span class="sxs-lookup"><span data-stu-id="15d29-111">0</span></span>|<span data-ttu-id="15d29-112">Aplica a ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="15d29-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="15d29-113">clean</span><span class="sxs-lookup"><span data-stu-id="15d29-113">clean</span></span>|<span data-ttu-id="15d29-114">1</span><span class="sxs-lookup"><span data-stu-id="15d29-114">1</span></span>|<span data-ttu-id="15d29-115">Limpe ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="15d29-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="15d29-116">quarentena</span><span class="sxs-lookup"><span data-stu-id="15d29-116">quarantine</span></span>|<span data-ttu-id="15d29-117">2</span><span class="sxs-lookup"><span data-stu-id="15d29-117">2</span></span>|<span data-ttu-id="15d29-118">Quarentena ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="15d29-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="15d29-119">remover</span><span class="sxs-lookup"><span data-stu-id="15d29-119">remove</span></span>|<span data-ttu-id="15d29-120">3</span><span class="sxs-lookup"><span data-stu-id="15d29-120">3</span></span>|<span data-ttu-id="15d29-121">Remova ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="15d29-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="15d29-122">permitir</span><span class="sxs-lookup"><span data-stu-id="15d29-122">allow</span></span>|<span data-ttu-id="15d29-123">4</span><span class="sxs-lookup"><span data-stu-id="15d29-123">4</span></span>|<span data-ttu-id="15d29-124">Permitir ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="15d29-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="15d29-125">userDefined</span><span class="sxs-lookup"><span data-stu-id="15d29-125">userDefined</span></span>|<span data-ttu-id="15d29-126">5</span><span class="sxs-lookup"><span data-stu-id="15d29-126">5</span></span>|<span data-ttu-id="15d29-127">Permitir que o usuário determinar a ação a ser executada com ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="15d29-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="15d29-128">bloquear</span><span class="sxs-lookup"><span data-stu-id="15d29-128">block</span></span>|<span data-ttu-id="15d29-129">6</span><span class="sxs-lookup"><span data-stu-id="15d29-129">6</span></span>|<span data-ttu-id="15d29-130">Bloquear ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="15d29-130">Block the detected threat.</span></span>|



