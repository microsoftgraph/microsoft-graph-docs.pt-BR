---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e20e93543ca681ebd9d900aeaac43731a3d4fa2d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444383"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="e23b1-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e23b1-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="e23b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e23b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e23b1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e23b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e23b1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e23b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e23b1-107">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="e23b1-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="e23b1-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e23b1-108">Members</span></span>
|<span data-ttu-id="e23b1-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e23b1-109">Member</span></span>|<span data-ttu-id="e23b1-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e23b1-110">Value</span></span>|<span data-ttu-id="e23b1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e23b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e23b1-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="e23b1-112">deviceDefault</span></span>|<span data-ttu-id="e23b1-113">,0</span><span class="sxs-lookup"><span data-stu-id="e23b1-113">0</span></span>|<span data-ttu-id="e23b1-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="e23b1-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="e23b1-115">caracteres</span><span class="sxs-lookup"><span data-stu-id="e23b1-115">alphabetic</span></span>|<span data-ttu-id="e23b1-116">1</span><span class="sxs-lookup"><span data-stu-id="e23b1-116">1</span></span>|<span data-ttu-id="e23b1-117">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="e23b1-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="e23b1-118">tecla</span><span class="sxs-lookup"><span data-stu-id="e23b1-118">alphanumeric</span></span>|<span data-ttu-id="e23b1-119">duas</span><span class="sxs-lookup"><span data-stu-id="e23b1-119">2</span></span>|<span data-ttu-id="e23b1-120">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="e23b1-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="e23b1-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="e23b1-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="e23b1-122">3D</span><span class="sxs-lookup"><span data-stu-id="e23b1-122">3</span></span>|<span data-ttu-id="e23b1-123">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="e23b1-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="e23b1-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="e23b1-124">lowSecurityBiometric</span></span>|<span data-ttu-id="e23b1-125">4 </span><span class="sxs-lookup"><span data-stu-id="e23b1-125">4</span></span>|<span data-ttu-id="e23b1-126">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="e23b1-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="e23b1-127">numéricos</span><span class="sxs-lookup"><span data-stu-id="e23b1-127">numeric</span></span>|<span data-ttu-id="e23b1-128">5 </span><span class="sxs-lookup"><span data-stu-id="e23b1-128">5</span></span>|<span data-ttu-id="e23b1-129">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="e23b1-129">Numeric password required.</span></span>|
|<span data-ttu-id="e23b1-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="e23b1-130">numericComplex</span></span>|<span data-ttu-id="e23b1-131">6 </span><span class="sxs-lookup"><span data-stu-id="e23b1-131">6</span></span>|<span data-ttu-id="e23b1-132">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="e23b1-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="e23b1-133">qualquer</span><span class="sxs-lookup"><span data-stu-id="e23b1-133">any</span></span>|<span data-ttu-id="e23b1-134">7 </span><span class="sxs-lookup"><span data-stu-id="e23b1-134">7</span></span>|<span data-ttu-id="e23b1-135">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="e23b1-135">A password or pattern is required, and any is acceptable.</span></span>|



