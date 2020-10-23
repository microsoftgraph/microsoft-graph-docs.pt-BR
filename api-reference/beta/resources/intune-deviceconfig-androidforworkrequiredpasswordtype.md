---
title: tipo de enumeração androidForWorkRequiredPasswordType
description: Android para o tipo de senha de trabalho necessário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 249a5081e63bd94885bdee059ae1521e03c52e71
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724625"
---
# <a name="androidforworkrequiredpasswordtype-enum-type"></a><span data-ttu-id="a062c-103">tipo de enumeração androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a062c-103">androidForWorkRequiredPasswordType enum type</span></span>

<span data-ttu-id="a062c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a062c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a062c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a062c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a062c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a062c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a062c-107">Android para o tipo de senha de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="a062c-107">Android For Work required password type.</span></span>

## <a name="members"></a><span data-ttu-id="a062c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a062c-108">Members</span></span>
|<span data-ttu-id="a062c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a062c-109">Member</span></span>|<span data-ttu-id="a062c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a062c-110">Value</span></span>|<span data-ttu-id="a062c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a062c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a062c-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a062c-112">deviceDefault</span></span>|<span data-ttu-id="a062c-113">,0</span><span class="sxs-lookup"><span data-stu-id="a062c-113">0</span></span>|<span data-ttu-id="a062c-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="a062c-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="a062c-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="a062c-115">lowSecurityBiometric</span></span>|<span data-ttu-id="a062c-116">1</span><span class="sxs-lookup"><span data-stu-id="a062c-116">1</span></span>|<span data-ttu-id="a062c-117">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="a062c-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="a062c-118">obrigatório</span><span class="sxs-lookup"><span data-stu-id="a062c-118">required</span></span>|<span data-ttu-id="a062c-119">duas</span><span class="sxs-lookup"><span data-stu-id="a062c-119">2</span></span>|<span data-ttu-id="a062c-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a062c-120">Required.</span></span>|
|<span data-ttu-id="a062c-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="a062c-121">atLeastNumeric</span></span>|<span data-ttu-id="a062c-122">3D</span><span class="sxs-lookup"><span data-stu-id="a062c-122">3</span></span>|<span data-ttu-id="a062c-123">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="a062c-123">At least numeric password required.</span></span>|
|<span data-ttu-id="a062c-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="a062c-124">numericComplex</span></span>|<span data-ttu-id="a062c-125">4 </span><span class="sxs-lookup"><span data-stu-id="a062c-125">4</span></span>|<span data-ttu-id="a062c-126">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="a062c-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="a062c-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="a062c-127">atLeastAlphabetic</span></span>|<span data-ttu-id="a062c-128">5 </span><span class="sxs-lookup"><span data-stu-id="a062c-128">5</span></span>|<span data-ttu-id="a062c-129">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="a062c-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="a062c-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="a062c-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="a062c-131">6 </span><span class="sxs-lookup"><span data-stu-id="a062c-131">6</span></span>|<span data-ttu-id="a062c-132">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="a062c-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="a062c-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="a062c-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="a062c-134">7 </span><span class="sxs-lookup"><span data-stu-id="a062c-134">7</span></span>|<span data-ttu-id="a062c-135">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="a062c-135">At least alphanumeric with symbols password required.</span></span>|





