---
title: tipo de enumeração androidDeviceOwnerRequiredPasswordType
description: Política de proprietário do dispositivo Android tipo de senha exigido.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6f37ddeb108db777b23f55abd67963688b9a3d3c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402801"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="66570-103">tipo de enumeração androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="66570-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

<span data-ttu-id="66570-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66570-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66570-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="66570-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66570-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="66570-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66570-107">Política de proprietário do dispositivo Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="66570-107">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="66570-108">Membros</span><span class="sxs-lookup"><span data-stu-id="66570-108">Members</span></span>
|<span data-ttu-id="66570-109">Membro</span><span class="sxs-lookup"><span data-stu-id="66570-109">Member</span></span>|<span data-ttu-id="66570-110">Valor</span><span class="sxs-lookup"><span data-stu-id="66570-110">Value</span></span>|<span data-ttu-id="66570-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="66570-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66570-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="66570-112">deviceDefault</span></span>|<span data-ttu-id="66570-113">,0</span><span class="sxs-lookup"><span data-stu-id="66570-113">0</span></span>|<span data-ttu-id="66570-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="66570-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="66570-115">obrigatório</span><span class="sxs-lookup"><span data-stu-id="66570-115">required</span></span>|<span data-ttu-id="66570-116">1</span><span class="sxs-lookup"><span data-stu-id="66570-116">1</span></span>|<span data-ttu-id="66570-117">Deve haver uma senha definida, mas não há restrições no tipo.</span><span class="sxs-lookup"><span data-stu-id="66570-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="66570-118">numéricos</span><span class="sxs-lookup"><span data-stu-id="66570-118">numeric</span></span>|<span data-ttu-id="66570-119">duas</span><span class="sxs-lookup"><span data-stu-id="66570-119">2</span></span>|<span data-ttu-id="66570-120">Pelo menos numérico.</span><span class="sxs-lookup"><span data-stu-id="66570-120">At least numeric.</span></span>|
|<span data-ttu-id="66570-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="66570-121">numericComplex</span></span>|<span data-ttu-id="66570-122">3D</span><span class="sxs-lookup"><span data-stu-id="66570-122">3</span></span>|<span data-ttu-id="66570-123">Pelo menos numérico sem sequências de repetição ou ordenadas.</span><span class="sxs-lookup"><span data-stu-id="66570-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="66570-124">caracteres</span><span class="sxs-lookup"><span data-stu-id="66570-124">alphabetic</span></span>|<span data-ttu-id="66570-125">4 </span><span class="sxs-lookup"><span data-stu-id="66570-125">4</span></span>|<span data-ttu-id="66570-126">Pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="66570-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="66570-127">tecla</span><span class="sxs-lookup"><span data-stu-id="66570-127">alphanumeric</span></span>|<span data-ttu-id="66570-128">5 </span><span class="sxs-lookup"><span data-stu-id="66570-128">5</span></span>|<span data-ttu-id="66570-129">Pelo menos a senha alfanumérica</span><span class="sxs-lookup"><span data-stu-id="66570-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="66570-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="66570-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="66570-131">6 </span><span class="sxs-lookup"><span data-stu-id="66570-131">6</span></span>|<span data-ttu-id="66570-132">Pelo menos alfanumérico com símbolos.</span><span class="sxs-lookup"><span data-stu-id="66570-132">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="66570-133">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="66570-133">lowSecurityBiometric</span></span>|<span data-ttu-id="66570-134">7 </span><span class="sxs-lookup"><span data-stu-id="66570-134">7</span></span>|<span data-ttu-id="66570-135">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="66570-135">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="66570-136">customPassword</span><span class="sxs-lookup"><span data-stu-id="66570-136">customPassword</span></span>|<span data-ttu-id="66570-137">8 </span><span class="sxs-lookup"><span data-stu-id="66570-137">8</span></span>|<span data-ttu-id="66570-138">Senha personalizada definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="66570-138">Custom password set by the admin.</span></span>|



