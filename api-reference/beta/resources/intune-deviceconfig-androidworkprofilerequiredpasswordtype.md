---
title: tipo de enumeração androidWorkProfileRequiredPasswordType
description: Perfil de trabalho do Android tipo de senha exigido.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bbe0e64fdbbca78766bf7471d29d6cdf17b0714
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562353"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="6ffb8-103">tipo de enumeração androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6ffb8-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="6ffb8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ffb8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ffb8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ffb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ffb8-106">Perfil de trabalho do Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="6ffb8-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="6ffb8-107">Membros</span><span class="sxs-lookup"><span data-stu-id="6ffb8-107">Members</span></span>
|<span data-ttu-id="6ffb8-108">Membro</span><span class="sxs-lookup"><span data-stu-id="6ffb8-108">Member</span></span>|<span data-ttu-id="6ffb8-109">Valor</span><span class="sxs-lookup"><span data-stu-id="6ffb8-109">Value</span></span>|<span data-ttu-id="6ffb8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ffb8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ffb8-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="6ffb8-111">deviceDefault</span></span>|<span data-ttu-id="6ffb8-112">,0</span><span class="sxs-lookup"><span data-stu-id="6ffb8-112">0</span></span>|<span data-ttu-id="6ffb8-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="6ffb8-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="6ffb8-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="6ffb8-114">lowSecurityBiometric</span></span>|<span data-ttu-id="6ffb8-115">1 </span><span class="sxs-lookup"><span data-stu-id="6ffb8-115">1</span></span>|<span data-ttu-id="6ffb8-116">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="6ffb8-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="6ffb8-117">obrigatório</span><span class="sxs-lookup"><span data-stu-id="6ffb8-117">required</span></span>|<span data-ttu-id="6ffb8-118">2 </span><span class="sxs-lookup"><span data-stu-id="6ffb8-118">2</span></span>|<span data-ttu-id="6ffb8-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ffb8-119">Required.</span></span>|
|<span data-ttu-id="6ffb8-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="6ffb8-120">atLeastNumeric</span></span>|<span data-ttu-id="6ffb8-121">3 </span><span class="sxs-lookup"><span data-stu-id="6ffb8-121">3</span></span>|<span data-ttu-id="6ffb8-122">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="6ffb8-122">At least numeric password required.</span></span>|
|<span data-ttu-id="6ffb8-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="6ffb8-123">numericComplex</span></span>|<span data-ttu-id="6ffb8-124">4 </span><span class="sxs-lookup"><span data-stu-id="6ffb8-124">4</span></span>|<span data-ttu-id="6ffb8-125">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="6ffb8-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="6ffb8-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="6ffb8-126">atLeastAlphabetic</span></span>|<span data-ttu-id="6ffb8-127">5 </span><span class="sxs-lookup"><span data-stu-id="6ffb8-127">5</span></span>|<span data-ttu-id="6ffb8-128">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="6ffb8-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="6ffb8-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="6ffb8-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="6ffb8-130">6 </span><span class="sxs-lookup"><span data-stu-id="6ffb8-130">6</span></span>|<span data-ttu-id="6ffb8-131">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="6ffb8-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="6ffb8-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="6ffb8-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="6ffb8-133">7 </span><span class="sxs-lookup"><span data-stu-id="6ffb8-133">7</span></span>|<span data-ttu-id="6ffb8-134">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="6ffb8-134">At least alphanumeric with symbols password required.</span></span>|





