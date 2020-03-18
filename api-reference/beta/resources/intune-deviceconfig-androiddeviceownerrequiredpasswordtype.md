---
title: tipo de enumeração androidDeviceOwnerRequiredPasswordType
description: Política de proprietário do dispositivo Android tipo de senha exigido.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e6d783f8bdf5faeed2d3e10a9286a897c8d85783
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796983"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="3cb7e-103">tipo de enumeração androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3cb7e-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="3cb7e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3cb7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cb7e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3cb7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cb7e-106">Política de proprietário do dispositivo Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="3cb7e-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="3cb7e-107">Membros</span><span class="sxs-lookup"><span data-stu-id="3cb7e-107">Members</span></span>
|<span data-ttu-id="3cb7e-108">Membro</span><span class="sxs-lookup"><span data-stu-id="3cb7e-108">Member</span></span>|<span data-ttu-id="3cb7e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3cb7e-109">Value</span></span>|<span data-ttu-id="3cb7e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cb7e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cb7e-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3cb7e-111">deviceDefault</span></span>|<span data-ttu-id="3cb7e-112">,0</span><span class="sxs-lookup"><span data-stu-id="3cb7e-112">0</span></span>|<span data-ttu-id="3cb7e-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="3cb7e-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="3cb7e-114">obrigatório</span><span class="sxs-lookup"><span data-stu-id="3cb7e-114">required</span></span>|<span data-ttu-id="3cb7e-115">1</span><span class="sxs-lookup"><span data-stu-id="3cb7e-115">1</span></span>|<span data-ttu-id="3cb7e-116">Deve haver uma senha definida, mas não há restrições no tipo.</span><span class="sxs-lookup"><span data-stu-id="3cb7e-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="3cb7e-117">numéricos</span><span class="sxs-lookup"><span data-stu-id="3cb7e-117">numeric</span></span>|<span data-ttu-id="3cb7e-118">duas</span><span class="sxs-lookup"><span data-stu-id="3cb7e-118">2</span></span>|<span data-ttu-id="3cb7e-119">Pelo menos numérico.</span><span class="sxs-lookup"><span data-stu-id="3cb7e-119">At least numeric.</span></span>|
|<span data-ttu-id="3cb7e-120">numericComplex</span><span class="sxs-lookup"><span data-stu-id="3cb7e-120">numericComplex</span></span>|<span data-ttu-id="3cb7e-121">3D</span><span class="sxs-lookup"><span data-stu-id="3cb7e-121">3</span></span>|<span data-ttu-id="3cb7e-122">Pelo menos numérico sem sequências de repetição ou ordenadas.</span><span class="sxs-lookup"><span data-stu-id="3cb7e-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="3cb7e-123">caracteres</span><span class="sxs-lookup"><span data-stu-id="3cb7e-123">alphabetic</span></span>|<span data-ttu-id="3cb7e-124">4 </span><span class="sxs-lookup"><span data-stu-id="3cb7e-124">4</span></span>|<span data-ttu-id="3cb7e-125">Pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="3cb7e-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="3cb7e-126">tecla</span><span class="sxs-lookup"><span data-stu-id="3cb7e-126">alphanumeric</span></span>|<span data-ttu-id="3cb7e-127">5 </span><span class="sxs-lookup"><span data-stu-id="3cb7e-127">5</span></span>|<span data-ttu-id="3cb7e-128">Pelo menos a senha alfanumérica</span><span class="sxs-lookup"><span data-stu-id="3cb7e-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="3cb7e-129">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="3cb7e-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="3cb7e-130">6 </span><span class="sxs-lookup"><span data-stu-id="3cb7e-130">6</span></span>|<span data-ttu-id="3cb7e-131">Pelo menos alfanumérico com símbolos.</span><span class="sxs-lookup"><span data-stu-id="3cb7e-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="3cb7e-132">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="3cb7e-132">lowSecurityBiometric</span></span>|<span data-ttu-id="3cb7e-133">7 </span><span class="sxs-lookup"><span data-stu-id="3cb7e-133">7</span></span>|<span data-ttu-id="3cb7e-134">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="3cb7e-134">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="3cb7e-135">customPassword</span><span class="sxs-lookup"><span data-stu-id="3cb7e-135">customPassword</span></span>|<span data-ttu-id="3cb7e-136">8 </span><span class="sxs-lookup"><span data-stu-id="3cb7e-136">8</span></span>|<span data-ttu-id="3cb7e-137">Senha personalizada definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3cb7e-137">Custom password set by the admin.</span></span>|



