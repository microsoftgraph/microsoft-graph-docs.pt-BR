---
title: tipo de enumeração androidDeviceOwnerRequiredPasswordType
description: Política de proprietário do dispositivo Android tipo de senha exigido.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8c575b1b39592eb8191e358563abb6d6bd834e7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556358"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="6ca0f-103">tipo de enumeração androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6ca0f-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="6ca0f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ca0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ca0f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ca0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ca0f-106">Política de proprietário do dispositivo Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="6ca0f-106">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="6ca0f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="6ca0f-107">Members</span></span>
|<span data-ttu-id="6ca0f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="6ca0f-108">Member</span></span>|<span data-ttu-id="6ca0f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="6ca0f-109">Value</span></span>|<span data-ttu-id="6ca0f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ca0f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ca0f-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="6ca0f-111">deviceDefault</span></span>|<span data-ttu-id="6ca0f-112">,0</span><span class="sxs-lookup"><span data-stu-id="6ca0f-112">0</span></span>|<span data-ttu-id="6ca0f-113">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="6ca0f-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="6ca0f-114">obrigatório</span><span class="sxs-lookup"><span data-stu-id="6ca0f-114">required</span></span>|<span data-ttu-id="6ca0f-115">1 </span><span class="sxs-lookup"><span data-stu-id="6ca0f-115">1</span></span>|<span data-ttu-id="6ca0f-116">Deve haver uma senha definida, mas não há restrições no tipo.</span><span class="sxs-lookup"><span data-stu-id="6ca0f-116">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="6ca0f-117">numéricos</span><span class="sxs-lookup"><span data-stu-id="6ca0f-117">numeric</span></span>|<span data-ttu-id="6ca0f-118">2 </span><span class="sxs-lookup"><span data-stu-id="6ca0f-118">2</span></span>|<span data-ttu-id="6ca0f-119">Pelo menos numérico.</span><span class="sxs-lookup"><span data-stu-id="6ca0f-119">At least numeric.</span></span>|
|<span data-ttu-id="6ca0f-120">numericComplex</span><span class="sxs-lookup"><span data-stu-id="6ca0f-120">numericComplex</span></span>|<span data-ttu-id="6ca0f-121">3 </span><span class="sxs-lookup"><span data-stu-id="6ca0f-121">3</span></span>|<span data-ttu-id="6ca0f-122">Pelo menos numérico sem sequências de repetição ou ordenadas.</span><span class="sxs-lookup"><span data-stu-id="6ca0f-122">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="6ca0f-123">caracteres</span><span class="sxs-lookup"><span data-stu-id="6ca0f-123">alphabetic</span></span>|<span data-ttu-id="6ca0f-124">4 </span><span class="sxs-lookup"><span data-stu-id="6ca0f-124">4</span></span>|<span data-ttu-id="6ca0f-125">Pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="6ca0f-125">At least alphabetic password.</span></span>|
|<span data-ttu-id="6ca0f-126">tecla</span><span class="sxs-lookup"><span data-stu-id="6ca0f-126">alphanumeric</span></span>|<span data-ttu-id="6ca0f-127">5 </span><span class="sxs-lookup"><span data-stu-id="6ca0f-127">5</span></span>|<span data-ttu-id="6ca0f-128">Pelo menos a senha alfanumérica</span><span class="sxs-lookup"><span data-stu-id="6ca0f-128">At least alphanumeric password</span></span>|
|<span data-ttu-id="6ca0f-129">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="6ca0f-129">alphanumericWithSymbols</span></span>|<span data-ttu-id="6ca0f-130">6 </span><span class="sxs-lookup"><span data-stu-id="6ca0f-130">6</span></span>|<span data-ttu-id="6ca0f-131">Pelo menos alfanumérico com símbolos.</span><span class="sxs-lookup"><span data-stu-id="6ca0f-131">At least alphanumeric with symbols.</span></span>|
|<span data-ttu-id="6ca0f-132">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="6ca0f-132">lowSecurityBiometric</span></span>|<span data-ttu-id="6ca0f-133">7 </span><span class="sxs-lookup"><span data-stu-id="6ca0f-133">7</span></span>|<span data-ttu-id="6ca0f-134">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="6ca0f-134">Low security biometrics based password required.</span></span>|





