---
title: tipo de enumeração androidWorkProfileRequiredPasswordType
description: Perfil de trabalho do Android tipo de senha exigido.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5553329c8519aa40eb4f1ee3ee3cb48f66c06995
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011635"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="89d65-103">tipo de enumeração androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="89d65-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="89d65-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="89d65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89d65-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89d65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89d65-106">Perfil de trabalho do Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="89d65-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="89d65-107">Membros</span><span class="sxs-lookup"><span data-stu-id="89d65-107">Members</span></span>
|<span data-ttu-id="89d65-108">Membro</span><span class="sxs-lookup"><span data-stu-id="89d65-108">Member</span></span>|<span data-ttu-id="89d65-109">Valor</span><span class="sxs-lookup"><span data-stu-id="89d65-109">Value</span></span>|<span data-ttu-id="89d65-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="89d65-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89d65-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="89d65-111">deviceDefault</span></span>|<span data-ttu-id="89d65-112">,0</span><span class="sxs-lookup"><span data-stu-id="89d65-112">0</span></span>|<span data-ttu-id="89d65-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="89d65-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="89d65-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="89d65-114">lowSecurityBiometric</span></span>|<span data-ttu-id="89d65-115">1</span><span class="sxs-lookup"><span data-stu-id="89d65-115">1</span></span>|<span data-ttu-id="89d65-116">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="89d65-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="89d65-117">obrigatório</span><span class="sxs-lookup"><span data-stu-id="89d65-117">required</span></span>|<span data-ttu-id="89d65-118">duas</span><span class="sxs-lookup"><span data-stu-id="89d65-118">2</span></span>|<span data-ttu-id="89d65-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89d65-119">Required.</span></span>|
|<span data-ttu-id="89d65-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="89d65-120">atLeastNumeric</span></span>|<span data-ttu-id="89d65-121">3D</span><span class="sxs-lookup"><span data-stu-id="89d65-121">3</span></span>|<span data-ttu-id="89d65-122">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="89d65-122">At least numeric password required.</span></span>|
|<span data-ttu-id="89d65-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="89d65-123">numericComplex</span></span>|<span data-ttu-id="89d65-124">quatro</span><span class="sxs-lookup"><span data-stu-id="89d65-124">4</span></span>|<span data-ttu-id="89d65-125">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="89d65-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="89d65-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="89d65-126">atLeastAlphabetic</span></span>|<span data-ttu-id="89d65-127">0,5</span><span class="sxs-lookup"><span data-stu-id="89d65-127">5</span></span>|<span data-ttu-id="89d65-128">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="89d65-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="89d65-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="89d65-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="89d65-130">6</span><span class="sxs-lookup"><span data-stu-id="89d65-130">6</span></span>|<span data-ttu-id="89d65-131">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="89d65-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="89d65-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="89d65-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="89d65-133">178</span><span class="sxs-lookup"><span data-stu-id="89d65-133">7</span></span>|<span data-ttu-id="89d65-134">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="89d65-134">At least alphanumeric with symbols password required.</span></span>|





