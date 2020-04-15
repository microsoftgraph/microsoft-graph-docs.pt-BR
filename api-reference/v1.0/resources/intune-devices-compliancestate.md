---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1c243145ee8511edb001ba2a55b3f72dde070297
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451283"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="5d73e-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="5d73e-103">complianceState enum type</span></span>

<span data-ttu-id="5d73e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d73e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d73e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5d73e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d73e-106">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="5d73e-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="5d73e-107">Membros</span><span class="sxs-lookup"><span data-stu-id="5d73e-107">Members</span></span>
|<span data-ttu-id="5d73e-108">Membro</span><span class="sxs-lookup"><span data-stu-id="5d73e-108">Member</span></span>|<span data-ttu-id="5d73e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="5d73e-109">Value</span></span>|<span data-ttu-id="5d73e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d73e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d73e-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="5d73e-111">unknown</span></span>|<span data-ttu-id="5d73e-112">,0</span><span class="sxs-lookup"><span data-stu-id="5d73e-112">0</span></span>|<span data-ttu-id="5d73e-113">Unknown.</span><span class="sxs-lookup"><span data-stu-id="5d73e-113">Unknown.</span></span>|
|<span data-ttu-id="5d73e-114">com</span><span class="sxs-lookup"><span data-stu-id="5d73e-114">compliant</span></span>|<span data-ttu-id="5d73e-115">1</span><span class="sxs-lookup"><span data-stu-id="5d73e-115">1</span></span>|<span data-ttu-id="5d73e-116">Com.</span><span class="sxs-lookup"><span data-stu-id="5d73e-116">Compliant.</span></span>|
|<span data-ttu-id="5d73e-117">incompatível</span><span class="sxs-lookup"><span data-stu-id="5d73e-117">noncompliant</span></span>|<span data-ttu-id="5d73e-118">duas</span><span class="sxs-lookup"><span data-stu-id="5d73e-118">2</span></span>|<span data-ttu-id="5d73e-119">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="5d73e-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="5d73e-120">apresentar</span><span class="sxs-lookup"><span data-stu-id="5d73e-120">conflict</span></span>|<span data-ttu-id="5d73e-121">3D</span><span class="sxs-lookup"><span data-stu-id="5d73e-121">3</span></span>|<span data-ttu-id="5d73e-122">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="5d73e-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="5d73e-123">erro</span><span class="sxs-lookup"><span data-stu-id="5d73e-123">error</span></span>|<span data-ttu-id="5d73e-124">4 </span><span class="sxs-lookup"><span data-stu-id="5d73e-124">4</span></span>|<span data-ttu-id="5d73e-125">Erro</span><span class="sxs-lookup"><span data-stu-id="5d73e-125">Error.</span></span>|
|<span data-ttu-id="5d73e-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="5d73e-126">inGracePeriod</span></span>|<span data-ttu-id="5d73e-127">254</span><span class="sxs-lookup"><span data-stu-id="5d73e-127">254</span></span>|<span data-ttu-id="5d73e-128">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="5d73e-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="5d73e-129">configmanager</span><span class="sxs-lookup"><span data-stu-id="5d73e-129">configManager</span></span>|<span data-ttu-id="5d73e-130">255</span><span class="sxs-lookup"><span data-stu-id="5d73e-130">255</span></span>|<span data-ttu-id="5d73e-131">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="5d73e-131">Managed by Config Manager</span></span>|







