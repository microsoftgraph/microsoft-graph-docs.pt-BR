---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d578417c616fc2dbf30b8fe95d2f58ede5fd3df2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253355"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="29537-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="29537-103">complianceState enum type</span></span>

> <span data-ttu-id="29537-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29537-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29537-105">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="29537-105">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="29537-106">Membros</span><span class="sxs-lookup"><span data-stu-id="29537-106">Members</span></span>
|<span data-ttu-id="29537-107">Membro</span><span class="sxs-lookup"><span data-stu-id="29537-107">Member</span></span>|<span data-ttu-id="29537-108">Valor</span><span class="sxs-lookup"><span data-stu-id="29537-108">Value</span></span>|<span data-ttu-id="29537-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="29537-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29537-110">unknown</span><span class="sxs-lookup"><span data-stu-id="29537-110">unknown</span></span>|<span data-ttu-id="29537-111">,0</span><span class="sxs-lookup"><span data-stu-id="29537-111">0</span></span>|<span data-ttu-id="29537-112">Unknown.</span><span class="sxs-lookup"><span data-stu-id="29537-112">Unknown.</span></span>|
|<span data-ttu-id="29537-113">com</span><span class="sxs-lookup"><span data-stu-id="29537-113">compliant</span></span>|<span data-ttu-id="29537-114">1</span><span class="sxs-lookup"><span data-stu-id="29537-114">1</span></span>|<span data-ttu-id="29537-115">Com.</span><span class="sxs-lookup"><span data-stu-id="29537-115">Compliant.</span></span>|
|<span data-ttu-id="29537-116">incompatível</span><span class="sxs-lookup"><span data-stu-id="29537-116">noncompliant</span></span>|<span data-ttu-id="29537-117">duas</span><span class="sxs-lookup"><span data-stu-id="29537-117">2</span></span>|<span data-ttu-id="29537-118">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="29537-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="29537-119">apresentar</span><span class="sxs-lookup"><span data-stu-id="29537-119">conflict</span></span>|<span data-ttu-id="29537-120">3D</span><span class="sxs-lookup"><span data-stu-id="29537-120">3</span></span>|<span data-ttu-id="29537-121">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="29537-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="29537-122">erro</span><span class="sxs-lookup"><span data-stu-id="29537-122">error</span></span>|<span data-ttu-id="29537-123">quatro</span><span class="sxs-lookup"><span data-stu-id="29537-123">4</span></span>|<span data-ttu-id="29537-124">Erro</span><span class="sxs-lookup"><span data-stu-id="29537-124">Error.</span></span>|
|<span data-ttu-id="29537-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="29537-125">inGracePeriod</span></span>|<span data-ttu-id="29537-126">254</span><span class="sxs-lookup"><span data-stu-id="29537-126">254</span></span>|<span data-ttu-id="29537-127">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="29537-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="29537-128">configmanager</span><span class="sxs-lookup"><span data-stu-id="29537-128">configManager</span></span>|<span data-ttu-id="29537-129">255</span><span class="sxs-lookup"><span data-stu-id="29537-129">255</span></span>|<span data-ttu-id="29537-130">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="29537-130">Managed by Config Manager</span></span>|



