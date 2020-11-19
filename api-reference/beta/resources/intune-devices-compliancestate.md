---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a4bff788ff7bed5b06d5efac8247bc55e195c762
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214620"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="20bbb-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="20bbb-103">complianceState enum type</span></span>

<span data-ttu-id="20bbb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20bbb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20bbb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="20bbb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20bbb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20bbb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20bbb-107">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="20bbb-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="20bbb-108">Membros</span><span class="sxs-lookup"><span data-stu-id="20bbb-108">Members</span></span>
|<span data-ttu-id="20bbb-109">Membro</span><span class="sxs-lookup"><span data-stu-id="20bbb-109">Member</span></span>|<span data-ttu-id="20bbb-110">Valor</span><span class="sxs-lookup"><span data-stu-id="20bbb-110">Value</span></span>|<span data-ttu-id="20bbb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="20bbb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20bbb-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="20bbb-112">unknown</span></span>|<span data-ttu-id="20bbb-113">,0</span><span class="sxs-lookup"><span data-stu-id="20bbb-113">0</span></span>|<span data-ttu-id="20bbb-114">Unknown.</span><span class="sxs-lookup"><span data-stu-id="20bbb-114">Unknown.</span></span>|
|<span data-ttu-id="20bbb-115">com</span><span class="sxs-lookup"><span data-stu-id="20bbb-115">compliant</span></span>|<span data-ttu-id="20bbb-116">1</span><span class="sxs-lookup"><span data-stu-id="20bbb-116">1</span></span>|<span data-ttu-id="20bbb-117">Com.</span><span class="sxs-lookup"><span data-stu-id="20bbb-117">Compliant.</span></span>|
|<span data-ttu-id="20bbb-118">incompatível</span><span class="sxs-lookup"><span data-stu-id="20bbb-118">noncompliant</span></span>|<span data-ttu-id="20bbb-119">duas</span><span class="sxs-lookup"><span data-stu-id="20bbb-119">2</span></span>|<span data-ttu-id="20bbb-120">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="20bbb-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="20bbb-121">apresentar</span><span class="sxs-lookup"><span data-stu-id="20bbb-121">conflict</span></span>|<span data-ttu-id="20bbb-122">3D</span><span class="sxs-lookup"><span data-stu-id="20bbb-122">3</span></span>|<span data-ttu-id="20bbb-123">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="20bbb-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="20bbb-124">erro</span><span class="sxs-lookup"><span data-stu-id="20bbb-124">error</span></span>|<span data-ttu-id="20bbb-125">4 </span><span class="sxs-lookup"><span data-stu-id="20bbb-125">4</span></span>|<span data-ttu-id="20bbb-126">Erro</span><span class="sxs-lookup"><span data-stu-id="20bbb-126">Error.</span></span>|
|<span data-ttu-id="20bbb-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="20bbb-127">inGracePeriod</span></span>|<span data-ttu-id="20bbb-128">254</span><span class="sxs-lookup"><span data-stu-id="20bbb-128">254</span></span>|<span data-ttu-id="20bbb-129">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="20bbb-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="20bbb-130">configmanager</span><span class="sxs-lookup"><span data-stu-id="20bbb-130">configManager</span></span>|<span data-ttu-id="20bbb-131">255</span><span class="sxs-lookup"><span data-stu-id="20bbb-131">255</span></span>|<span data-ttu-id="20bbb-132">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="20bbb-132">Managed by Config Manager</span></span>|




