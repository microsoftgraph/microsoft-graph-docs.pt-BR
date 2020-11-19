---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5842974b164361f834041e741554045428a7b95a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49231651"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="606ae-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="606ae-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="606ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="606ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="606ae-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="606ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="606ae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="606ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="606ae-107">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="606ae-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="606ae-108">Membros</span><span class="sxs-lookup"><span data-stu-id="606ae-108">Members</span></span>
|<span data-ttu-id="606ae-109">Membro</span><span class="sxs-lookup"><span data-stu-id="606ae-109">Member</span></span>|<span data-ttu-id="606ae-110">Valor</span><span class="sxs-lookup"><span data-stu-id="606ae-110">Value</span></span>|<span data-ttu-id="606ae-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="606ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="606ae-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="606ae-112">deviceDefault</span></span>|<span data-ttu-id="606ae-113">,0</span><span class="sxs-lookup"><span data-stu-id="606ae-113">0</span></span>|<span data-ttu-id="606ae-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="606ae-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="606ae-115">caracteres</span><span class="sxs-lookup"><span data-stu-id="606ae-115">alphabetic</span></span>|<span data-ttu-id="606ae-116">1</span><span class="sxs-lookup"><span data-stu-id="606ae-116">1</span></span>|<span data-ttu-id="606ae-117">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="606ae-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="606ae-118">tecla</span><span class="sxs-lookup"><span data-stu-id="606ae-118">alphanumeric</span></span>|<span data-ttu-id="606ae-119">duas</span><span class="sxs-lookup"><span data-stu-id="606ae-119">2</span></span>|<span data-ttu-id="606ae-120">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="606ae-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="606ae-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="606ae-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="606ae-122">3D</span><span class="sxs-lookup"><span data-stu-id="606ae-122">3</span></span>|<span data-ttu-id="606ae-123">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="606ae-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="606ae-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="606ae-124">lowSecurityBiometric</span></span>|<span data-ttu-id="606ae-125">4 </span><span class="sxs-lookup"><span data-stu-id="606ae-125">4</span></span>|<span data-ttu-id="606ae-126">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="606ae-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="606ae-127">numéricos</span><span class="sxs-lookup"><span data-stu-id="606ae-127">numeric</span></span>|<span data-ttu-id="606ae-128">5 </span><span class="sxs-lookup"><span data-stu-id="606ae-128">5</span></span>|<span data-ttu-id="606ae-129">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="606ae-129">Numeric password required.</span></span>|
|<span data-ttu-id="606ae-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="606ae-130">numericComplex</span></span>|<span data-ttu-id="606ae-131">6 </span><span class="sxs-lookup"><span data-stu-id="606ae-131">6</span></span>|<span data-ttu-id="606ae-132">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="606ae-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="606ae-133">qualquer</span><span class="sxs-lookup"><span data-stu-id="606ae-133">any</span></span>|<span data-ttu-id="606ae-134">7 </span><span class="sxs-lookup"><span data-stu-id="606ae-134">7</span></span>|<span data-ttu-id="606ae-135">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="606ae-135">A password or pattern is required, and any is acceptable.</span></span>|




