---
title: tipo de enum androidDeviceOwnerRequiredPasswordType
description: Política do proprietário do dispositivo Android necessários tipo de senha.
ms.openlocfilehash: 16f4bc59f2b4fa9f37989d1bc1978cdfacb2892c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037551"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="72cbc-103">tipo de enum androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="72cbc-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="72cbc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="72cbc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72cbc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="72cbc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72cbc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="72cbc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72cbc-107">Política do proprietário do dispositivo Android necessários tipo de senha.</span><span class="sxs-lookup"><span data-stu-id="72cbc-107">Android Device Owner policy required password type.</span></span>
## <a name="members"></a><span data-ttu-id="72cbc-108">Membros</span><span class="sxs-lookup"><span data-stu-id="72cbc-108">Members</span></span>
|<span data-ttu-id="72cbc-109">Membro</span><span class="sxs-lookup"><span data-stu-id="72cbc-109">Member</span></span>|<span data-ttu-id="72cbc-110">Valor</span><span class="sxs-lookup"><span data-stu-id="72cbc-110">Value</span></span>|<span data-ttu-id="72cbc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="72cbc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72cbc-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="72cbc-112">deviceDefault</span></span>|<span data-ttu-id="72cbc-113">0</span><span class="sxs-lookup"><span data-stu-id="72cbc-113">0</span></span>|<span data-ttu-id="72cbc-114">Valor de padrão de dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="72cbc-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="72cbc-115">obrigatório</span><span class="sxs-lookup"><span data-stu-id="72cbc-115">required</span></span>|<span data-ttu-id="72cbc-116">1</span><span class="sxs-lookup"><span data-stu-id="72cbc-116">1</span></span>|<span data-ttu-id="72cbc-117">Deve haver um conjunto de senha, mas não existem restrições no tipo.</span><span class="sxs-lookup"><span data-stu-id="72cbc-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="72cbc-118">numéricos</span><span class="sxs-lookup"><span data-stu-id="72cbc-118">numeric</span></span>|<span data-ttu-id="72cbc-119">2</span><span class="sxs-lookup"><span data-stu-id="72cbc-119">2</span></span>|<span data-ttu-id="72cbc-120">AT menos numérico.</span><span class="sxs-lookup"><span data-stu-id="72cbc-120">At least numeric.</span></span>|
|<span data-ttu-id="72cbc-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="72cbc-121">numericComplex</span></span>|<span data-ttu-id="72cbc-122">3</span><span class="sxs-lookup"><span data-stu-id="72cbc-122">3</span></span>|<span data-ttu-id="72cbc-123">AT menos numérico com sequências de repetição ou ordenadas.</span><span class="sxs-lookup"><span data-stu-id="72cbc-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="72cbc-124">alfabético</span><span class="sxs-lookup"><span data-stu-id="72cbc-124">alphabetic</span></span>|<span data-ttu-id="72cbc-125">4</span><span class="sxs-lookup"><span data-stu-id="72cbc-125">4</span></span>|<span data-ttu-id="72cbc-126">Senha de pelo menos alfabética.</span><span class="sxs-lookup"><span data-stu-id="72cbc-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="72cbc-127">alfanumérico</span><span class="sxs-lookup"><span data-stu-id="72cbc-127">alphanumeric</span></span>|<span data-ttu-id="72cbc-128">5</span><span class="sxs-lookup"><span data-stu-id="72cbc-128">5</span></span>|<span data-ttu-id="72cbc-129">Senha alfanumérica pelo menos</span><span class="sxs-lookup"><span data-stu-id="72cbc-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="72cbc-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="72cbc-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="72cbc-131">6</span><span class="sxs-lookup"><span data-stu-id="72cbc-131">6</span></span>|<span data-ttu-id="72cbc-132">Pelo menos alfanumérico com símbolos.</span><span class="sxs-lookup"><span data-stu-id="72cbc-132">At least alphanumeric with symbols.</span></span>|





