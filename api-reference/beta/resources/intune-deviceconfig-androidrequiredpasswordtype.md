---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9112074842e3dc661786acfa6c6c223aa5fe225b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334371"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="f31e2-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f31e2-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="f31e2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f31e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f31e2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f31e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f31e2-106">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="f31e2-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="f31e2-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f31e2-107">Members</span></span>
|<span data-ttu-id="f31e2-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f31e2-108">Member</span></span>|<span data-ttu-id="f31e2-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f31e2-109">Value</span></span>|<span data-ttu-id="f31e2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f31e2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f31e2-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f31e2-111">deviceDefault</span></span>|<span data-ttu-id="f31e2-112">,0</span><span class="sxs-lookup"><span data-stu-id="f31e2-112">0</span></span>|<span data-ttu-id="f31e2-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="f31e2-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="f31e2-114">caracteres</span><span class="sxs-lookup"><span data-stu-id="f31e2-114">alphabetic</span></span>|<span data-ttu-id="f31e2-115">1</span><span class="sxs-lookup"><span data-stu-id="f31e2-115">1</span></span>|<span data-ttu-id="f31e2-116">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="f31e2-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="f31e2-117">tecla</span><span class="sxs-lookup"><span data-stu-id="f31e2-117">alphanumeric</span></span>|<span data-ttu-id="f31e2-118">duas</span><span class="sxs-lookup"><span data-stu-id="f31e2-118">2</span></span>|<span data-ttu-id="f31e2-119">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="f31e2-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="f31e2-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="f31e2-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="f31e2-121">3D</span><span class="sxs-lookup"><span data-stu-id="f31e2-121">3</span></span>|<span data-ttu-id="f31e2-122">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="f31e2-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="f31e2-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="f31e2-123">lowSecurityBiometric</span></span>|<span data-ttu-id="f31e2-124">quatro</span><span class="sxs-lookup"><span data-stu-id="f31e2-124">4</span></span>|<span data-ttu-id="f31e2-125">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="f31e2-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="f31e2-126">numéricos</span><span class="sxs-lookup"><span data-stu-id="f31e2-126">numeric</span></span>|<span data-ttu-id="f31e2-127">0,5</span><span class="sxs-lookup"><span data-stu-id="f31e2-127">5</span></span>|<span data-ttu-id="f31e2-128">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="f31e2-128">Numeric password required.</span></span>|
|<span data-ttu-id="f31e2-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="f31e2-129">numericComplex</span></span>|<span data-ttu-id="f31e2-130">6</span><span class="sxs-lookup"><span data-stu-id="f31e2-130">6</span></span>|<span data-ttu-id="f31e2-131">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="f31e2-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="f31e2-132">qualquer</span><span class="sxs-lookup"><span data-stu-id="f31e2-132">any</span></span>|<span data-ttu-id="f31e2-133">178</span><span class="sxs-lookup"><span data-stu-id="f31e2-133">7</span></span>|<span data-ttu-id="f31e2-134">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="f31e2-134">A password or pattern is required, and any is acceptable.</span></span>|



