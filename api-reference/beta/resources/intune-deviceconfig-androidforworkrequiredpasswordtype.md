---
title: tipo de enumeração androidForWorkRequiredPasswordType
description: Android para o tipo de senha de trabalho necessário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 20c7e330d060346557717e9eea0924b275c60d04
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968490"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="1bc02-103">tipo de enumeração androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1bc02-103">androidForWorkRequiredPasswordType enum type</span></span>

<span data-ttu-id="1bc02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bc02-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bc02-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1bc02-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bc02-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1bc02-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bc02-107">Android para o tipo de senha de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="1bc02-107">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="1bc02-108">Membros</span><span class="sxs-lookup"><span data-stu-id="1bc02-108">Members</span></span>
|<span data-ttu-id="1bc02-109">Membro</span><span class="sxs-lookup"><span data-stu-id="1bc02-109">Member</span></span>|<span data-ttu-id="1bc02-110">Valor</span><span class="sxs-lookup"><span data-stu-id="1bc02-110">Value</span></span>|<span data-ttu-id="1bc02-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bc02-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bc02-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1bc02-112">deviceDefault</span></span>|<span data-ttu-id="1bc02-113">,0</span><span class="sxs-lookup"><span data-stu-id="1bc02-113">0</span></span>|<span data-ttu-id="1bc02-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="1bc02-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="1bc02-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="1bc02-115">lowSecurityBiometric</span></span>|<span data-ttu-id="1bc02-116">1 </span><span class="sxs-lookup"><span data-stu-id="1bc02-116">1</span></span>|<span data-ttu-id="1bc02-117">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="1bc02-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="1bc02-118">obrigatório</span><span class="sxs-lookup"><span data-stu-id="1bc02-118">required</span></span>|<span data-ttu-id="1bc02-119">2 </span><span class="sxs-lookup"><span data-stu-id="1bc02-119">2</span></span>|<span data-ttu-id="1bc02-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bc02-120">Required.</span></span>|
|<span data-ttu-id="1bc02-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="1bc02-121">atLeastNumeric</span></span>|<span data-ttu-id="1bc02-122">3 </span><span class="sxs-lookup"><span data-stu-id="1bc02-122">3</span></span>|<span data-ttu-id="1bc02-123">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="1bc02-123">At least numeric password required.</span></span>|
|<span data-ttu-id="1bc02-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="1bc02-124">numericComplex</span></span>|<span data-ttu-id="1bc02-125">4 </span><span class="sxs-lookup"><span data-stu-id="1bc02-125">4</span></span>|<span data-ttu-id="1bc02-126">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="1bc02-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="1bc02-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="1bc02-127">atLeastAlphabetic</span></span>|<span data-ttu-id="1bc02-128">5 </span><span class="sxs-lookup"><span data-stu-id="1bc02-128">5</span></span>|<span data-ttu-id="1bc02-129">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="1bc02-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="1bc02-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="1bc02-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="1bc02-131">6 </span><span class="sxs-lookup"><span data-stu-id="1bc02-131">6</span></span>|<span data-ttu-id="1bc02-132">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="1bc02-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="1bc02-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="1bc02-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="1bc02-134">7 </span><span class="sxs-lookup"><span data-stu-id="1bc02-134">7</span></span>|<span data-ttu-id="1bc02-135">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="1bc02-135">At least alphanumeric with symbols password required.</span></span>|






