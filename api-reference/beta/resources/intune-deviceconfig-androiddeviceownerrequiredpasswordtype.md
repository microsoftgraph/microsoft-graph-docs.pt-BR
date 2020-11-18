---
title: tipo de enumeração androidDeviceOwnerRequiredPasswordType
description: Política de proprietário do dispositivo Android tipo de senha exigido.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b6e36f6bba7cd996e5bf264f91ac3d59d9495759
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199928"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="72654-103">tipo de enumeração androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="72654-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

<span data-ttu-id="72654-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72654-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72654-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="72654-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72654-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72654-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72654-107">Política de proprietário do dispositivo Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="72654-107">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="72654-108">Membros</span><span class="sxs-lookup"><span data-stu-id="72654-108">Members</span></span>
|<span data-ttu-id="72654-109">Membro</span><span class="sxs-lookup"><span data-stu-id="72654-109">Member</span></span>|<span data-ttu-id="72654-110">Valor</span><span class="sxs-lookup"><span data-stu-id="72654-110">Value</span></span>|<span data-ttu-id="72654-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="72654-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72654-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="72654-112">deviceDefault</span></span>|<span data-ttu-id="72654-113">,0</span><span class="sxs-lookup"><span data-stu-id="72654-113">0</span></span>|<span data-ttu-id="72654-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="72654-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="72654-115">obrigatório</span><span class="sxs-lookup"><span data-stu-id="72654-115">required</span></span>|<span data-ttu-id="72654-116">1</span><span class="sxs-lookup"><span data-stu-id="72654-116">1</span></span>|<span data-ttu-id="72654-117">Deve haver uma senha definida, mas não há restrições no tipo.</span><span class="sxs-lookup"><span data-stu-id="72654-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="72654-118">numéricos</span><span class="sxs-lookup"><span data-stu-id="72654-118">numeric</span></span>|<span data-ttu-id="72654-119">duas</span><span class="sxs-lookup"><span data-stu-id="72654-119">2</span></span>|<span data-ttu-id="72654-120">Pelo menos numérico.</span><span class="sxs-lookup"><span data-stu-id="72654-120">At least numeric.</span></span>|
|<span data-ttu-id="72654-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="72654-121">numericComplex</span></span>|<span data-ttu-id="72654-122">3D</span><span class="sxs-lookup"><span data-stu-id="72654-122">3</span></span>|<span data-ttu-id="72654-123">Pelo menos numérico sem sequências de repetição ou ordenadas.</span><span class="sxs-lookup"><span data-stu-id="72654-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="72654-124">caracteres</span><span class="sxs-lookup"><span data-stu-id="72654-124">alphabetic</span></span>|<span data-ttu-id="72654-125">4 </span><span class="sxs-lookup"><span data-stu-id="72654-125">4</span></span>|<span data-ttu-id="72654-126">Pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="72654-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="72654-127">tecla</span><span class="sxs-lookup"><span data-stu-id="72654-127">alphanumeric</span></span>|<span data-ttu-id="72654-128">5 </span><span class="sxs-lookup"><span data-stu-id="72654-128">5</span></span>|<span data-ttu-id="72654-129">Pelo menos a senha alfanumérica</span><span class="sxs-lookup"><span data-stu-id="72654-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="72654-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="72654-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="72654-131">6 </span><span class="sxs-lookup"><span data-stu-id="72654-131">6</span></span>|<span data-ttu-id="72654-132">Pelo menos alfanumérico com símbolos.</span><span class="sxs-lookup"><span data-stu-id="72654-132">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="72654-133">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="72654-133">lowSecurityBiometric</span></span>|<span data-ttu-id="72654-134">7 </span><span class="sxs-lookup"><span data-stu-id="72654-134">7</span></span>|<span data-ttu-id="72654-135">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="72654-135">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="72654-136">customPassword</span><span class="sxs-lookup"><span data-stu-id="72654-136">customPassword</span></span>|<span data-ttu-id="72654-137">8 </span><span class="sxs-lookup"><span data-stu-id="72654-137">8</span></span>|<span data-ttu-id="72654-138">Senha personalizada definida pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="72654-138">Custom password set by the admin.</span></span>|




