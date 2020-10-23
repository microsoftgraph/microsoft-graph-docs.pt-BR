---
title: tipo de enumeração androidWorkProfileRequiredPasswordType
description: Perfil de trabalho do Android tipo de senha exigido.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5e89c96d08fa1c265647692b3edb831fd308b7f7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730676"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="e7f04-103">tipo de enumeração androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e7f04-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="e7f04-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7f04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7f04-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7f04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7f04-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7f04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7f04-107">Perfil de trabalho do Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="e7f04-107">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="e7f04-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e7f04-108">Members</span></span>
|<span data-ttu-id="e7f04-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e7f04-109">Member</span></span>|<span data-ttu-id="e7f04-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e7f04-110">Value</span></span>|<span data-ttu-id="e7f04-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7f04-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7f04-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="e7f04-112">deviceDefault</span></span>|<span data-ttu-id="e7f04-113">,0</span><span class="sxs-lookup"><span data-stu-id="e7f04-113">0</span></span>|<span data-ttu-id="e7f04-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="e7f04-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="e7f04-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="e7f04-115">lowSecurityBiometric</span></span>|<span data-ttu-id="e7f04-116">1</span><span class="sxs-lookup"><span data-stu-id="e7f04-116">1</span></span>|<span data-ttu-id="e7f04-117">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="e7f04-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="e7f04-118">obrigatório</span><span class="sxs-lookup"><span data-stu-id="e7f04-118">required</span></span>|<span data-ttu-id="e7f04-119">duas</span><span class="sxs-lookup"><span data-stu-id="e7f04-119">2</span></span>|<span data-ttu-id="e7f04-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7f04-120">Required.</span></span>|
|<span data-ttu-id="e7f04-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="e7f04-121">atLeastNumeric</span></span>|<span data-ttu-id="e7f04-122">3D</span><span class="sxs-lookup"><span data-stu-id="e7f04-122">3</span></span>|<span data-ttu-id="e7f04-123">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="e7f04-123">At least numeric password required.</span></span>|
|<span data-ttu-id="e7f04-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="e7f04-124">numericComplex</span></span>|<span data-ttu-id="e7f04-125">4 </span><span class="sxs-lookup"><span data-stu-id="e7f04-125">4</span></span>|<span data-ttu-id="e7f04-126">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="e7f04-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="e7f04-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="e7f04-127">atLeastAlphabetic</span></span>|<span data-ttu-id="e7f04-128">5 </span><span class="sxs-lookup"><span data-stu-id="e7f04-128">5</span></span>|<span data-ttu-id="e7f04-129">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="e7f04-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="e7f04-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="e7f04-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="e7f04-131">6 </span><span class="sxs-lookup"><span data-stu-id="e7f04-131">6</span></span>|<span data-ttu-id="e7f04-132">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="e7f04-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="e7f04-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="e7f04-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="e7f04-134">7 </span><span class="sxs-lookup"><span data-stu-id="e7f04-134">7</span></span>|<span data-ttu-id="e7f04-135">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="e7f04-135">At least alphanumeric with symbols password required.</span></span>|





