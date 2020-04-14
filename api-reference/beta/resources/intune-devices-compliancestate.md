---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c088f3a0fc3a4bd4b01f29da5f228920f00a398f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465140"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="c466d-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="c466d-103">complianceState enum type</span></span>

<span data-ttu-id="c466d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c466d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c466d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c466d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c466d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c466d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c466d-107">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="c466d-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="c466d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c466d-108">Members</span></span>
|<span data-ttu-id="c466d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c466d-109">Member</span></span>|<span data-ttu-id="c466d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c466d-110">Value</span></span>|<span data-ttu-id="c466d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c466d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c466d-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="c466d-112">unknown</span></span>|<span data-ttu-id="c466d-113">,0</span><span class="sxs-lookup"><span data-stu-id="c466d-113">0</span></span>|<span data-ttu-id="c466d-114">Unknown.</span><span class="sxs-lookup"><span data-stu-id="c466d-114">Unknown.</span></span>|
|<span data-ttu-id="c466d-115">com</span><span class="sxs-lookup"><span data-stu-id="c466d-115">compliant</span></span>|<span data-ttu-id="c466d-116">1</span><span class="sxs-lookup"><span data-stu-id="c466d-116">1</span></span>|<span data-ttu-id="c466d-117">Com.</span><span class="sxs-lookup"><span data-stu-id="c466d-117">Compliant.</span></span>|
|<span data-ttu-id="c466d-118">incompatível</span><span class="sxs-lookup"><span data-stu-id="c466d-118">noncompliant</span></span>|<span data-ttu-id="c466d-119">duas</span><span class="sxs-lookup"><span data-stu-id="c466d-119">2</span></span>|<span data-ttu-id="c466d-120">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="c466d-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="c466d-121">apresentar</span><span class="sxs-lookup"><span data-stu-id="c466d-121">conflict</span></span>|<span data-ttu-id="c466d-122">3D</span><span class="sxs-lookup"><span data-stu-id="c466d-122">3</span></span>|<span data-ttu-id="c466d-123">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="c466d-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="c466d-124">erro</span><span class="sxs-lookup"><span data-stu-id="c466d-124">error</span></span>|<span data-ttu-id="c466d-125">4 </span><span class="sxs-lookup"><span data-stu-id="c466d-125">4</span></span>|<span data-ttu-id="c466d-126">Erro</span><span class="sxs-lookup"><span data-stu-id="c466d-126">Error.</span></span>|
|<span data-ttu-id="c466d-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="c466d-127">inGracePeriod</span></span>|<span data-ttu-id="c466d-128">254</span><span class="sxs-lookup"><span data-stu-id="c466d-128">254</span></span>|<span data-ttu-id="c466d-129">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="c466d-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="c466d-130">configmanager</span><span class="sxs-lookup"><span data-stu-id="c466d-130">configManager</span></span>|<span data-ttu-id="c466d-131">255</span><span class="sxs-lookup"><span data-stu-id="c466d-131">255</span></span>|<span data-ttu-id="c466d-132">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="c466d-132">Managed by Config Manager</span></span>|



