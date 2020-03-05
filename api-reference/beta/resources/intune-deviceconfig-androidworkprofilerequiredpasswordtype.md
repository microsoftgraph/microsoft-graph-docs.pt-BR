---
title: tipo de enumeração androidWorkProfileRequiredPasswordType
description: Perfil de trabalho do Android tipo de senha exigido.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 865f867510df85b3f784930558bad948c26d5d61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527195"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="84bb3-103">tipo de enumeração androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="84bb3-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="84bb3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="84bb3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84bb3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84bb3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84bb3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84bb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84bb3-107">Perfil de trabalho do Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="84bb3-107">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="84bb3-108">Membros</span><span class="sxs-lookup"><span data-stu-id="84bb3-108">Members</span></span>
|<span data-ttu-id="84bb3-109">Membro</span><span class="sxs-lookup"><span data-stu-id="84bb3-109">Member</span></span>|<span data-ttu-id="84bb3-110">Valor</span><span class="sxs-lookup"><span data-stu-id="84bb3-110">Value</span></span>|<span data-ttu-id="84bb3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="84bb3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84bb3-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="84bb3-112">deviceDefault</span></span>|<span data-ttu-id="84bb3-113">,0</span><span class="sxs-lookup"><span data-stu-id="84bb3-113">0</span></span>|<span data-ttu-id="84bb3-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="84bb3-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="84bb3-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="84bb3-115">lowSecurityBiometric</span></span>|<span data-ttu-id="84bb3-116">1 </span><span class="sxs-lookup"><span data-stu-id="84bb3-116">1</span></span>|<span data-ttu-id="84bb3-117">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="84bb3-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="84bb3-118">obrigatório</span><span class="sxs-lookup"><span data-stu-id="84bb3-118">required</span></span>|<span data-ttu-id="84bb3-119">2 </span><span class="sxs-lookup"><span data-stu-id="84bb3-119">2</span></span>|<span data-ttu-id="84bb3-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84bb3-120">Required.</span></span>|
|<span data-ttu-id="84bb3-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="84bb3-121">atLeastNumeric</span></span>|<span data-ttu-id="84bb3-122">3 </span><span class="sxs-lookup"><span data-stu-id="84bb3-122">3</span></span>|<span data-ttu-id="84bb3-123">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="84bb3-123">At least numeric password required.</span></span>|
|<span data-ttu-id="84bb3-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="84bb3-124">numericComplex</span></span>|<span data-ttu-id="84bb3-125">4 </span><span class="sxs-lookup"><span data-stu-id="84bb3-125">4</span></span>|<span data-ttu-id="84bb3-126">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="84bb3-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="84bb3-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="84bb3-127">atLeastAlphabetic</span></span>|<span data-ttu-id="84bb3-128">5 </span><span class="sxs-lookup"><span data-stu-id="84bb3-128">5</span></span>|<span data-ttu-id="84bb3-129">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="84bb3-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="84bb3-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="84bb3-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="84bb3-131">6 </span><span class="sxs-lookup"><span data-stu-id="84bb3-131">6</span></span>|<span data-ttu-id="84bb3-132">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="84bb3-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="84bb3-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="84bb3-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="84bb3-134">7 </span><span class="sxs-lookup"><span data-stu-id="84bb3-134">7</span></span>|<span data-ttu-id="84bb3-135">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="84bb3-135">At least alphanumeric with symbols password required.</span></span>|



