---
title: tipo de número de complianceState
description: Estado de conformidade.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4bae464724712333c81b73bdcd23e57148655624
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757735"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="e0b51-103">tipo de número de complianceState</span><span class="sxs-lookup"><span data-stu-id="e0b51-103">complianceState enum type</span></span>

<span data-ttu-id="e0b51-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0b51-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0b51-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0b51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0b51-106">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="e0b51-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="e0b51-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e0b51-107">Members</span></span>
|<span data-ttu-id="e0b51-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e0b51-108">Member</span></span>|<span data-ttu-id="e0b51-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e0b51-109">Value</span></span>|<span data-ttu-id="e0b51-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0b51-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0b51-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="e0b51-111">unknown</span></span>|<span data-ttu-id="e0b51-112">0</span><span class="sxs-lookup"><span data-stu-id="e0b51-112">0</span></span>|<span data-ttu-id="e0b51-113">Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="e0b51-113">Unknown.</span></span>|
|<span data-ttu-id="e0b51-114">compatível</span><span class="sxs-lookup"><span data-stu-id="e0b51-114">compliant</span></span>|<span data-ttu-id="e0b51-115">1</span><span class="sxs-lookup"><span data-stu-id="e0b51-115">1</span></span>|<span data-ttu-id="e0b51-116">Compatível.</span><span class="sxs-lookup"><span data-stu-id="e0b51-116">Compliant.</span></span>|
|<span data-ttu-id="e0b51-117">noncompliant</span><span class="sxs-lookup"><span data-stu-id="e0b51-117">noncompliant</span></span>|<span data-ttu-id="e0b51-118">2</span><span class="sxs-lookup"><span data-stu-id="e0b51-118">2</span></span>|<span data-ttu-id="e0b51-119">O dispositivo não é compatível e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="e0b51-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="e0b51-120">conflict</span><span class="sxs-lookup"><span data-stu-id="e0b51-120">conflict</span></span>|<span data-ttu-id="e0b51-121">3</span><span class="sxs-lookup"><span data-stu-id="e0b51-121">3</span></span>|<span data-ttu-id="e0b51-122">Conflita com outras regras.</span><span class="sxs-lookup"><span data-stu-id="e0b51-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="e0b51-123">erro</span><span class="sxs-lookup"><span data-stu-id="e0b51-123">error</span></span>|<span data-ttu-id="e0b51-124">4 </span><span class="sxs-lookup"><span data-stu-id="e0b51-124">4</span></span>|<span data-ttu-id="e0b51-125">Erro</span><span class="sxs-lookup"><span data-stu-id="e0b51-125">Error.</span></span>|
|<span data-ttu-id="e0b51-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="e0b51-126">inGracePeriod</span></span>|<span data-ttu-id="e0b51-127">254</span><span class="sxs-lookup"><span data-stu-id="e0b51-127">254</span></span>|<span data-ttu-id="e0b51-128">O dispositivo não é compatível, mas ainda tem acesso a recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="e0b51-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="e0b51-129">configManager</span><span class="sxs-lookup"><span data-stu-id="e0b51-129">configManager</span></span>|<span data-ttu-id="e0b51-130">255</span><span class="sxs-lookup"><span data-stu-id="e0b51-130">255</span></span>|<span data-ttu-id="e0b51-131">Gerenciado pelo Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="e0b51-131">Managed by Config Manager</span></span>|




