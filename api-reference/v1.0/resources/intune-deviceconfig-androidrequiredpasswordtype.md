---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4921263e1960617b8d9e013ce12a799e11d61516
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041558"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="3331c-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3331c-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="3331c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3331c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3331c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3331c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3331c-106">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="3331c-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="3331c-107">Membros</span><span class="sxs-lookup"><span data-stu-id="3331c-107">Members</span></span>
|<span data-ttu-id="3331c-108">Membro</span><span class="sxs-lookup"><span data-stu-id="3331c-108">Member</span></span>|<span data-ttu-id="3331c-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3331c-109">Value</span></span>|<span data-ttu-id="3331c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3331c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3331c-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3331c-111">deviceDefault</span></span>|<span data-ttu-id="3331c-112">,0</span><span class="sxs-lookup"><span data-stu-id="3331c-112">0</span></span>|<span data-ttu-id="3331c-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="3331c-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="3331c-114">caracteres</span><span class="sxs-lookup"><span data-stu-id="3331c-114">alphabetic</span></span>|<span data-ttu-id="3331c-115">1 </span><span class="sxs-lookup"><span data-stu-id="3331c-115">1</span></span>|<span data-ttu-id="3331c-116">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="3331c-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="3331c-117">tecla</span><span class="sxs-lookup"><span data-stu-id="3331c-117">alphanumeric</span></span>|<span data-ttu-id="3331c-118">2 </span><span class="sxs-lookup"><span data-stu-id="3331c-118">2</span></span>|<span data-ttu-id="3331c-119">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="3331c-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="3331c-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="3331c-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="3331c-121">3 </span><span class="sxs-lookup"><span data-stu-id="3331c-121">3</span></span>|<span data-ttu-id="3331c-122">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="3331c-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="3331c-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="3331c-123">lowSecurityBiometric</span></span>|<span data-ttu-id="3331c-124">4 </span><span class="sxs-lookup"><span data-stu-id="3331c-124">4</span></span>|<span data-ttu-id="3331c-125">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="3331c-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="3331c-126">numéricos</span><span class="sxs-lookup"><span data-stu-id="3331c-126">numeric</span></span>|<span data-ttu-id="3331c-127">5 </span><span class="sxs-lookup"><span data-stu-id="3331c-127">5</span></span>|<span data-ttu-id="3331c-128">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="3331c-128">Numeric password required.</span></span>|
|<span data-ttu-id="3331c-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="3331c-129">numericComplex</span></span>|<span data-ttu-id="3331c-130">6 </span><span class="sxs-lookup"><span data-stu-id="3331c-130">6</span></span>|<span data-ttu-id="3331c-131">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="3331c-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="3331c-132">qualquer</span><span class="sxs-lookup"><span data-stu-id="3331c-132">any</span></span>|<span data-ttu-id="3331c-133">7 </span><span class="sxs-lookup"><span data-stu-id="3331c-133">7</span></span>|<span data-ttu-id="3331c-134">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="3331c-134">A password or pattern is required, and any is acceptable.</span></span>|









