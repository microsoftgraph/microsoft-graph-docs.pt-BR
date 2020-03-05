---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7d20aee3893d9d74e01fad6858c59d2c524059d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527301"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="c5e7b-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c5e7b-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="c5e7b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c5e7b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5e7b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5e7b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5e7b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5e7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5e7b-107">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="c5e7b-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="c5e7b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c5e7b-108">Members</span></span>
|<span data-ttu-id="c5e7b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c5e7b-109">Member</span></span>|<span data-ttu-id="c5e7b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c5e7b-110">Value</span></span>|<span data-ttu-id="c5e7b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5e7b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5e7b-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c5e7b-112">deviceDefault</span></span>|<span data-ttu-id="c5e7b-113">,0</span><span class="sxs-lookup"><span data-stu-id="c5e7b-113">0</span></span>|<span data-ttu-id="c5e7b-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="c5e7b-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="c5e7b-115">caracteres</span><span class="sxs-lookup"><span data-stu-id="c5e7b-115">alphabetic</span></span>|<span data-ttu-id="c5e7b-116">1 </span><span class="sxs-lookup"><span data-stu-id="c5e7b-116">1</span></span>|<span data-ttu-id="c5e7b-117">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="c5e7b-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="c5e7b-118">tecla</span><span class="sxs-lookup"><span data-stu-id="c5e7b-118">alphanumeric</span></span>|<span data-ttu-id="c5e7b-119">2 </span><span class="sxs-lookup"><span data-stu-id="c5e7b-119">2</span></span>|<span data-ttu-id="c5e7b-120">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="c5e7b-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="c5e7b-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="c5e7b-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="c5e7b-122">3 </span><span class="sxs-lookup"><span data-stu-id="c5e7b-122">3</span></span>|<span data-ttu-id="c5e7b-123">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="c5e7b-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="c5e7b-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="c5e7b-124">lowSecurityBiometric</span></span>|<span data-ttu-id="c5e7b-125">4 </span><span class="sxs-lookup"><span data-stu-id="c5e7b-125">4</span></span>|<span data-ttu-id="c5e7b-126">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="c5e7b-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="c5e7b-127">numéricos</span><span class="sxs-lookup"><span data-stu-id="c5e7b-127">numeric</span></span>|<span data-ttu-id="c5e7b-128">5 </span><span class="sxs-lookup"><span data-stu-id="c5e7b-128">5</span></span>|<span data-ttu-id="c5e7b-129">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="c5e7b-129">Numeric password required.</span></span>|
|<span data-ttu-id="c5e7b-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="c5e7b-130">numericComplex</span></span>|<span data-ttu-id="c5e7b-131">6 </span><span class="sxs-lookup"><span data-stu-id="c5e7b-131">6</span></span>|<span data-ttu-id="c5e7b-132">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="c5e7b-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="c5e7b-133">qualquer</span><span class="sxs-lookup"><span data-stu-id="c5e7b-133">any</span></span>|<span data-ttu-id="c5e7b-134">7 </span><span class="sxs-lookup"><span data-stu-id="c5e7b-134">7</span></span>|<span data-ttu-id="c5e7b-135">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="c5e7b-135">A password or pattern is required, and any is acceptable.</span></span>|



