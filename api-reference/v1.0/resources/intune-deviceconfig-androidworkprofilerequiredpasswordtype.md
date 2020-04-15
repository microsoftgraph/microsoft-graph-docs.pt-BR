---
title: tipo de enumeração androidWorkProfileRequiredPasswordType
description: Perfil de trabalho do Android tipo de senha exigido.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e84439dbd7125d02a5413b46bca1e4e79e13089c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449243"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="02461-103">tipo de enumeração androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="02461-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="02461-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02461-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02461-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02461-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02461-106">Perfil de trabalho do Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="02461-106">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="02461-107">Membros</span><span class="sxs-lookup"><span data-stu-id="02461-107">Members</span></span>
|<span data-ttu-id="02461-108">Membro</span><span class="sxs-lookup"><span data-stu-id="02461-108">Member</span></span>|<span data-ttu-id="02461-109">Valor</span><span class="sxs-lookup"><span data-stu-id="02461-109">Value</span></span>|<span data-ttu-id="02461-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="02461-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02461-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="02461-111">deviceDefault</span></span>|<span data-ttu-id="02461-112">,0</span><span class="sxs-lookup"><span data-stu-id="02461-112">0</span></span>|<span data-ttu-id="02461-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="02461-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="02461-114">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="02461-114">lowSecurityBiometric</span></span>|<span data-ttu-id="02461-115">1</span><span class="sxs-lookup"><span data-stu-id="02461-115">1</span></span>|<span data-ttu-id="02461-116">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="02461-116">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="02461-117">obrigatório</span><span class="sxs-lookup"><span data-stu-id="02461-117">required</span></span>|<span data-ttu-id="02461-118">duas</span><span class="sxs-lookup"><span data-stu-id="02461-118">2</span></span>|<span data-ttu-id="02461-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02461-119">Required.</span></span>|
|<span data-ttu-id="02461-120">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="02461-120">atLeastNumeric</span></span>|<span data-ttu-id="02461-121">3D</span><span class="sxs-lookup"><span data-stu-id="02461-121">3</span></span>|<span data-ttu-id="02461-122">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="02461-122">At least numeric password required.</span></span>|
|<span data-ttu-id="02461-123">numericComplex</span><span class="sxs-lookup"><span data-stu-id="02461-123">numericComplex</span></span>|<span data-ttu-id="02461-124">4 </span><span class="sxs-lookup"><span data-stu-id="02461-124">4</span></span>|<span data-ttu-id="02461-125">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="02461-125">Numeric complex password required.</span></span>|
|<span data-ttu-id="02461-126">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="02461-126">atLeastAlphabetic</span></span>|<span data-ttu-id="02461-127">5 </span><span class="sxs-lookup"><span data-stu-id="02461-127">5</span></span>|<span data-ttu-id="02461-128">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="02461-128">At least alphabetic password required.</span></span>|
|<span data-ttu-id="02461-129">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="02461-129">atLeastAlphanumeric</span></span>|<span data-ttu-id="02461-130">6 </span><span class="sxs-lookup"><span data-stu-id="02461-130">6</span></span>|<span data-ttu-id="02461-131">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="02461-131">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="02461-132">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="02461-132">alphanumericWithSymbols</span></span>|<span data-ttu-id="02461-133">7 </span><span class="sxs-lookup"><span data-stu-id="02461-133">7</span></span>|<span data-ttu-id="02461-134">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="02461-134">At least alphanumeric with symbols password required.</span></span>|







