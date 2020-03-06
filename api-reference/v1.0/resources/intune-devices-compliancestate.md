---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3b0b20615dfdda489649182d0c0687e9a735b5f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532227"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="321dc-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="321dc-103">complianceState enum type</span></span>

<span data-ttu-id="321dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="321dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="321dc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="321dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="321dc-106">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="321dc-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="321dc-107">Membros</span><span class="sxs-lookup"><span data-stu-id="321dc-107">Members</span></span>
|<span data-ttu-id="321dc-108">Membro</span><span class="sxs-lookup"><span data-stu-id="321dc-108">Member</span></span>|<span data-ttu-id="321dc-109">Valor</span><span class="sxs-lookup"><span data-stu-id="321dc-109">Value</span></span>|<span data-ttu-id="321dc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="321dc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="321dc-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="321dc-111">unknown</span></span>|<span data-ttu-id="321dc-112">,0</span><span class="sxs-lookup"><span data-stu-id="321dc-112">0</span></span>|<span data-ttu-id="321dc-113">Unknown.</span><span class="sxs-lookup"><span data-stu-id="321dc-113">Unknown.</span></span>|
|<span data-ttu-id="321dc-114">com</span><span class="sxs-lookup"><span data-stu-id="321dc-114">compliant</span></span>|<span data-ttu-id="321dc-115">1 </span><span class="sxs-lookup"><span data-stu-id="321dc-115">1</span></span>|<span data-ttu-id="321dc-116">Com.</span><span class="sxs-lookup"><span data-stu-id="321dc-116">Compliant.</span></span>|
|<span data-ttu-id="321dc-117">incompatível</span><span class="sxs-lookup"><span data-stu-id="321dc-117">noncompliant</span></span>|<span data-ttu-id="321dc-118">2 </span><span class="sxs-lookup"><span data-stu-id="321dc-118">2</span></span>|<span data-ttu-id="321dc-119">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="321dc-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="321dc-120">apresentar</span><span class="sxs-lookup"><span data-stu-id="321dc-120">conflict</span></span>|<span data-ttu-id="321dc-121">3 </span><span class="sxs-lookup"><span data-stu-id="321dc-121">3</span></span>|<span data-ttu-id="321dc-122">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="321dc-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="321dc-123">erro</span><span class="sxs-lookup"><span data-stu-id="321dc-123">error</span></span>|<span data-ttu-id="321dc-124">4 </span><span class="sxs-lookup"><span data-stu-id="321dc-124">4</span></span>|<span data-ttu-id="321dc-125">Erro</span><span class="sxs-lookup"><span data-stu-id="321dc-125">Error.</span></span>|
|<span data-ttu-id="321dc-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="321dc-126">inGracePeriod</span></span>|<span data-ttu-id="321dc-127">254</span><span class="sxs-lookup"><span data-stu-id="321dc-127">254</span></span>|<span data-ttu-id="321dc-128">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="321dc-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="321dc-129">configmanager</span><span class="sxs-lookup"><span data-stu-id="321dc-129">configManager</span></span>|<span data-ttu-id="321dc-130">255</span><span class="sxs-lookup"><span data-stu-id="321dc-130">255</span></span>|<span data-ttu-id="321dc-131">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="321dc-131">Managed by Config Manager</span></span>|




