---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f2377942f5a8dd0a57b0822a1cb9973005e6f321
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011719"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="c63ff-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c63ff-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="c63ff-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c63ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c63ff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c63ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c63ff-106">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="c63ff-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="c63ff-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c63ff-107">Members</span></span>
|<span data-ttu-id="c63ff-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c63ff-108">Member</span></span>|<span data-ttu-id="c63ff-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c63ff-109">Value</span></span>|<span data-ttu-id="c63ff-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c63ff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c63ff-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c63ff-111">deviceDefault</span></span>|<span data-ttu-id="c63ff-112">,0</span><span class="sxs-lookup"><span data-stu-id="c63ff-112">0</span></span>|<span data-ttu-id="c63ff-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="c63ff-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="c63ff-114">caracteres</span><span class="sxs-lookup"><span data-stu-id="c63ff-114">alphabetic</span></span>|<span data-ttu-id="c63ff-115">1</span><span class="sxs-lookup"><span data-stu-id="c63ff-115">1</span></span>|<span data-ttu-id="c63ff-116">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="c63ff-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="c63ff-117">tecla</span><span class="sxs-lookup"><span data-stu-id="c63ff-117">alphanumeric</span></span>|<span data-ttu-id="c63ff-118">duas</span><span class="sxs-lookup"><span data-stu-id="c63ff-118">2</span></span>|<span data-ttu-id="c63ff-119">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="c63ff-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="c63ff-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="c63ff-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="c63ff-121">3D</span><span class="sxs-lookup"><span data-stu-id="c63ff-121">3</span></span>|<span data-ttu-id="c63ff-122">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="c63ff-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="c63ff-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="c63ff-123">lowSecurityBiometric</span></span>|<span data-ttu-id="c63ff-124">quatro</span><span class="sxs-lookup"><span data-stu-id="c63ff-124">4</span></span>|<span data-ttu-id="c63ff-125">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="c63ff-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="c63ff-126">numéricos</span><span class="sxs-lookup"><span data-stu-id="c63ff-126">numeric</span></span>|<span data-ttu-id="c63ff-127">0,5</span><span class="sxs-lookup"><span data-stu-id="c63ff-127">5</span></span>|<span data-ttu-id="c63ff-128">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="c63ff-128">Numeric password required.</span></span>|
|<span data-ttu-id="c63ff-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="c63ff-129">numericComplex</span></span>|<span data-ttu-id="c63ff-130">6</span><span class="sxs-lookup"><span data-stu-id="c63ff-130">6</span></span>|<span data-ttu-id="c63ff-131">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="c63ff-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="c63ff-132">qualquer</span><span class="sxs-lookup"><span data-stu-id="c63ff-132">any</span></span>|<span data-ttu-id="c63ff-133">178</span><span class="sxs-lookup"><span data-stu-id="c63ff-133">7</span></span>|<span data-ttu-id="c63ff-134">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="c63ff-134">A password or pattern is required, and any is acceptable.</span></span>|





