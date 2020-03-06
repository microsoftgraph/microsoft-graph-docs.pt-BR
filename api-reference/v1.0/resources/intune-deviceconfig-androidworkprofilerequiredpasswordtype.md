---
title: tipo de enumeração androidWorkProfileRequiredPasswordType
description: Perfil de trabalho do Android tipo de senha exigido.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 24065e97b08b408193f4a3108db5e51fa6f1d28a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530940"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="9a68f-103">tipo de enumeração androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9a68f-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="9a68f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a68f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a68f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a68f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a68f-106">Perfil de trabalho do Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="9a68f-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="9a68f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="9a68f-107">Members</span></span>
|<span data-ttu-id="9a68f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="9a68f-108">Member</span></span>|<span data-ttu-id="9a68f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="9a68f-109">Value</span></span>|<span data-ttu-id="9a68f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a68f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a68f-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9a68f-111">deviceDefault</span></span>|<span data-ttu-id="9a68f-112">,0</span><span class="sxs-lookup"><span data-stu-id="9a68f-112">0</span></span>|<span data-ttu-id="9a68f-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="9a68f-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="9a68f-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="9a68f-114">lowSecurityBiometric</span></span>|<span data-ttu-id="9a68f-115">1 </span><span class="sxs-lookup"><span data-stu-id="9a68f-115">1</span></span>|<span data-ttu-id="9a68f-116">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="9a68f-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="9a68f-117">obrigatório</span><span class="sxs-lookup"><span data-stu-id="9a68f-117">required</span></span>|<span data-ttu-id="9a68f-118">2 </span><span class="sxs-lookup"><span data-stu-id="9a68f-118">2</span></span>|<span data-ttu-id="9a68f-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a68f-119">Required.</span></span>|
|<span data-ttu-id="9a68f-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="9a68f-120">atLeastNumeric</span></span>|<span data-ttu-id="9a68f-121">3 </span><span class="sxs-lookup"><span data-stu-id="9a68f-121">3</span></span>|<span data-ttu-id="9a68f-122">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="9a68f-122">At least numeric password required.</span></span>|
|<span data-ttu-id="9a68f-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="9a68f-123">numericComplex</span></span>|<span data-ttu-id="9a68f-124">4 </span><span class="sxs-lookup"><span data-stu-id="9a68f-124">4</span></span>|<span data-ttu-id="9a68f-125">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="9a68f-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="9a68f-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="9a68f-126">atLeastAlphabetic</span></span>|<span data-ttu-id="9a68f-127">5 </span><span class="sxs-lookup"><span data-stu-id="9a68f-127">5</span></span>|<span data-ttu-id="9a68f-128">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="9a68f-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="9a68f-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="9a68f-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="9a68f-130">6 </span><span class="sxs-lookup"><span data-stu-id="9a68f-130">6</span></span>|<span data-ttu-id="9a68f-131">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="9a68f-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="9a68f-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="9a68f-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="9a68f-133">7 </span><span class="sxs-lookup"><span data-stu-id="9a68f-133">7</span></span>|<span data-ttu-id="9a68f-134">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="9a68f-134">At least alphanumeric with symbols password required.</span></span>|




