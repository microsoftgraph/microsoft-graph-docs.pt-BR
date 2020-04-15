---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1baa25eeac9745b41a9b2fc356ff98f3991ad8f2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449349"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="1f688-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1f688-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="1f688-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f688-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f688-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1f688-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f688-106">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="1f688-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="1f688-107">Membros</span><span class="sxs-lookup"><span data-stu-id="1f688-107">Members</span></span>
|<span data-ttu-id="1f688-108">Membro</span><span class="sxs-lookup"><span data-stu-id="1f688-108">Member</span></span>|<span data-ttu-id="1f688-109">Valor</span><span class="sxs-lookup"><span data-stu-id="1f688-109">Value</span></span>|<span data-ttu-id="1f688-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f688-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f688-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1f688-111">deviceDefault</span></span>|<span data-ttu-id="1f688-112">,0</span><span class="sxs-lookup"><span data-stu-id="1f688-112">0</span></span>|<span data-ttu-id="1f688-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="1f688-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="1f688-114">caracteres</span><span class="sxs-lookup"><span data-stu-id="1f688-114">alphabetic</span></span>|<span data-ttu-id="1f688-115">1</span><span class="sxs-lookup"><span data-stu-id="1f688-115">1</span></span>|<span data-ttu-id="1f688-116">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="1f688-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="1f688-117">tecla</span><span class="sxs-lookup"><span data-stu-id="1f688-117">alphanumeric</span></span>|<span data-ttu-id="1f688-118">duas</span><span class="sxs-lookup"><span data-stu-id="1f688-118">2</span></span>|<span data-ttu-id="1f688-119">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="1f688-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="1f688-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="1f688-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="1f688-121">3D</span><span class="sxs-lookup"><span data-stu-id="1f688-121">3</span></span>|<span data-ttu-id="1f688-122">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="1f688-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="1f688-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="1f688-123">lowSecurityBiometric</span></span>|<span data-ttu-id="1f688-124">4 </span><span class="sxs-lookup"><span data-stu-id="1f688-124">4</span></span>|<span data-ttu-id="1f688-125">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="1f688-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="1f688-126">numéricos</span><span class="sxs-lookup"><span data-stu-id="1f688-126">numeric</span></span>|<span data-ttu-id="1f688-127">5 </span><span class="sxs-lookup"><span data-stu-id="1f688-127">5</span></span>|<span data-ttu-id="1f688-128">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="1f688-128">Numeric password required.</span></span>|
|<span data-ttu-id="1f688-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="1f688-129">numericComplex</span></span>|<span data-ttu-id="1f688-130">6 </span><span class="sxs-lookup"><span data-stu-id="1f688-130">6</span></span>|<span data-ttu-id="1f688-131">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="1f688-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="1f688-132">qualquer</span><span class="sxs-lookup"><span data-stu-id="1f688-132">any</span></span>|<span data-ttu-id="1f688-133">7 </span><span class="sxs-lookup"><span data-stu-id="1f688-133">7</span></span>|<span data-ttu-id="1f688-134">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="1f688-134">A password or pattern is required, and any is acceptable.</span></span>|







