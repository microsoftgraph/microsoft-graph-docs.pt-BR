---
title: tipo de enumeração androidDeviceOwnerRequiredPasswordType
description: Política de proprietário do dispositivo Android tipo de senha exigido.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc6d81a71fe01addb6111252b28aee01072fe0dd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949063"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="06e09-103">tipo de enumeração androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="06e09-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="06e09-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06e09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06e09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06e09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06e09-106">Política de proprietário do dispositivo Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="06e09-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="06e09-107">Membros</span><span class="sxs-lookup"><span data-stu-id="06e09-107">Members</span></span>
|<span data-ttu-id="06e09-108">Membro</span><span class="sxs-lookup"><span data-stu-id="06e09-108">Member</span></span>|<span data-ttu-id="06e09-109">Valor</span><span class="sxs-lookup"><span data-stu-id="06e09-109">Value</span></span>|<span data-ttu-id="06e09-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="06e09-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06e09-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="06e09-111">deviceDefault</span></span>|<span data-ttu-id="06e09-112">,0</span><span class="sxs-lookup"><span data-stu-id="06e09-112">0</span></span>|<span data-ttu-id="06e09-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="06e09-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="06e09-114">obrigatório</span><span class="sxs-lookup"><span data-stu-id="06e09-114">required</span></span>|<span data-ttu-id="06e09-115">1</span><span class="sxs-lookup"><span data-stu-id="06e09-115">1</span></span>|<span data-ttu-id="06e09-116">Deve haver uma senha definida, mas não há restrições no tipo.</span><span class="sxs-lookup"><span data-stu-id="06e09-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="06e09-117">numéricos</span><span class="sxs-lookup"><span data-stu-id="06e09-117">numeric</span></span>|<span data-ttu-id="06e09-118">duas</span><span class="sxs-lookup"><span data-stu-id="06e09-118">2</span></span>|<span data-ttu-id="06e09-119">Pelo menos numérico.</span><span class="sxs-lookup"><span data-stu-id="06e09-119">At least numeric.</span></span>|
|<span data-ttu-id="06e09-120">numericComplex</span><span class="sxs-lookup"><span data-stu-id="06e09-120">numericComplex</span></span>|<span data-ttu-id="06e09-121">3D</span><span class="sxs-lookup"><span data-stu-id="06e09-121">3</span></span>|<span data-ttu-id="06e09-122">Pelo menos numérico sem sequências de repetição ou ordenadas.</span><span class="sxs-lookup"><span data-stu-id="06e09-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="06e09-123">caracteres</span><span class="sxs-lookup"><span data-stu-id="06e09-123">alphabetic</span></span>|<span data-ttu-id="06e09-124">quatro</span><span class="sxs-lookup"><span data-stu-id="06e09-124">4</span></span>|<span data-ttu-id="06e09-125">Pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="06e09-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="06e09-126">tecla</span><span class="sxs-lookup"><span data-stu-id="06e09-126">alphanumeric</span></span>|<span data-ttu-id="06e09-127">0,5</span><span class="sxs-lookup"><span data-stu-id="06e09-127">5</span></span>|<span data-ttu-id="06e09-128">Pelo menos a senha alfanumérica</span><span class="sxs-lookup"><span data-stu-id="06e09-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="06e09-129">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="06e09-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="06e09-130">6</span><span class="sxs-lookup"><span data-stu-id="06e09-130">6</span></span>|<span data-ttu-id="06e09-131">Pelo menos alfanumérico com símbolos.</span><span class="sxs-lookup"><span data-stu-id="06e09-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="06e09-132">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="06e09-132">lowSecurityBiometric</span></span>|<span data-ttu-id="06e09-133">178</span><span class="sxs-lookup"><span data-stu-id="06e09-133">7</span></span>|<span data-ttu-id="06e09-134">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="06e09-134">Low security biometrics based password required.</span></span>|




