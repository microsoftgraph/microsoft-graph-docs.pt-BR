---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9ed1a1ad0d6aee843eed4c1349dd2668f277e6c7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697767"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="8360c-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="8360c-103">complianceState enum type</span></span>

<span data-ttu-id="8360c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8360c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8360c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8360c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8360c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8360c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8360c-107">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="8360c-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="8360c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="8360c-108">Members</span></span>
|<span data-ttu-id="8360c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="8360c-109">Member</span></span>|<span data-ttu-id="8360c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="8360c-110">Value</span></span>|<span data-ttu-id="8360c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8360c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8360c-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="8360c-112">unknown</span></span>|<span data-ttu-id="8360c-113">,0</span><span class="sxs-lookup"><span data-stu-id="8360c-113">0</span></span>|<span data-ttu-id="8360c-114">Unknown.</span><span class="sxs-lookup"><span data-stu-id="8360c-114">Unknown.</span></span>|
|<span data-ttu-id="8360c-115">com</span><span class="sxs-lookup"><span data-stu-id="8360c-115">compliant</span></span>|<span data-ttu-id="8360c-116">1</span><span class="sxs-lookup"><span data-stu-id="8360c-116">1</span></span>|<span data-ttu-id="8360c-117">Com.</span><span class="sxs-lookup"><span data-stu-id="8360c-117">Compliant.</span></span>|
|<span data-ttu-id="8360c-118">incompatível</span><span class="sxs-lookup"><span data-stu-id="8360c-118">noncompliant</span></span>|<span data-ttu-id="8360c-119">duas</span><span class="sxs-lookup"><span data-stu-id="8360c-119">2</span></span>|<span data-ttu-id="8360c-120">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="8360c-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="8360c-121">apresentar</span><span class="sxs-lookup"><span data-stu-id="8360c-121">conflict</span></span>|<span data-ttu-id="8360c-122">3D</span><span class="sxs-lookup"><span data-stu-id="8360c-122">3</span></span>|<span data-ttu-id="8360c-123">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="8360c-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="8360c-124">erro</span><span class="sxs-lookup"><span data-stu-id="8360c-124">error</span></span>|<span data-ttu-id="8360c-125">4 </span><span class="sxs-lookup"><span data-stu-id="8360c-125">4</span></span>|<span data-ttu-id="8360c-126">Erro</span><span class="sxs-lookup"><span data-stu-id="8360c-126">Error.</span></span>|
|<span data-ttu-id="8360c-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="8360c-127">inGracePeriod</span></span>|<span data-ttu-id="8360c-128">254</span><span class="sxs-lookup"><span data-stu-id="8360c-128">254</span></span>|<span data-ttu-id="8360c-129">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="8360c-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="8360c-130">configmanager</span><span class="sxs-lookup"><span data-stu-id="8360c-130">configManager</span></span>|<span data-ttu-id="8360c-131">255</span><span class="sxs-lookup"><span data-stu-id="8360c-131">255</span></span>|<span data-ttu-id="8360c-132">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="8360c-132">Managed by Config Manager</span></span>|





