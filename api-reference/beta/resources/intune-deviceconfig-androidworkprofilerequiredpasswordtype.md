---
title: tipo de enumeração androidWorkProfileRequiredPasswordType
description: Perfil de trabalho do Android tipo de senha exigido.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 822c2021040b0dc4e6eb827e9fec54a40b5cad64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062082"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="e47f9-103">tipo de enumeração androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e47f9-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="e47f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e47f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e47f9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e47f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e47f9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e47f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e47f9-107">Perfil de trabalho do Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="e47f9-107">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="e47f9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e47f9-108">Members</span></span>
|<span data-ttu-id="e47f9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e47f9-109">Member</span></span>|<span data-ttu-id="e47f9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e47f9-110">Value</span></span>|<span data-ttu-id="e47f9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e47f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e47f9-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="e47f9-112">deviceDefault</span></span>|<span data-ttu-id="e47f9-113">,0</span><span class="sxs-lookup"><span data-stu-id="e47f9-113">0</span></span>|<span data-ttu-id="e47f9-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="e47f9-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="e47f9-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="e47f9-115">lowSecurityBiometric</span></span>|<span data-ttu-id="e47f9-116">1 </span><span class="sxs-lookup"><span data-stu-id="e47f9-116">1</span></span>|<span data-ttu-id="e47f9-117">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="e47f9-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="e47f9-118">obrigatório</span><span class="sxs-lookup"><span data-stu-id="e47f9-118">required</span></span>|<span data-ttu-id="e47f9-119">2 </span><span class="sxs-lookup"><span data-stu-id="e47f9-119">2</span></span>|<span data-ttu-id="e47f9-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e47f9-120">Required.</span></span>|
|<span data-ttu-id="e47f9-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="e47f9-121">atLeastNumeric</span></span>|<span data-ttu-id="e47f9-122">3 </span><span class="sxs-lookup"><span data-stu-id="e47f9-122">3</span></span>|<span data-ttu-id="e47f9-123">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="e47f9-123">At least numeric password required.</span></span>|
|<span data-ttu-id="e47f9-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="e47f9-124">numericComplex</span></span>|<span data-ttu-id="e47f9-125">4 </span><span class="sxs-lookup"><span data-stu-id="e47f9-125">4</span></span>|<span data-ttu-id="e47f9-126">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="e47f9-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="e47f9-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="e47f9-127">atLeastAlphabetic</span></span>|<span data-ttu-id="e47f9-128">5 </span><span class="sxs-lookup"><span data-stu-id="e47f9-128">5</span></span>|<span data-ttu-id="e47f9-129">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="e47f9-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="e47f9-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="e47f9-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="e47f9-131">6 </span><span class="sxs-lookup"><span data-stu-id="e47f9-131">6</span></span>|<span data-ttu-id="e47f9-132">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="e47f9-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="e47f9-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="e47f9-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="e47f9-134">7 </span><span class="sxs-lookup"><span data-stu-id="e47f9-134">7</span></span>|<span data-ttu-id="e47f9-135">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="e47f9-135">At least alphanumeric with symbols password required.</span></span>|






