---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 01c0a3443eae87fb69b4b6482a2da2c2e067c5d1
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357056"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="5f1fa-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="5f1fa-103">complianceState enum type</span></span>

> <span data-ttu-id="5f1fa-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f1fa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f1fa-105">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="5f1fa-105">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="5f1fa-106">Membros</span><span class="sxs-lookup"><span data-stu-id="5f1fa-106">Members</span></span>
|<span data-ttu-id="5f1fa-107">Membro</span><span class="sxs-lookup"><span data-stu-id="5f1fa-107">Member</span></span>|<span data-ttu-id="5f1fa-108">Valor</span><span class="sxs-lookup"><span data-stu-id="5f1fa-108">Value</span></span>|<span data-ttu-id="5f1fa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f1fa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f1fa-110">desconhecido</span><span class="sxs-lookup"><span data-stu-id="5f1fa-110">unknown</span></span>|<span data-ttu-id="5f1fa-111">,0</span><span class="sxs-lookup"><span data-stu-id="5f1fa-111">0</span></span>|<span data-ttu-id="5f1fa-112">Unknown.</span><span class="sxs-lookup"><span data-stu-id="5f1fa-112">Unknown.</span></span>|
|<span data-ttu-id="5f1fa-113">com</span><span class="sxs-lookup"><span data-stu-id="5f1fa-113">compliant</span></span>|<span data-ttu-id="5f1fa-114">1</span><span class="sxs-lookup"><span data-stu-id="5f1fa-114">1</span></span>|<span data-ttu-id="5f1fa-115">Com.</span><span class="sxs-lookup"><span data-stu-id="5f1fa-115">Compliant.</span></span>|
|<span data-ttu-id="5f1fa-116">incompatível</span><span class="sxs-lookup"><span data-stu-id="5f1fa-116">noncompliant</span></span>|<span data-ttu-id="5f1fa-117">duas</span><span class="sxs-lookup"><span data-stu-id="5f1fa-117">2</span></span>|<span data-ttu-id="5f1fa-118">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="5f1fa-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="5f1fa-119">apresentar</span><span class="sxs-lookup"><span data-stu-id="5f1fa-119">conflict</span></span>|<span data-ttu-id="5f1fa-120">3D</span><span class="sxs-lookup"><span data-stu-id="5f1fa-120">3</span></span>|<span data-ttu-id="5f1fa-121">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="5f1fa-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="5f1fa-122">erro</span><span class="sxs-lookup"><span data-stu-id="5f1fa-122">error</span></span>|<span data-ttu-id="5f1fa-123">quatro</span><span class="sxs-lookup"><span data-stu-id="5f1fa-123">4</span></span>|<span data-ttu-id="5f1fa-124">Erro</span><span class="sxs-lookup"><span data-stu-id="5f1fa-124">Error.</span></span>|
|<span data-ttu-id="5f1fa-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="5f1fa-125">inGracePeriod</span></span>|<span data-ttu-id="5f1fa-126">254</span><span class="sxs-lookup"><span data-stu-id="5f1fa-126">254</span></span>|<span data-ttu-id="5f1fa-127">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="5f1fa-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="5f1fa-128">configmanager</span><span class="sxs-lookup"><span data-stu-id="5f1fa-128">configManager</span></span>|<span data-ttu-id="5f1fa-129">255</span><span class="sxs-lookup"><span data-stu-id="5f1fa-129">255</span></span>|<span data-ttu-id="5f1fa-130">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="5f1fa-130">Managed by Config Manager</span></span>|




