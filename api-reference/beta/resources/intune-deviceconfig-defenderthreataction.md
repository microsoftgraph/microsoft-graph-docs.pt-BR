---
title: tipo de enum defenderThreatAction
description: Ação de padrão do Defender assuma detectadas ameaças de Malware.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d092d5a23fc006a9accdf9062a27cd79f323d208
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400267"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="b8f80-103">tipo de enum defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="b8f80-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="b8f80-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b8f80-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b8f80-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b8f80-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8f80-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b8f80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8f80-107">Ação de padrão do Defender assuma detectadas ameaças de Malware.</span><span class="sxs-lookup"><span data-stu-id="b8f80-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="b8f80-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b8f80-108">Members</span></span>
|<span data-ttu-id="b8f80-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b8f80-109">Member</span></span>|<span data-ttu-id="b8f80-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b8f80-110">Value</span></span>|<span data-ttu-id="b8f80-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8f80-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8f80-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b8f80-112">deviceDefault</span></span>|<span data-ttu-id="b8f80-113">0</span><span class="sxs-lookup"><span data-stu-id="b8f80-113">0</span></span>|<span data-ttu-id="b8f80-114">Aplica a ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="b8f80-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="b8f80-115">clean</span><span class="sxs-lookup"><span data-stu-id="b8f80-115">clean</span></span>|<span data-ttu-id="b8f80-116">1</span><span class="sxs-lookup"><span data-stu-id="b8f80-116">1</span></span>|<span data-ttu-id="b8f80-117">Limpe ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="b8f80-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="b8f80-118">quarentena</span><span class="sxs-lookup"><span data-stu-id="b8f80-118">quarantine</span></span>|<span data-ttu-id="b8f80-119">2</span><span class="sxs-lookup"><span data-stu-id="b8f80-119">2</span></span>|<span data-ttu-id="b8f80-120">Quarentena ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="b8f80-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="b8f80-121">remover</span><span class="sxs-lookup"><span data-stu-id="b8f80-121">remove</span></span>|<span data-ttu-id="b8f80-122">3</span><span class="sxs-lookup"><span data-stu-id="b8f80-122">3</span></span>|<span data-ttu-id="b8f80-123">Remova ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="b8f80-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="b8f80-124">permitir</span><span class="sxs-lookup"><span data-stu-id="b8f80-124">allow</span></span>|<span data-ttu-id="b8f80-125">4</span><span class="sxs-lookup"><span data-stu-id="b8f80-125">4</span></span>|<span data-ttu-id="b8f80-126">Permitir ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="b8f80-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="b8f80-127">userDefined</span><span class="sxs-lookup"><span data-stu-id="b8f80-127">userDefined</span></span>|<span data-ttu-id="b8f80-128">5</span><span class="sxs-lookup"><span data-stu-id="b8f80-128">5</span></span>|<span data-ttu-id="b8f80-129">Permitir que o usuário determinar a ação a ser executada com ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="b8f80-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="b8f80-130">bloquear</span><span class="sxs-lookup"><span data-stu-id="b8f80-130">block</span></span>|<span data-ttu-id="b8f80-131">6</span><span class="sxs-lookup"><span data-stu-id="b8f80-131">6</span></span>|<span data-ttu-id="b8f80-132">Bloquear ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="b8f80-132">Block the detected threat.</span></span>|




