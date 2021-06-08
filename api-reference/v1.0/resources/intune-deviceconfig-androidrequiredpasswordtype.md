---
title: tipo de número androidRequiredPasswordType
description: Tipo de senha obrigatório do Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d179666a4de9256e98c704bccd9e512d4aebd0ce
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760283"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="58d84-103">tipo de número androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="58d84-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="58d84-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58d84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58d84-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58d84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58d84-106">Tipo de senha obrigatório do Android.</span><span class="sxs-lookup"><span data-stu-id="58d84-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="58d84-107">Membros</span><span class="sxs-lookup"><span data-stu-id="58d84-107">Members</span></span>
|<span data-ttu-id="58d84-108">Membro</span><span class="sxs-lookup"><span data-stu-id="58d84-108">Member</span></span>|<span data-ttu-id="58d84-109">Valor</span><span class="sxs-lookup"><span data-stu-id="58d84-109">Value</span></span>|<span data-ttu-id="58d84-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="58d84-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58d84-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="58d84-111">deviceDefault</span></span>|<span data-ttu-id="58d84-112">0</span><span class="sxs-lookup"><span data-stu-id="58d84-112">0</span></span>|<span data-ttu-id="58d84-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="58d84-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="58d84-114">alfabético</span><span class="sxs-lookup"><span data-stu-id="58d84-114">alphabetic</span></span>|<span data-ttu-id="58d84-115">1</span><span class="sxs-lookup"><span data-stu-id="58d84-115">1</span></span>|<span data-ttu-id="58d84-116">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="58d84-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="58d84-117">alfanumérico</span><span class="sxs-lookup"><span data-stu-id="58d84-117">alphanumeric</span></span>|<span data-ttu-id="58d84-118">2</span><span class="sxs-lookup"><span data-stu-id="58d84-118">2</span></span>|<span data-ttu-id="58d84-119">Senha alfanumérica necessária.</span><span class="sxs-lookup"><span data-stu-id="58d84-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="58d84-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="58d84-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="58d84-121">3</span><span class="sxs-lookup"><span data-stu-id="58d84-121">3</span></span>|<span data-ttu-id="58d84-122">Alfanumérico com símbolos de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="58d84-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="58d84-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="58d84-123">lowSecurityBiometric</span></span>|<span data-ttu-id="58d84-124">4 </span><span class="sxs-lookup"><span data-stu-id="58d84-124">4</span></span>|<span data-ttu-id="58d84-125">Senha de baixa biometria baseada em segurança necessária.</span><span class="sxs-lookup"><span data-stu-id="58d84-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="58d84-126">numeric</span><span class="sxs-lookup"><span data-stu-id="58d84-126">numeric</span></span>|<span data-ttu-id="58d84-127">5 </span><span class="sxs-lookup"><span data-stu-id="58d84-127">5</span></span>|<span data-ttu-id="58d84-128">Senha numérica necessária.</span><span class="sxs-lookup"><span data-stu-id="58d84-128">Numeric password required.</span></span>|
|<span data-ttu-id="58d84-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="58d84-129">numericComplex</span></span>|<span data-ttu-id="58d84-130">6 </span><span class="sxs-lookup"><span data-stu-id="58d84-130">6</span></span>|<span data-ttu-id="58d84-131">Senha complexa numérica necessária.</span><span class="sxs-lookup"><span data-stu-id="58d84-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="58d84-132">qualquer</span><span class="sxs-lookup"><span data-stu-id="58d84-132">any</span></span>|<span data-ttu-id="58d84-133">7 </span><span class="sxs-lookup"><span data-stu-id="58d84-133">7</span></span>|<span data-ttu-id="58d84-134">Uma senha ou padrão é necessária e qualquer uma é aceitável.</span><span class="sxs-lookup"><span data-stu-id="58d84-134">A password or pattern is required, and any is acceptable.</span></span>|




