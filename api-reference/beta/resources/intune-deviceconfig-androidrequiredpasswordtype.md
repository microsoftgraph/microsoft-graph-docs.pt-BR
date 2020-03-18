---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2ceac6e3953615524fb78b14c380218bf5c43f19
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796731"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="10106-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="10106-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="10106-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="10106-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10106-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10106-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10106-106">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="10106-106">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="10106-107">Membros</span><span class="sxs-lookup"><span data-stu-id="10106-107">Members</span></span>
|<span data-ttu-id="10106-108">Membro</span><span class="sxs-lookup"><span data-stu-id="10106-108">Member</span></span>|<span data-ttu-id="10106-109">Valor</span><span class="sxs-lookup"><span data-stu-id="10106-109">Value</span></span>|<span data-ttu-id="10106-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="10106-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10106-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="10106-111">deviceDefault</span></span>|<span data-ttu-id="10106-112">,0</span><span class="sxs-lookup"><span data-stu-id="10106-112">0</span></span>|<span data-ttu-id="10106-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="10106-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="10106-114">caracteres</span><span class="sxs-lookup"><span data-stu-id="10106-114">alphabetic</span></span>|<span data-ttu-id="10106-115">1</span><span class="sxs-lookup"><span data-stu-id="10106-115">1</span></span>|<span data-ttu-id="10106-116">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="10106-116">Alphabetic password required.</span></span>|
|<span data-ttu-id="10106-117">tecla</span><span class="sxs-lookup"><span data-stu-id="10106-117">alphanumeric</span></span>|<span data-ttu-id="10106-118">duas</span><span class="sxs-lookup"><span data-stu-id="10106-118">2</span></span>|<span data-ttu-id="10106-119">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="10106-119">Alphanumeric password required.</span></span>|
|<span data-ttu-id="10106-120">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="10106-120">alphanumericWithSymbols</span></span>|<span data-ttu-id="10106-121">3D</span><span class="sxs-lookup"><span data-stu-id="10106-121">3</span></span>|<span data-ttu-id="10106-122">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="10106-122">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="10106-123">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="10106-123">lowSecurityBiometric</span></span>|<span data-ttu-id="10106-124">4 </span><span class="sxs-lookup"><span data-stu-id="10106-124">4</span></span>|<span data-ttu-id="10106-125">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="10106-125">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="10106-126">numéricos</span><span class="sxs-lookup"><span data-stu-id="10106-126">numeric</span></span>|<span data-ttu-id="10106-127">5 </span><span class="sxs-lookup"><span data-stu-id="10106-127">5</span></span>|<span data-ttu-id="10106-128">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="10106-128">Numeric password required.</span></span>|
|<span data-ttu-id="10106-129">numericComplex</span><span class="sxs-lookup"><span data-stu-id="10106-129">numericComplex</span></span>|<span data-ttu-id="10106-130">6 </span><span class="sxs-lookup"><span data-stu-id="10106-130">6</span></span>|<span data-ttu-id="10106-131">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="10106-131">Numeric complex password required.</span></span>|
|<span data-ttu-id="10106-132">qualquer</span><span class="sxs-lookup"><span data-stu-id="10106-132">any</span></span>|<span data-ttu-id="10106-133">7 </span><span class="sxs-lookup"><span data-stu-id="10106-133">7</span></span>|<span data-ttu-id="10106-134">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="10106-134">A password or pattern is required, and any is acceptable.</span></span>|



