---
title: tipo de enumeração androidWorkProfileRequiredPasswordType
description: Perfil de trabalho do Android tipo de senha exigido.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1ebbbb51390d5d96afcfe0e2d4805e0ba9a3007
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993771"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="a62f0-103">tipo de enumeração androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a62f0-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="a62f0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a62f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a62f0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a62f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a62f0-106">Perfil de trabalho do Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="a62f0-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="a62f0-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a62f0-107">Members</span></span>
|<span data-ttu-id="a62f0-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a62f0-108">Member</span></span>|<span data-ttu-id="a62f0-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a62f0-109">Value</span></span>|<span data-ttu-id="a62f0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a62f0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a62f0-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a62f0-111">deviceDefault</span></span>|<span data-ttu-id="a62f0-112">,0</span><span class="sxs-lookup"><span data-stu-id="a62f0-112">0</span></span>|<span data-ttu-id="a62f0-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="a62f0-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="a62f0-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="a62f0-114">lowSecurityBiometric</span></span>|<span data-ttu-id="a62f0-115">1</span><span class="sxs-lookup"><span data-stu-id="a62f0-115">1</span></span>|<span data-ttu-id="a62f0-116">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="a62f0-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="a62f0-117">obrigatório</span><span class="sxs-lookup"><span data-stu-id="a62f0-117">required</span></span>|<span data-ttu-id="a62f0-118">duas</span><span class="sxs-lookup"><span data-stu-id="a62f0-118">2</span></span>|<span data-ttu-id="a62f0-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a62f0-119">Required.</span></span>|
|<span data-ttu-id="a62f0-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="a62f0-120">atLeastNumeric</span></span>|<span data-ttu-id="a62f0-121">3D</span><span class="sxs-lookup"><span data-stu-id="a62f0-121">3</span></span>|<span data-ttu-id="a62f0-122">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="a62f0-122">At least numeric password required.</span></span>|
|<span data-ttu-id="a62f0-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="a62f0-123">numericComplex</span></span>|<span data-ttu-id="a62f0-124">quatro</span><span class="sxs-lookup"><span data-stu-id="a62f0-124">4</span></span>|<span data-ttu-id="a62f0-125">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="a62f0-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="a62f0-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="a62f0-126">atLeastAlphabetic</span></span>|<span data-ttu-id="a62f0-127">0,5</span><span class="sxs-lookup"><span data-stu-id="a62f0-127">5</span></span>|<span data-ttu-id="a62f0-128">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="a62f0-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="a62f0-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="a62f0-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="a62f0-130">6</span><span class="sxs-lookup"><span data-stu-id="a62f0-130">6</span></span>|<span data-ttu-id="a62f0-131">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="a62f0-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="a62f0-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="a62f0-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="a62f0-133">178</span><span class="sxs-lookup"><span data-stu-id="a62f0-133">7</span></span>|<span data-ttu-id="a62f0-134">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="a62f0-134">At least alphanumeric with symbols password required.</span></span>|





