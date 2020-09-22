---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3aaf2ad668e87f7f3fee1a8f168845203704a5a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021543"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="6ad1a-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6ad1a-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="6ad1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ad1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ad1a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ad1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ad1a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ad1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ad1a-107">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="6ad1a-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="6ad1a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6ad1a-108">Members</span></span>
|<span data-ttu-id="6ad1a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6ad1a-109">Member</span></span>|<span data-ttu-id="6ad1a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6ad1a-110">Value</span></span>|<span data-ttu-id="6ad1a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ad1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ad1a-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="6ad1a-112">deviceDefault</span></span>|<span data-ttu-id="6ad1a-113">,0</span><span class="sxs-lookup"><span data-stu-id="6ad1a-113">0</span></span>|<span data-ttu-id="6ad1a-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="6ad1a-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="6ad1a-115">caracteres</span><span class="sxs-lookup"><span data-stu-id="6ad1a-115">alphabetic</span></span>|<span data-ttu-id="6ad1a-116">1 </span><span class="sxs-lookup"><span data-stu-id="6ad1a-116">1</span></span>|<span data-ttu-id="6ad1a-117">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="6ad1a-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="6ad1a-118">tecla</span><span class="sxs-lookup"><span data-stu-id="6ad1a-118">alphanumeric</span></span>|<span data-ttu-id="6ad1a-119">2 </span><span class="sxs-lookup"><span data-stu-id="6ad1a-119">2</span></span>|<span data-ttu-id="6ad1a-120">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="6ad1a-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="6ad1a-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="6ad1a-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="6ad1a-122">3 </span><span class="sxs-lookup"><span data-stu-id="6ad1a-122">3</span></span>|<span data-ttu-id="6ad1a-123">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="6ad1a-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="6ad1a-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="6ad1a-124">lowSecurityBiometric</span></span>|<span data-ttu-id="6ad1a-125">4 </span><span class="sxs-lookup"><span data-stu-id="6ad1a-125">4</span></span>|<span data-ttu-id="6ad1a-126">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="6ad1a-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="6ad1a-127">numéricos</span><span class="sxs-lookup"><span data-stu-id="6ad1a-127">numeric</span></span>|<span data-ttu-id="6ad1a-128">5 </span><span class="sxs-lookup"><span data-stu-id="6ad1a-128">5</span></span>|<span data-ttu-id="6ad1a-129">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="6ad1a-129">Numeric password required.</span></span>|
|<span data-ttu-id="6ad1a-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="6ad1a-130">numericComplex</span></span>|<span data-ttu-id="6ad1a-131">6 </span><span class="sxs-lookup"><span data-stu-id="6ad1a-131">6</span></span>|<span data-ttu-id="6ad1a-132">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="6ad1a-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="6ad1a-133">qualquer</span><span class="sxs-lookup"><span data-stu-id="6ad1a-133">any</span></span>|<span data-ttu-id="6ad1a-134">7 </span><span class="sxs-lookup"><span data-stu-id="6ad1a-134">7</span></span>|<span data-ttu-id="6ad1a-135">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="6ad1a-135">A password or pattern is required, and any is acceptable.</span></span>|






