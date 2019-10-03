---
title: tipo de enumeração androidWorkProfileRequiredPasswordType
description: Perfil de trabalho do Android tipo de senha exigido.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5cb75fca742f1be0d4e5e00b8ba7e46da3aed954
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366780"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="af28b-103">tipo de enumeração androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="af28b-103">androidWorkProfileRequiredPasswordType enum type</span></span>

> <span data-ttu-id="af28b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="af28b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af28b-105">Perfil de trabalho do Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="af28b-105">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="af28b-106">Membros</span><span class="sxs-lookup"><span data-stu-id="af28b-106">Members</span></span>
|<span data-ttu-id="af28b-107">Membro</span><span class="sxs-lookup"><span data-stu-id="af28b-107">Member</span></span>|<span data-ttu-id="af28b-108">Valor</span><span class="sxs-lookup"><span data-stu-id="af28b-108">Value</span></span>|<span data-ttu-id="af28b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="af28b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af28b-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="af28b-110">deviceDefault</span></span>|<span data-ttu-id="af28b-111">,0</span><span class="sxs-lookup"><span data-stu-id="af28b-111">0</span></span>|<span data-ttu-id="af28b-112">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="af28b-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="af28b-113">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="af28b-113">lowSecurityBiometric</span></span>|<span data-ttu-id="af28b-114">1</span><span class="sxs-lookup"><span data-stu-id="af28b-114">1</span></span>|<span data-ttu-id="af28b-115">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="af28b-115">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="af28b-116">obrigatório</span><span class="sxs-lookup"><span data-stu-id="af28b-116">required</span></span>|<span data-ttu-id="af28b-117">duas</span><span class="sxs-lookup"><span data-stu-id="af28b-117">2</span></span>|<span data-ttu-id="af28b-118">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af28b-118">Required.</span></span>|
|<span data-ttu-id="af28b-119">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="af28b-119">atLeastNumeric</span></span>|<span data-ttu-id="af28b-120">3D</span><span class="sxs-lookup"><span data-stu-id="af28b-120">3</span></span>|<span data-ttu-id="af28b-121">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="af28b-121">At least numeric password required.</span></span>|
|<span data-ttu-id="af28b-122">numericComplex</span><span class="sxs-lookup"><span data-stu-id="af28b-122">numericComplex</span></span>|<span data-ttu-id="af28b-123">quatro</span><span class="sxs-lookup"><span data-stu-id="af28b-123">4</span></span>|<span data-ttu-id="af28b-124">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="af28b-124">Numeric complex password required.</span></span>|
|<span data-ttu-id="af28b-125">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="af28b-125">atLeastAlphabetic</span></span>|<span data-ttu-id="af28b-126">0,5</span><span class="sxs-lookup"><span data-stu-id="af28b-126">5</span></span>|<span data-ttu-id="af28b-127">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="af28b-127">At least alphabetic password required.</span></span>|
|<span data-ttu-id="af28b-128">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="af28b-128">atLeastAlphanumeric</span></span>|<span data-ttu-id="af28b-129">6</span><span class="sxs-lookup"><span data-stu-id="af28b-129">6</span></span>|<span data-ttu-id="af28b-130">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="af28b-130">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="af28b-131">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="af28b-131">alphanumericWithSymbols</span></span>|<span data-ttu-id="af28b-132">178</span><span class="sxs-lookup"><span data-stu-id="af28b-132">7</span></span>|<span data-ttu-id="af28b-133">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="af28b-133">At least alphanumeric with symbols password required.</span></span>|




