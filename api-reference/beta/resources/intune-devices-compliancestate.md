---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: dea5f5a1bb84d139389416990bbbd4bd96ee9eba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060738"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="cfe18-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="cfe18-103">complianceState enum type</span></span>

<span data-ttu-id="cfe18-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfe18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cfe18-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cfe18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfe18-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cfe18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfe18-107">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="cfe18-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="cfe18-108">Membros</span><span class="sxs-lookup"><span data-stu-id="cfe18-108">Members</span></span>
|<span data-ttu-id="cfe18-109">Membro</span><span class="sxs-lookup"><span data-stu-id="cfe18-109">Member</span></span>|<span data-ttu-id="cfe18-110">Valor</span><span class="sxs-lookup"><span data-stu-id="cfe18-110">Value</span></span>|<span data-ttu-id="cfe18-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfe18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfe18-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="cfe18-112">unknown</span></span>|<span data-ttu-id="cfe18-113">,0</span><span class="sxs-lookup"><span data-stu-id="cfe18-113">0</span></span>|<span data-ttu-id="cfe18-114">Unknown.</span><span class="sxs-lookup"><span data-stu-id="cfe18-114">Unknown.</span></span>|
|<span data-ttu-id="cfe18-115">com</span><span class="sxs-lookup"><span data-stu-id="cfe18-115">compliant</span></span>|<span data-ttu-id="cfe18-116">1 </span><span class="sxs-lookup"><span data-stu-id="cfe18-116">1</span></span>|<span data-ttu-id="cfe18-117">Com.</span><span class="sxs-lookup"><span data-stu-id="cfe18-117">Compliant.</span></span>|
|<span data-ttu-id="cfe18-118">incompatível</span><span class="sxs-lookup"><span data-stu-id="cfe18-118">noncompliant</span></span>|<span data-ttu-id="cfe18-119">2 </span><span class="sxs-lookup"><span data-stu-id="cfe18-119">2</span></span>|<span data-ttu-id="cfe18-120">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="cfe18-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="cfe18-121">apresentar</span><span class="sxs-lookup"><span data-stu-id="cfe18-121">conflict</span></span>|<span data-ttu-id="cfe18-122">3 </span><span class="sxs-lookup"><span data-stu-id="cfe18-122">3</span></span>|<span data-ttu-id="cfe18-123">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="cfe18-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="cfe18-124">erro</span><span class="sxs-lookup"><span data-stu-id="cfe18-124">error</span></span>|<span data-ttu-id="cfe18-125">4 </span><span class="sxs-lookup"><span data-stu-id="cfe18-125">4</span></span>|<span data-ttu-id="cfe18-126">Erro</span><span class="sxs-lookup"><span data-stu-id="cfe18-126">Error.</span></span>|
|<span data-ttu-id="cfe18-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="cfe18-127">inGracePeriod</span></span>|<span data-ttu-id="cfe18-128">254</span><span class="sxs-lookup"><span data-stu-id="cfe18-128">254</span></span>|<span data-ttu-id="cfe18-129">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="cfe18-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="cfe18-130">configmanager</span><span class="sxs-lookup"><span data-stu-id="cfe18-130">configManager</span></span>|<span data-ttu-id="cfe18-131">255</span><span class="sxs-lookup"><span data-stu-id="cfe18-131">255</span></span>|<span data-ttu-id="cfe18-132">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="cfe18-132">Managed by Config Manager</span></span>|






