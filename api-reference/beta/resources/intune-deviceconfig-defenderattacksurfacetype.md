---
title: tipo de enumeração defenderAttackSurfaceType
description: Valores possíveis de regras de redução da superfície de ataque do defender
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 435ce477f60f14437a05e22fd5c670cbe1b25796
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256649"
---
# <a name="defenderattacksurfacetype-enum-type"></a><span data-ttu-id="5bb18-103">tipo de enumeração defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="5bb18-103">defenderAttackSurfaceType enum type</span></span>

<span data-ttu-id="5bb18-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bb18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5bb18-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5bb18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bb18-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5bb18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bb18-107">Valores possíveis de regras de redução da superfície de ataque do defender</span><span class="sxs-lookup"><span data-stu-id="5bb18-107">Possible values of Defender Attack Surface Reduction Rules</span></span>

## <a name="members"></a><span data-ttu-id="5bb18-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5bb18-108">Members</span></span>
|<span data-ttu-id="5bb18-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5bb18-109">Member</span></span>|<span data-ttu-id="5bb18-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5bb18-110">Value</span></span>|<span data-ttu-id="5bb18-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5bb18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bb18-112">UserDefined</span><span class="sxs-lookup"><span data-stu-id="5bb18-112">userDefined</span></span>|<span data-ttu-id="5bb18-113">,0</span><span class="sxs-lookup"><span data-stu-id="5bb18-113">0</span></span>|<span data-ttu-id="5bb18-114">Padrão, que desabilita a regra de redução de superfície de ataque.</span><span class="sxs-lookup"><span data-stu-id="5bb18-114">Default, which disables attack surface reduction rule.</span></span>|
|<span data-ttu-id="5bb18-115">Larga</span><span class="sxs-lookup"><span data-stu-id="5bb18-115">block</span></span>|<span data-ttu-id="5bb18-116">1</span><span class="sxs-lookup"><span data-stu-id="5bb18-116">1</span></span>|<span data-ttu-id="5bb18-117">Habilitar a regra de redução de superfície de ataque.</span><span class="sxs-lookup"><span data-stu-id="5bb18-117">Enable the attack surface reduction rule.</span></span>|
|<span data-ttu-id="5bb18-118">auditmode</span><span class="sxs-lookup"><span data-stu-id="5bb18-118">auditMode</span></span>|<span data-ttu-id="5bb18-119">duas</span><span class="sxs-lookup"><span data-stu-id="5bb18-119">2</span></span>|<span data-ttu-id="5bb18-120">Avaliar como a regra ASR afetaria sua organização se estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="5bb18-120">Evaluate how the ASR rule would impact your organization if enabled.</span></span> <span data-ttu-id="5bb18-121">Não altera a funcionalidade, mas gera logs.</span><span class="sxs-lookup"><span data-stu-id="5bb18-121">Does not change functionality but generate logs.</span></span>|
|<span data-ttu-id="5bb18-122">emite</span><span class="sxs-lookup"><span data-stu-id="5bb18-122">warn</span></span>|<span data-ttu-id="5bb18-123">6 </span><span class="sxs-lookup"><span data-stu-id="5bb18-123">6</span></span>|<span data-ttu-id="5bb18-124">Mensagem de aviso para o usuário final com capacidade para ignorar o bloqueio da regra de redução de superfície de ataque.</span><span class="sxs-lookup"><span data-stu-id="5bb18-124">Warning message to end user with ability to bypass block from attack surface reduction rule.</span></span>|
|<span data-ttu-id="5bb18-125">desabilitar</span><span class="sxs-lookup"><span data-stu-id="5bb18-125">disable</span></span>|<span data-ttu-id="5bb18-126">99</span><span class="sxs-lookup"><span data-stu-id="5bb18-126">99</span></span>|<span data-ttu-id="5bb18-127">Desabilitar a regra de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="5bb18-127">Disable the attack surface reduction rule</span></span>|




