---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 78dc7dfee02a1b1670a2259d20465d4660e73a08
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525149"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="a5041-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="a5041-103">complianceState enum type</span></span>

<span data-ttu-id="a5041-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a5041-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a5041-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a5041-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5041-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5041-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5041-107">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="a5041-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="a5041-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a5041-108">Members</span></span>
|<span data-ttu-id="a5041-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a5041-109">Member</span></span>|<span data-ttu-id="a5041-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a5041-110">Value</span></span>|<span data-ttu-id="a5041-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5041-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5041-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="a5041-112">unknown</span></span>|<span data-ttu-id="a5041-113">,0</span><span class="sxs-lookup"><span data-stu-id="a5041-113">0</span></span>|<span data-ttu-id="a5041-114">Unknown.</span><span class="sxs-lookup"><span data-stu-id="a5041-114">Unknown.</span></span>|
|<span data-ttu-id="a5041-115">com</span><span class="sxs-lookup"><span data-stu-id="a5041-115">compliant</span></span>|<span data-ttu-id="a5041-116">1 </span><span class="sxs-lookup"><span data-stu-id="a5041-116">1</span></span>|<span data-ttu-id="a5041-117">Com.</span><span class="sxs-lookup"><span data-stu-id="a5041-117">Compliant.</span></span>|
|<span data-ttu-id="a5041-118">incompatível</span><span class="sxs-lookup"><span data-stu-id="a5041-118">noncompliant</span></span>|<span data-ttu-id="a5041-119">2 </span><span class="sxs-lookup"><span data-stu-id="a5041-119">2</span></span>|<span data-ttu-id="a5041-120">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="a5041-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="a5041-121">apresentar</span><span class="sxs-lookup"><span data-stu-id="a5041-121">conflict</span></span>|<span data-ttu-id="a5041-122">3 </span><span class="sxs-lookup"><span data-stu-id="a5041-122">3</span></span>|<span data-ttu-id="a5041-123">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="a5041-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="a5041-124">erro</span><span class="sxs-lookup"><span data-stu-id="a5041-124">error</span></span>|<span data-ttu-id="a5041-125">4 </span><span class="sxs-lookup"><span data-stu-id="a5041-125">4</span></span>|<span data-ttu-id="a5041-126">Erro</span><span class="sxs-lookup"><span data-stu-id="a5041-126">Error.</span></span>|
|<span data-ttu-id="a5041-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="a5041-127">inGracePeriod</span></span>|<span data-ttu-id="a5041-128">254</span><span class="sxs-lookup"><span data-stu-id="a5041-128">254</span></span>|<span data-ttu-id="a5041-129">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="a5041-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="a5041-130">configmanager</span><span class="sxs-lookup"><span data-stu-id="a5041-130">configManager</span></span>|<span data-ttu-id="a5041-131">255</span><span class="sxs-lookup"><span data-stu-id="a5041-131">255</span></span>|<span data-ttu-id="a5041-132">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="a5041-132">Managed by Config Manager</span></span>|



