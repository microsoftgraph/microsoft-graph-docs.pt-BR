---
title: tipo de enumeração androidDeviceOwnerRequiredPasswordType
description: Política de proprietário do dispositivo Android tipo de senha exigido.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fda5f4ee9e8565180100ca96b227727b20efa2eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42486364"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="d80a0-103">tipo de enumeração androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d80a0-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

<span data-ttu-id="d80a0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d80a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d80a0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d80a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d80a0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d80a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d80a0-107">Política de proprietário do dispositivo Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="d80a0-107">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="d80a0-108">Membros</span><span class="sxs-lookup"><span data-stu-id="d80a0-108">Members</span></span>
|<span data-ttu-id="d80a0-109">Membro</span><span class="sxs-lookup"><span data-stu-id="d80a0-109">Member</span></span>|<span data-ttu-id="d80a0-110">Valor</span><span class="sxs-lookup"><span data-stu-id="d80a0-110">Value</span></span>|<span data-ttu-id="d80a0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d80a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d80a0-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d80a0-112">deviceDefault</span></span>|<span data-ttu-id="d80a0-113">,0</span><span class="sxs-lookup"><span data-stu-id="d80a0-113">0</span></span>|<span data-ttu-id="d80a0-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="d80a0-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="d80a0-115">obrigatório</span><span class="sxs-lookup"><span data-stu-id="d80a0-115">required</span></span>|<span data-ttu-id="d80a0-116">1 </span><span class="sxs-lookup"><span data-stu-id="d80a0-116">1</span></span>|<span data-ttu-id="d80a0-117">Deve haver uma senha definida, mas não há restrições no tipo.</span><span class="sxs-lookup"><span data-stu-id="d80a0-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="d80a0-118">numéricos</span><span class="sxs-lookup"><span data-stu-id="d80a0-118">numeric</span></span>|<span data-ttu-id="d80a0-119">2 </span><span class="sxs-lookup"><span data-stu-id="d80a0-119">2</span></span>|<span data-ttu-id="d80a0-120">Pelo menos numérico.</span><span class="sxs-lookup"><span data-stu-id="d80a0-120">At least numeric.</span></span>|
|<span data-ttu-id="d80a0-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="d80a0-121">numericComplex</span></span>|<span data-ttu-id="d80a0-122">3 </span><span class="sxs-lookup"><span data-stu-id="d80a0-122">3</span></span>|<span data-ttu-id="d80a0-123">Pelo menos numérico sem sequências de repetição ou ordenadas.</span><span class="sxs-lookup"><span data-stu-id="d80a0-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="d80a0-124">caracteres</span><span class="sxs-lookup"><span data-stu-id="d80a0-124">alphabetic</span></span>|<span data-ttu-id="d80a0-125">4 </span><span class="sxs-lookup"><span data-stu-id="d80a0-125">4</span></span>|<span data-ttu-id="d80a0-126">Pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="d80a0-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="d80a0-127">tecla</span><span class="sxs-lookup"><span data-stu-id="d80a0-127">alphanumeric</span></span>|<span data-ttu-id="d80a0-128">5 </span><span class="sxs-lookup"><span data-stu-id="d80a0-128">5</span></span>|<span data-ttu-id="d80a0-129">Pelo menos a senha alfanumérica</span><span class="sxs-lookup"><span data-stu-id="d80a0-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="d80a0-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="d80a0-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="d80a0-131">6 </span><span class="sxs-lookup"><span data-stu-id="d80a0-131">6</span></span>|<span data-ttu-id="d80a0-132">Pelo menos alfanumérico com símbolos.</span><span class="sxs-lookup"><span data-stu-id="d80a0-132">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="d80a0-133">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="d80a0-133">lowSecurityBiometric</span></span>|<span data-ttu-id="d80a0-134">7 </span><span class="sxs-lookup"><span data-stu-id="d80a0-134">7</span></span>|<span data-ttu-id="d80a0-135">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="d80a0-135">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="d80a0-136">customPassword</span><span class="sxs-lookup"><span data-stu-id="d80a0-136">customPassword</span></span>|<span data-ttu-id="d80a0-137">8 </span><span class="sxs-lookup"><span data-stu-id="d80a0-137">8</span></span>|<span data-ttu-id="d80a0-138">Senha personalizada definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d80a0-138">Custom password set by the admin.</span></span>|



