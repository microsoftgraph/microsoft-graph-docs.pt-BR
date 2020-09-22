---
title: tipo de enumeração androidWorkProfileRequiredPasswordType
description: Perfil de trabalho do Android tipo de senha exigido.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4c87a56e6b53654597a41742d835d7de5eaddcc2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051162"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="0dbf5-103">tipo de enumeração androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0dbf5-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="0dbf5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dbf5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0dbf5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0dbf5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dbf5-106">Perfil de trabalho do Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="0dbf5-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="0dbf5-107">Membros</span><span class="sxs-lookup"><span data-stu-id="0dbf5-107">Members</span></span>
|<span data-ttu-id="0dbf5-108">Membro</span><span class="sxs-lookup"><span data-stu-id="0dbf5-108">Member</span></span>|<span data-ttu-id="0dbf5-109">Valor</span><span class="sxs-lookup"><span data-stu-id="0dbf5-109">Value</span></span>|<span data-ttu-id="0dbf5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dbf5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dbf5-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="0dbf5-111">deviceDefault</span></span>|<span data-ttu-id="0dbf5-112">,0</span><span class="sxs-lookup"><span data-stu-id="0dbf5-112">0</span></span>|<span data-ttu-id="0dbf5-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="0dbf5-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="0dbf5-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="0dbf5-114">lowSecurityBiometric</span></span>|<span data-ttu-id="0dbf5-115">1 </span><span class="sxs-lookup"><span data-stu-id="0dbf5-115">1</span></span>|<span data-ttu-id="0dbf5-116">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="0dbf5-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="0dbf5-117">obrigatório</span><span class="sxs-lookup"><span data-stu-id="0dbf5-117">required</span></span>|<span data-ttu-id="0dbf5-118">2 </span><span class="sxs-lookup"><span data-stu-id="0dbf5-118">2</span></span>|<span data-ttu-id="0dbf5-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0dbf5-119">Required.</span></span>|
|<span data-ttu-id="0dbf5-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="0dbf5-120">atLeastNumeric</span></span>|<span data-ttu-id="0dbf5-121">3 </span><span class="sxs-lookup"><span data-stu-id="0dbf5-121">3</span></span>|<span data-ttu-id="0dbf5-122">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="0dbf5-122">At least numeric password required.</span></span>|
|<span data-ttu-id="0dbf5-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="0dbf5-123">numericComplex</span></span>|<span data-ttu-id="0dbf5-124">4 </span><span class="sxs-lookup"><span data-stu-id="0dbf5-124">4</span></span>|<span data-ttu-id="0dbf5-125">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="0dbf5-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="0dbf5-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="0dbf5-126">atLeastAlphabetic</span></span>|<span data-ttu-id="0dbf5-127">5 </span><span class="sxs-lookup"><span data-stu-id="0dbf5-127">5</span></span>|<span data-ttu-id="0dbf5-128">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="0dbf5-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="0dbf5-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="0dbf5-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="0dbf5-130">6 </span><span class="sxs-lookup"><span data-stu-id="0dbf5-130">6</span></span>|<span data-ttu-id="0dbf5-131">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="0dbf5-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="0dbf5-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="0dbf5-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="0dbf5-133">7 </span><span class="sxs-lookup"><span data-stu-id="0dbf5-133">7</span></span>|<span data-ttu-id="0dbf5-134">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="0dbf5-134">At least alphanumeric with symbols password required.</span></span>|









