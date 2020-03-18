---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1b0ba44c95a49d7646008ac4664926e257c02a19
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785102"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="d389c-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="d389c-103">complianceState enum type</span></span>

> <span data-ttu-id="d389c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d389c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d389c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d389c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d389c-106">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="d389c-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="d389c-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d389c-107">Members</span></span>
|<span data-ttu-id="d389c-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d389c-108">Member</span></span>|<span data-ttu-id="d389c-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d389c-109">Value</span></span>|<span data-ttu-id="d389c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d389c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d389c-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="d389c-111">unknown</span></span>|<span data-ttu-id="d389c-112">,0</span><span class="sxs-lookup"><span data-stu-id="d389c-112">0</span></span>|<span data-ttu-id="d389c-113">Unknown.</span><span class="sxs-lookup"><span data-stu-id="d389c-113">Unknown.</span></span>|
|<span data-ttu-id="d389c-114">com</span><span class="sxs-lookup"><span data-stu-id="d389c-114">compliant</span></span>|<span data-ttu-id="d389c-115">1</span><span class="sxs-lookup"><span data-stu-id="d389c-115">1</span></span>|<span data-ttu-id="d389c-116">Com.</span><span class="sxs-lookup"><span data-stu-id="d389c-116">Compliant.</span></span>|
|<span data-ttu-id="d389c-117">incompatível</span><span class="sxs-lookup"><span data-stu-id="d389c-117">noncompliant</span></span>|<span data-ttu-id="d389c-118">duas</span><span class="sxs-lookup"><span data-stu-id="d389c-118">2</span></span>|<span data-ttu-id="d389c-119">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="d389c-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="d389c-120">apresentar</span><span class="sxs-lookup"><span data-stu-id="d389c-120">conflict</span></span>|<span data-ttu-id="d389c-121">3D</span><span class="sxs-lookup"><span data-stu-id="d389c-121">3</span></span>|<span data-ttu-id="d389c-122">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="d389c-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="d389c-123">erro</span><span class="sxs-lookup"><span data-stu-id="d389c-123">error</span></span>|<span data-ttu-id="d389c-124">4 </span><span class="sxs-lookup"><span data-stu-id="d389c-124">4</span></span>|<span data-ttu-id="d389c-125">Erro</span><span class="sxs-lookup"><span data-stu-id="d389c-125">Error.</span></span>|
|<span data-ttu-id="d389c-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="d389c-126">inGracePeriod</span></span>|<span data-ttu-id="d389c-127">254</span><span class="sxs-lookup"><span data-stu-id="d389c-127">254</span></span>|<span data-ttu-id="d389c-128">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="d389c-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="d389c-129">configmanager</span><span class="sxs-lookup"><span data-stu-id="d389c-129">configManager</span></span>|<span data-ttu-id="d389c-130">255</span><span class="sxs-lookup"><span data-stu-id="d389c-130">255</span></span>|<span data-ttu-id="d389c-131">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="d389c-131">Managed by Config Manager</span></span>|



