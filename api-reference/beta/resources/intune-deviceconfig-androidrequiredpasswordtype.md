---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1845656d43ec2a8f567506ed61b5ee3bc6d8a9ad
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151517"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="34ba6-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="34ba6-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="34ba6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34ba6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34ba6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34ba6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34ba6-106">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="34ba6-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="34ba6-107">Membros</span><span class="sxs-lookup"><span data-stu-id="34ba6-107">Members</span></span>
|<span data-ttu-id="34ba6-108">Membro</span><span class="sxs-lookup"><span data-stu-id="34ba6-108">Member</span></span>|<span data-ttu-id="34ba6-109">Valor</span><span class="sxs-lookup"><span data-stu-id="34ba6-109">Value</span></span>|<span data-ttu-id="34ba6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="34ba6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34ba6-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="34ba6-111">deviceDefault</span></span>|<span data-ttu-id="34ba6-112">,0</span><span class="sxs-lookup"><span data-stu-id="34ba6-112">0</span></span>|<span data-ttu-id="34ba6-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="34ba6-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="34ba6-114">caracteres</span><span class="sxs-lookup"><span data-stu-id="34ba6-114">alphabetic</span></span>|<span data-ttu-id="34ba6-115">1</span><span class="sxs-lookup"><span data-stu-id="34ba6-115">1</span></span>|<span data-ttu-id="34ba6-116">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="34ba6-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="34ba6-117">tecla</span><span class="sxs-lookup"><span data-stu-id="34ba6-117">alphanumeric</span></span>|<span data-ttu-id="34ba6-118">duas</span><span class="sxs-lookup"><span data-stu-id="34ba6-118">2</span></span>|<span data-ttu-id="34ba6-119">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="34ba6-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="34ba6-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="34ba6-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="34ba6-121">3D</span><span class="sxs-lookup"><span data-stu-id="34ba6-121">3</span></span>|<span data-ttu-id="34ba6-122">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="34ba6-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="34ba6-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="34ba6-123">lowSecurityBiometric</span></span>|<span data-ttu-id="34ba6-124">quatro</span><span class="sxs-lookup"><span data-stu-id="34ba6-124">4</span></span>|<span data-ttu-id="34ba6-125">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="34ba6-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="34ba6-126">numéricos</span><span class="sxs-lookup"><span data-stu-id="34ba6-126">numeric</span></span>|<span data-ttu-id="34ba6-127">0,5</span><span class="sxs-lookup"><span data-stu-id="34ba6-127">5</span></span>|<span data-ttu-id="34ba6-128">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="34ba6-128">Numeric password required.</span></span>|
|<span data-ttu-id="34ba6-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="34ba6-129">numericComplex</span></span>|<span data-ttu-id="34ba6-130">6</span><span class="sxs-lookup"><span data-stu-id="34ba6-130">6</span></span>|<span data-ttu-id="34ba6-131">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="34ba6-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="34ba6-132">qualquer</span><span class="sxs-lookup"><span data-stu-id="34ba6-132">any</span></span>|<span data-ttu-id="34ba6-133">178</span><span class="sxs-lookup"><span data-stu-id="34ba6-133">7</span></span>|<span data-ttu-id="34ba6-134">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="34ba6-134">A password or pattern is required, and any is acceptable.</span></span>|




