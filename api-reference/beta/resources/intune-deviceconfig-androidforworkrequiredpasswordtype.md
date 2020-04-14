---
title: tipo de enumeração androidForWorkRequiredPasswordType
description: Android para o tipo de senha de trabalho necessário.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 60cf442d821aabb4e9e6ca07e46d69cfc2f9b107
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444412"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="c63ce-103">tipo de enumeração androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c63ce-103">androidForWorkRequiredPasswordType enum type</span></span>

<span data-ttu-id="c63ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c63ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c63ce-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c63ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c63ce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c63ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c63ce-107">Android para o tipo de senha de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="c63ce-107">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="c63ce-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c63ce-108">Members</span></span>
|<span data-ttu-id="c63ce-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c63ce-109">Member</span></span>|<span data-ttu-id="c63ce-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c63ce-110">Value</span></span>|<span data-ttu-id="c63ce-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c63ce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c63ce-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c63ce-112">deviceDefault</span></span>|<span data-ttu-id="c63ce-113">,0</span><span class="sxs-lookup"><span data-stu-id="c63ce-113">0</span></span>|<span data-ttu-id="c63ce-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="c63ce-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="c63ce-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="c63ce-115">lowSecurityBiometric</span></span>|<span data-ttu-id="c63ce-116">1</span><span class="sxs-lookup"><span data-stu-id="c63ce-116">1</span></span>|<span data-ttu-id="c63ce-117">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="c63ce-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="c63ce-118">obrigatório</span><span class="sxs-lookup"><span data-stu-id="c63ce-118">required</span></span>|<span data-ttu-id="c63ce-119">duas</span><span class="sxs-lookup"><span data-stu-id="c63ce-119">2</span></span>|<span data-ttu-id="c63ce-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c63ce-120">Required.</span></span>|
|<span data-ttu-id="c63ce-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="c63ce-121">atLeastNumeric</span></span>|<span data-ttu-id="c63ce-122">3D</span><span class="sxs-lookup"><span data-stu-id="c63ce-122">3</span></span>|<span data-ttu-id="c63ce-123">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="c63ce-123">At least numeric password required.</span></span>|
|<span data-ttu-id="c63ce-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="c63ce-124">numericComplex</span></span>|<span data-ttu-id="c63ce-125">4 </span><span class="sxs-lookup"><span data-stu-id="c63ce-125">4</span></span>|<span data-ttu-id="c63ce-126">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="c63ce-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="c63ce-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="c63ce-127">atLeastAlphabetic</span></span>|<span data-ttu-id="c63ce-128">5 </span><span class="sxs-lookup"><span data-stu-id="c63ce-128">5</span></span>|<span data-ttu-id="c63ce-129">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="c63ce-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="c63ce-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="c63ce-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="c63ce-131">6 </span><span class="sxs-lookup"><span data-stu-id="c63ce-131">6</span></span>|<span data-ttu-id="c63ce-132">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="c63ce-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="c63ce-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="c63ce-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="c63ce-134">7 </span><span class="sxs-lookup"><span data-stu-id="c63ce-134">7</span></span>|<span data-ttu-id="c63ce-135">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="c63ce-135">At least alphanumeric with symbols password required.</span></span>|



