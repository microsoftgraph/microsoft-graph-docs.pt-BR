---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 24f7a2a62ae45504c03d2fcff49ca8f17bfab28b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091303"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="61b58-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="61b58-103">complianceState enum type</span></span>

<span data-ttu-id="61b58-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61b58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61b58-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61b58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61b58-106">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="61b58-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="61b58-107">Membros</span><span class="sxs-lookup"><span data-stu-id="61b58-107">Members</span></span>
|<span data-ttu-id="61b58-108">Membro</span><span class="sxs-lookup"><span data-stu-id="61b58-108">Member</span></span>|<span data-ttu-id="61b58-109">Valor</span><span class="sxs-lookup"><span data-stu-id="61b58-109">Value</span></span>|<span data-ttu-id="61b58-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="61b58-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61b58-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="61b58-111">unknown</span></span>|<span data-ttu-id="61b58-112">,0</span><span class="sxs-lookup"><span data-stu-id="61b58-112">0</span></span>|<span data-ttu-id="61b58-113">Unknown.</span><span class="sxs-lookup"><span data-stu-id="61b58-113">Unknown.</span></span>|
|<span data-ttu-id="61b58-114">com</span><span class="sxs-lookup"><span data-stu-id="61b58-114">compliant</span></span>|<span data-ttu-id="61b58-115">1 </span><span class="sxs-lookup"><span data-stu-id="61b58-115">1</span></span>|<span data-ttu-id="61b58-116">Com.</span><span class="sxs-lookup"><span data-stu-id="61b58-116">Compliant.</span></span>|
|<span data-ttu-id="61b58-117">incompatível</span><span class="sxs-lookup"><span data-stu-id="61b58-117">noncompliant</span></span>|<span data-ttu-id="61b58-118">2 </span><span class="sxs-lookup"><span data-stu-id="61b58-118">2</span></span>|<span data-ttu-id="61b58-119">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="61b58-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="61b58-120">apresentar</span><span class="sxs-lookup"><span data-stu-id="61b58-120">conflict</span></span>|<span data-ttu-id="61b58-121">3D</span><span class="sxs-lookup"><span data-stu-id="61b58-121">3</span></span>|<span data-ttu-id="61b58-122">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="61b58-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="61b58-123">erro</span><span class="sxs-lookup"><span data-stu-id="61b58-123">error</span></span>|<span data-ttu-id="61b58-124">4 </span><span class="sxs-lookup"><span data-stu-id="61b58-124">4</span></span>|<span data-ttu-id="61b58-125">Erro</span><span class="sxs-lookup"><span data-stu-id="61b58-125">Error.</span></span>|
|<span data-ttu-id="61b58-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="61b58-126">inGracePeriod</span></span>|<span data-ttu-id="61b58-127">254</span><span class="sxs-lookup"><span data-stu-id="61b58-127">254</span></span>|<span data-ttu-id="61b58-128">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="61b58-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="61b58-129">configmanager</span><span class="sxs-lookup"><span data-stu-id="61b58-129">configManager</span></span>|<span data-ttu-id="61b58-130">255</span><span class="sxs-lookup"><span data-stu-id="61b58-130">255</span></span>|<span data-ttu-id="61b58-131">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="61b58-131">Managed by Config Manager</span></span>|









