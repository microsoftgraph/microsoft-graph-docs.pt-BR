---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2cfbf31bc2c263031e2e850e4caf479abb325ec
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988932"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="18b4b-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="18b4b-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="18b4b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="18b4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18b4b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18b4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18b4b-106">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="18b4b-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="18b4b-107">Membros</span><span class="sxs-lookup"><span data-stu-id="18b4b-107">Members</span></span>
|<span data-ttu-id="18b4b-108">Membro</span><span class="sxs-lookup"><span data-stu-id="18b4b-108">Member</span></span>|<span data-ttu-id="18b4b-109">Valor</span><span class="sxs-lookup"><span data-stu-id="18b4b-109">Value</span></span>|<span data-ttu-id="18b4b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="18b4b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18b4b-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="18b4b-111">deviceDefault</span></span>|<span data-ttu-id="18b4b-112">,0</span><span class="sxs-lookup"><span data-stu-id="18b4b-112">0</span></span>|<span data-ttu-id="18b4b-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="18b4b-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="18b4b-114">caracteres</span><span class="sxs-lookup"><span data-stu-id="18b4b-114">alphabetic</span></span>|<span data-ttu-id="18b4b-115">1</span><span class="sxs-lookup"><span data-stu-id="18b4b-115">1</span></span>|<span data-ttu-id="18b4b-116">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="18b4b-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="18b4b-117">tecla</span><span class="sxs-lookup"><span data-stu-id="18b4b-117">alphanumeric</span></span>|<span data-ttu-id="18b4b-118">duas</span><span class="sxs-lookup"><span data-stu-id="18b4b-118">2</span></span>|<span data-ttu-id="18b4b-119">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="18b4b-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="18b4b-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="18b4b-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="18b4b-121">3D</span><span class="sxs-lookup"><span data-stu-id="18b4b-121">3</span></span>|<span data-ttu-id="18b4b-122">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="18b4b-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="18b4b-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="18b4b-123">lowSecurityBiometric</span></span>|<span data-ttu-id="18b4b-124">quatro</span><span class="sxs-lookup"><span data-stu-id="18b4b-124">4</span></span>|<span data-ttu-id="18b4b-125">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="18b4b-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="18b4b-126">numéricos</span><span class="sxs-lookup"><span data-stu-id="18b4b-126">numeric</span></span>|<span data-ttu-id="18b4b-127">0,5</span><span class="sxs-lookup"><span data-stu-id="18b4b-127">5</span></span>|<span data-ttu-id="18b4b-128">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="18b4b-128">Numeric password required.</span></span>|
|<span data-ttu-id="18b4b-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="18b4b-129">numericComplex</span></span>|<span data-ttu-id="18b4b-130">6</span><span class="sxs-lookup"><span data-stu-id="18b4b-130">6</span></span>|<span data-ttu-id="18b4b-131">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="18b4b-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="18b4b-132">qualquer</span><span class="sxs-lookup"><span data-stu-id="18b4b-132">any</span></span>|<span data-ttu-id="18b4b-133">178</span><span class="sxs-lookup"><span data-stu-id="18b4b-133">7</span></span>|<span data-ttu-id="18b4b-134">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="18b4b-134">A password or pattern is required, and any is acceptable.</span></span>|





