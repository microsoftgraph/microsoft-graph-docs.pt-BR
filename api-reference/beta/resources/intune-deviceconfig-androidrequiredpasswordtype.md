---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d70ac87a0e8e3e8d97705b46f5d6ec63d85fbcac
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782069"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="27995-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="27995-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="27995-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="27995-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27995-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27995-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27995-106">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="27995-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="27995-107">Membros</span><span class="sxs-lookup"><span data-stu-id="27995-107">Members</span></span>
|<span data-ttu-id="27995-108">Membro</span><span class="sxs-lookup"><span data-stu-id="27995-108">Member</span></span>|<span data-ttu-id="27995-109">Valor</span><span class="sxs-lookup"><span data-stu-id="27995-109">Value</span></span>|<span data-ttu-id="27995-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="27995-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27995-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="27995-111">deviceDefault</span></span>|<span data-ttu-id="27995-112">,0</span><span class="sxs-lookup"><span data-stu-id="27995-112">0</span></span>|<span data-ttu-id="27995-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="27995-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="27995-114">caracteres</span><span class="sxs-lookup"><span data-stu-id="27995-114">alphabetic</span></span>|<span data-ttu-id="27995-115">1</span><span class="sxs-lookup"><span data-stu-id="27995-115">1</span></span>|<span data-ttu-id="27995-116">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="27995-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="27995-117">tecla</span><span class="sxs-lookup"><span data-stu-id="27995-117">alphanumeric</span></span>|<span data-ttu-id="27995-118">duas</span><span class="sxs-lookup"><span data-stu-id="27995-118">2</span></span>|<span data-ttu-id="27995-119">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="27995-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="27995-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="27995-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="27995-121">3D</span><span class="sxs-lookup"><span data-stu-id="27995-121">3</span></span>|<span data-ttu-id="27995-122">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="27995-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="27995-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="27995-123">lowSecurityBiometric</span></span>|<span data-ttu-id="27995-124">quatro</span><span class="sxs-lookup"><span data-stu-id="27995-124">4</span></span>|<span data-ttu-id="27995-125">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="27995-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="27995-126">numéricos</span><span class="sxs-lookup"><span data-stu-id="27995-126">numeric</span></span>|<span data-ttu-id="27995-127">0,5</span><span class="sxs-lookup"><span data-stu-id="27995-127">5</span></span>|<span data-ttu-id="27995-128">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="27995-128">Numeric password required.</span></span>|
|<span data-ttu-id="27995-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="27995-129">numericComplex</span></span>|<span data-ttu-id="27995-130">6</span><span class="sxs-lookup"><span data-stu-id="27995-130">6</span></span>|<span data-ttu-id="27995-131">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="27995-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="27995-132">qualquer</span><span class="sxs-lookup"><span data-stu-id="27995-132">any</span></span>|<span data-ttu-id="27995-133">178</span><span class="sxs-lookup"><span data-stu-id="27995-133">7</span></span>|<span data-ttu-id="27995-134">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="27995-134">A password or pattern is required, and any is acceptable.</span></span>|





