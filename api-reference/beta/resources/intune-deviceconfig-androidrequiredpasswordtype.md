---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d70ac87a0e8e3e8d97705b46f5d6ec63d85fbcac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562493"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="a1c90-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a1c90-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="a1c90-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1c90-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1c90-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1c90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1c90-106">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="a1c90-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="a1c90-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a1c90-107">Members</span></span>
|<span data-ttu-id="a1c90-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a1c90-108">Member</span></span>|<span data-ttu-id="a1c90-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a1c90-109">Value</span></span>|<span data-ttu-id="a1c90-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1c90-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1c90-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a1c90-111">deviceDefault</span></span>|<span data-ttu-id="a1c90-112">,0</span><span class="sxs-lookup"><span data-stu-id="a1c90-112">0</span></span>|<span data-ttu-id="a1c90-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="a1c90-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="a1c90-114">caracteres</span><span class="sxs-lookup"><span data-stu-id="a1c90-114">alphabetic</span></span>|<span data-ttu-id="a1c90-115">1 </span><span class="sxs-lookup"><span data-stu-id="a1c90-115">1</span></span>|<span data-ttu-id="a1c90-116">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="a1c90-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="a1c90-117">tecla</span><span class="sxs-lookup"><span data-stu-id="a1c90-117">alphanumeric</span></span>|<span data-ttu-id="a1c90-118">2 </span><span class="sxs-lookup"><span data-stu-id="a1c90-118">2</span></span>|<span data-ttu-id="a1c90-119">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="a1c90-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="a1c90-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="a1c90-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="a1c90-121">3 </span><span class="sxs-lookup"><span data-stu-id="a1c90-121">3</span></span>|<span data-ttu-id="a1c90-122">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="a1c90-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="a1c90-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="a1c90-123">lowSecurityBiometric</span></span>|<span data-ttu-id="a1c90-124">4 </span><span class="sxs-lookup"><span data-stu-id="a1c90-124">4</span></span>|<span data-ttu-id="a1c90-125">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="a1c90-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="a1c90-126">numéricos</span><span class="sxs-lookup"><span data-stu-id="a1c90-126">numeric</span></span>|<span data-ttu-id="a1c90-127">5 </span><span class="sxs-lookup"><span data-stu-id="a1c90-127">5</span></span>|<span data-ttu-id="a1c90-128">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="a1c90-128">Numeric password required.</span></span>|
|<span data-ttu-id="a1c90-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="a1c90-129">numericComplex</span></span>|<span data-ttu-id="a1c90-130">6 </span><span class="sxs-lookup"><span data-stu-id="a1c90-130">6</span></span>|<span data-ttu-id="a1c90-131">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="a1c90-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="a1c90-132">qualquer</span><span class="sxs-lookup"><span data-stu-id="a1c90-132">any</span></span>|<span data-ttu-id="a1c90-133">7 </span><span class="sxs-lookup"><span data-stu-id="a1c90-133">7</span></span>|<span data-ttu-id="a1c90-134">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="a1c90-134">A password or pattern is required, and any is acceptable.</span></span>|





