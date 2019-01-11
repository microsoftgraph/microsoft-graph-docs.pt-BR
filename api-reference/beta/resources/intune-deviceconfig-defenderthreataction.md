---
title: tipo de enum defenderThreatAction
description: Ação de padrão do Defender assuma detectadas ameaças de Malware.
localization_priority: Normal
ms.openlocfilehash: 7e448e6fae0ebbb0f14a3b7932e6f306a70588b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837867"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="37905-103">tipo de enum defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="37905-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="37905-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="37905-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37905-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="37905-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37905-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="37905-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37905-107">Ação de padrão do Defender assuma detectadas ameaças de Malware.</span><span class="sxs-lookup"><span data-stu-id="37905-107">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="37905-108">Membros</span><span class="sxs-lookup"><span data-stu-id="37905-108">Members</span></span>
|<span data-ttu-id="37905-109">Membro</span><span class="sxs-lookup"><span data-stu-id="37905-109">Member</span></span>|<span data-ttu-id="37905-110">Valor</span><span class="sxs-lookup"><span data-stu-id="37905-110">Value</span></span>|<span data-ttu-id="37905-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="37905-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37905-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="37905-112">deviceDefault</span></span>|<span data-ttu-id="37905-113">0</span><span class="sxs-lookup"><span data-stu-id="37905-113">0</span></span>|<span data-ttu-id="37905-114">Aplica a ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="37905-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="37905-115">clean</span><span class="sxs-lookup"><span data-stu-id="37905-115">clean</span></span>|<span data-ttu-id="37905-116">1</span><span class="sxs-lookup"><span data-stu-id="37905-116">1</span></span>|<span data-ttu-id="37905-117">Limpe ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="37905-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="37905-118">quarentena</span><span class="sxs-lookup"><span data-stu-id="37905-118">quarantine</span></span>|<span data-ttu-id="37905-119">2</span><span class="sxs-lookup"><span data-stu-id="37905-119">2</span></span>|<span data-ttu-id="37905-120">Quarentena ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="37905-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="37905-121">remover</span><span class="sxs-lookup"><span data-stu-id="37905-121">remove</span></span>|<span data-ttu-id="37905-122">3</span><span class="sxs-lookup"><span data-stu-id="37905-122">3</span></span>|<span data-ttu-id="37905-123">Remova ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="37905-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="37905-124">permitir</span><span class="sxs-lookup"><span data-stu-id="37905-124">allow</span></span>|<span data-ttu-id="37905-125">4</span><span class="sxs-lookup"><span data-stu-id="37905-125">4</span></span>|<span data-ttu-id="37905-126">Permitir ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="37905-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="37905-127">userDefined</span><span class="sxs-lookup"><span data-stu-id="37905-127">userDefined</span></span>|<span data-ttu-id="37905-128">5</span><span class="sxs-lookup"><span data-stu-id="37905-128">5</span></span>|<span data-ttu-id="37905-129">Permitir que o usuário determinar a ação a ser executada com ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="37905-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="37905-130">bloquear</span><span class="sxs-lookup"><span data-stu-id="37905-130">block</span></span>|<span data-ttu-id="37905-131">6</span><span class="sxs-lookup"><span data-stu-id="37905-131">6</span></span>|<span data-ttu-id="37905-132">Bloquear ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="37905-132">Block the detected threat.</span></span>|





