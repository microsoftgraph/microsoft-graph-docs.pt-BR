---
title: tipo de enum androidDeviceOwnerRequiredPasswordType
description: Política do proprietário do dispositivo Android necessários tipo de senha.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c405cf3a69597994d5539427698baa92cabd3904
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403536"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="9530f-103">tipo de enum androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9530f-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="9530f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9530f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9530f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9530f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9530f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9530f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9530f-107">Política do proprietário do dispositivo Android necessários tipo de senha.</span><span class="sxs-lookup"><span data-stu-id="9530f-107">Android Device Owner policy required password type.</span></span>

## <a name="members"></a><span data-ttu-id="9530f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="9530f-108">Members</span></span>
|<span data-ttu-id="9530f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="9530f-109">Member</span></span>|<span data-ttu-id="9530f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="9530f-110">Value</span></span>|<span data-ttu-id="9530f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9530f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9530f-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9530f-112">deviceDefault</span></span>|<span data-ttu-id="9530f-113">0</span><span class="sxs-lookup"><span data-stu-id="9530f-113">0</span></span>|<span data-ttu-id="9530f-114">Valor de padrão de dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="9530f-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="9530f-115">obrigatório</span><span class="sxs-lookup"><span data-stu-id="9530f-115">required</span></span>|<span data-ttu-id="9530f-116">1</span><span class="sxs-lookup"><span data-stu-id="9530f-116">1</span></span>|<span data-ttu-id="9530f-117">Deve haver um conjunto de senha, mas não existem restrições no tipo.</span><span class="sxs-lookup"><span data-stu-id="9530f-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="9530f-118">numéricos</span><span class="sxs-lookup"><span data-stu-id="9530f-118">numeric</span></span>|<span data-ttu-id="9530f-119">2</span><span class="sxs-lookup"><span data-stu-id="9530f-119">2</span></span>|<span data-ttu-id="9530f-120">AT menos numérico.</span><span class="sxs-lookup"><span data-stu-id="9530f-120">At least numeric.</span></span>|
|<span data-ttu-id="9530f-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="9530f-121">numericComplex</span></span>|<span data-ttu-id="9530f-122">3</span><span class="sxs-lookup"><span data-stu-id="9530f-122">3</span></span>|<span data-ttu-id="9530f-123">AT menos numérico com sequências de repetição ou ordenadas.</span><span class="sxs-lookup"><span data-stu-id="9530f-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="9530f-124">alfabético</span><span class="sxs-lookup"><span data-stu-id="9530f-124">alphabetic</span></span>|<span data-ttu-id="9530f-125">4</span><span class="sxs-lookup"><span data-stu-id="9530f-125">4</span></span>|<span data-ttu-id="9530f-126">Senha de pelo menos alfabética.</span><span class="sxs-lookup"><span data-stu-id="9530f-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="9530f-127">alfanumérico</span><span class="sxs-lookup"><span data-stu-id="9530f-127">alphanumeric</span></span>|<span data-ttu-id="9530f-128">5</span><span class="sxs-lookup"><span data-stu-id="9530f-128">5</span></span>|<span data-ttu-id="9530f-129">Senha alfanumérica pelo menos</span><span class="sxs-lookup"><span data-stu-id="9530f-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="9530f-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="9530f-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="9530f-131">6</span><span class="sxs-lookup"><span data-stu-id="9530f-131">6</span></span>|<span data-ttu-id="9530f-132">Pelo menos alfanumérico com símbolos.</span><span class="sxs-lookup"><span data-stu-id="9530f-132">At least alphanumeric with symbols.</span></span>|




