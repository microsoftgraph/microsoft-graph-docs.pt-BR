---
title: tipo de enumeração androidWorkProfileRequiredPasswordType
description: Perfil de trabalho do Android tipo de senha exigido.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 742ffaff4c235f9abfeb44d707a3af4429fc86e6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169185"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="ff779-103">tipo de enumeração androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ff779-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="ff779-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff779-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff779-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff779-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff779-106">Perfil de trabalho do Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="ff779-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="ff779-107">Membros</span><span class="sxs-lookup"><span data-stu-id="ff779-107">Members</span></span>
|<span data-ttu-id="ff779-108">Membro</span><span class="sxs-lookup"><span data-stu-id="ff779-108">Member</span></span>|<span data-ttu-id="ff779-109">Valor</span><span class="sxs-lookup"><span data-stu-id="ff779-109">Value</span></span>|<span data-ttu-id="ff779-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff779-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff779-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ff779-111">deviceDefault</span></span>|<span data-ttu-id="ff779-112">,0</span><span class="sxs-lookup"><span data-stu-id="ff779-112">0</span></span>|<span data-ttu-id="ff779-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="ff779-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="ff779-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="ff779-114">lowSecurityBiometric</span></span>|<span data-ttu-id="ff779-115">1</span><span class="sxs-lookup"><span data-stu-id="ff779-115">1</span></span>|<span data-ttu-id="ff779-116">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="ff779-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="ff779-117">obrigatório</span><span class="sxs-lookup"><span data-stu-id="ff779-117">required</span></span>|<span data-ttu-id="ff779-118">duas</span><span class="sxs-lookup"><span data-stu-id="ff779-118">2</span></span>|<span data-ttu-id="ff779-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff779-119">Required.</span></span>|
|<span data-ttu-id="ff779-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="ff779-120">atLeastNumeric</span></span>|<span data-ttu-id="ff779-121">3D</span><span class="sxs-lookup"><span data-stu-id="ff779-121">3</span></span>|<span data-ttu-id="ff779-122">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="ff779-122">At least numeric password required.</span></span>|
|<span data-ttu-id="ff779-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="ff779-123">numericComplex</span></span>|<span data-ttu-id="ff779-124">quatro</span><span class="sxs-lookup"><span data-stu-id="ff779-124">4</span></span>|<span data-ttu-id="ff779-125">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="ff779-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="ff779-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="ff779-126">atLeastAlphabetic</span></span>|<span data-ttu-id="ff779-127">0,5</span><span class="sxs-lookup"><span data-stu-id="ff779-127">5</span></span>|<span data-ttu-id="ff779-128">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="ff779-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="ff779-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="ff779-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="ff779-130">6</span><span class="sxs-lookup"><span data-stu-id="ff779-130">6</span></span>|<span data-ttu-id="ff779-131">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="ff779-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="ff779-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="ff779-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="ff779-133">178</span><span class="sxs-lookup"><span data-stu-id="ff779-133">7</span></span>|<span data-ttu-id="ff779-134">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="ff779-134">At least alphanumeric with symbols password required.</span></span>|




