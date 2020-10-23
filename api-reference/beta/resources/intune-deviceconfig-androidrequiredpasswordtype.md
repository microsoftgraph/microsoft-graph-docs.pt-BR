---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f78829f47a8f1d029ed78b2fb0d63192af69a3e6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725600"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="7c6dc-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7c6dc-103">androidRequiredPasswordType enum type</span></span>

<span data-ttu-id="7c6dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c6dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c6dc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c6dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c6dc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c6dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c6dc-107">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="7c6dc-107">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="7c6dc-108">Membros</span><span class="sxs-lookup"><span data-stu-id="7c6dc-108">Members</span></span>
|<span data-ttu-id="7c6dc-109">Membro</span><span class="sxs-lookup"><span data-stu-id="7c6dc-109">Member</span></span>|<span data-ttu-id="7c6dc-110">Valor</span><span class="sxs-lookup"><span data-stu-id="7c6dc-110">Value</span></span>|<span data-ttu-id="7c6dc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c6dc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c6dc-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="7c6dc-112">deviceDefault</span></span>|<span data-ttu-id="7c6dc-113">,0</span><span class="sxs-lookup"><span data-stu-id="7c6dc-113">0</span></span>|<span data-ttu-id="7c6dc-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="7c6dc-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="7c6dc-115">caracteres</span><span class="sxs-lookup"><span data-stu-id="7c6dc-115">alphabetic</span></span>|<span data-ttu-id="7c6dc-116">1</span><span class="sxs-lookup"><span data-stu-id="7c6dc-116">1</span></span>|<span data-ttu-id="7c6dc-117">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="7c6dc-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="7c6dc-118">tecla</span><span class="sxs-lookup"><span data-stu-id="7c6dc-118">alphanumeric</span></span>|<span data-ttu-id="7c6dc-119">duas</span><span class="sxs-lookup"><span data-stu-id="7c6dc-119">2</span></span>|<span data-ttu-id="7c6dc-120">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="7c6dc-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="7c6dc-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="7c6dc-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="7c6dc-122">3D</span><span class="sxs-lookup"><span data-stu-id="7c6dc-122">3</span></span>|<span data-ttu-id="7c6dc-123">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="7c6dc-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="7c6dc-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="7c6dc-124">lowSecurityBiometric</span></span>|<span data-ttu-id="7c6dc-125">4 </span><span class="sxs-lookup"><span data-stu-id="7c6dc-125">4</span></span>|<span data-ttu-id="7c6dc-126">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="7c6dc-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="7c6dc-127">numéricos</span><span class="sxs-lookup"><span data-stu-id="7c6dc-127">numeric</span></span>|<span data-ttu-id="7c6dc-128">5 </span><span class="sxs-lookup"><span data-stu-id="7c6dc-128">5</span></span>|<span data-ttu-id="7c6dc-129">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="7c6dc-129">Numeric password required.</span></span>|
|<span data-ttu-id="7c6dc-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="7c6dc-130">numericComplex</span></span>|<span data-ttu-id="7c6dc-131">6 </span><span class="sxs-lookup"><span data-stu-id="7c6dc-131">6</span></span>|<span data-ttu-id="7c6dc-132">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="7c6dc-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="7c6dc-133">qualquer</span><span class="sxs-lookup"><span data-stu-id="7c6dc-133">any</span></span>|<span data-ttu-id="7c6dc-134">7 </span><span class="sxs-lookup"><span data-stu-id="7c6dc-134">7</span></span>|<span data-ttu-id="7c6dc-135">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="7c6dc-135">A password or pattern is required, and any is acceptable.</span></span>|





