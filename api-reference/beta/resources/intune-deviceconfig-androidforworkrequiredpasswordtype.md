---
title: tipo de enumeração androidForWorkRequiredPasswordType
description: Android para o tipo de senha de trabalho necessário.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e0e99a5e54797441070308882d4137859390820
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169472"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="3cf03-103">tipo de enumeração androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3cf03-103">androidForWorkRequiredPasswordType enum type</span></span>

> <span data-ttu-id="3cf03-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3cf03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cf03-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3cf03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cf03-106">Android para o tipo de senha de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="3cf03-106">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="3cf03-107">Membros</span><span class="sxs-lookup"><span data-stu-id="3cf03-107">Members</span></span>
|<span data-ttu-id="3cf03-108">Membro</span><span class="sxs-lookup"><span data-stu-id="3cf03-108">Member</span></span>|<span data-ttu-id="3cf03-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3cf03-109">Value</span></span>|<span data-ttu-id="3cf03-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cf03-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cf03-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3cf03-111">deviceDefault</span></span>|<span data-ttu-id="3cf03-112">,0</span><span class="sxs-lookup"><span data-stu-id="3cf03-112">0</span></span>|<span data-ttu-id="3cf03-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="3cf03-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="3cf03-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="3cf03-114">lowSecurityBiometric</span></span>|<span data-ttu-id="3cf03-115">1</span><span class="sxs-lookup"><span data-stu-id="3cf03-115">1</span></span>|<span data-ttu-id="3cf03-116">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="3cf03-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="3cf03-117">obrigatório</span><span class="sxs-lookup"><span data-stu-id="3cf03-117">required</span></span>|<span data-ttu-id="3cf03-118">duas</span><span class="sxs-lookup"><span data-stu-id="3cf03-118">2</span></span>|<span data-ttu-id="3cf03-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cf03-119">Required.</span></span>|
|<span data-ttu-id="3cf03-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="3cf03-120">atLeastNumeric</span></span>|<span data-ttu-id="3cf03-121">3D</span><span class="sxs-lookup"><span data-stu-id="3cf03-121">3</span></span>|<span data-ttu-id="3cf03-122">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="3cf03-122">At least numeric password required.</span></span>|
|<span data-ttu-id="3cf03-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="3cf03-123">numericComplex</span></span>|<span data-ttu-id="3cf03-124">quatro</span><span class="sxs-lookup"><span data-stu-id="3cf03-124">4</span></span>|<span data-ttu-id="3cf03-125">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="3cf03-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="3cf03-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="3cf03-126">atLeastAlphabetic</span></span>|<span data-ttu-id="3cf03-127">0,5</span><span class="sxs-lookup"><span data-stu-id="3cf03-127">5</span></span>|<span data-ttu-id="3cf03-128">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="3cf03-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="3cf03-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="3cf03-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="3cf03-130">6</span><span class="sxs-lookup"><span data-stu-id="3cf03-130">6</span></span>|<span data-ttu-id="3cf03-131">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="3cf03-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="3cf03-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="3cf03-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="3cf03-133">178</span><span class="sxs-lookup"><span data-stu-id="3cf03-133">7</span></span>|<span data-ttu-id="3cf03-134">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="3cf03-134">At least alphanumeric with symbols password required.</span></span>|




