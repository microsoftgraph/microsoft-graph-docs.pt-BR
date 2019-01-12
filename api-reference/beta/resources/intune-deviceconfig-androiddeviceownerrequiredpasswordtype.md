---
title: tipo de enum androidDeviceOwnerRequiredPasswordType
description: Política do proprietário do dispositivo Android necessários tipo de senha.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b1208de597baff9dd05a48663435a3a928f3dae9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938038"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a><span data-ttu-id="88413-103">tipo de enum androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="88413-103">androidDeviceOwnerRequiredPasswordType enum type</span></span>

> <span data-ttu-id="88413-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="88413-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88413-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="88413-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88413-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="88413-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88413-107">Política do proprietário do dispositivo Android necessários tipo de senha.</span><span class="sxs-lookup"><span data-stu-id="88413-107">Android Device Owner policy required password type.</span></span>
## <a name="members"></a><span data-ttu-id="88413-108">Membros</span><span class="sxs-lookup"><span data-stu-id="88413-108">Members</span></span>
|<span data-ttu-id="88413-109">Membro</span><span class="sxs-lookup"><span data-stu-id="88413-109">Member</span></span>|<span data-ttu-id="88413-110">Valor</span><span class="sxs-lookup"><span data-stu-id="88413-110">Value</span></span>|<span data-ttu-id="88413-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="88413-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88413-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="88413-112">deviceDefault</span></span>|<span data-ttu-id="88413-113">0</span><span class="sxs-lookup"><span data-stu-id="88413-113">0</span></span>|<span data-ttu-id="88413-114">Valor de padrão de dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="88413-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="88413-115">obrigatório</span><span class="sxs-lookup"><span data-stu-id="88413-115">required</span></span>|<span data-ttu-id="88413-116">1</span><span class="sxs-lookup"><span data-stu-id="88413-116">1</span></span>|<span data-ttu-id="88413-117">Deve haver um conjunto de senha, mas não existem restrições no tipo.</span><span class="sxs-lookup"><span data-stu-id="88413-117">There must be a password set, but there are no restrictions on type.</span></span>|
|<span data-ttu-id="88413-118">numéricos</span><span class="sxs-lookup"><span data-stu-id="88413-118">numeric</span></span>|<span data-ttu-id="88413-119">2</span><span class="sxs-lookup"><span data-stu-id="88413-119">2</span></span>|<span data-ttu-id="88413-120">AT menos numérico.</span><span class="sxs-lookup"><span data-stu-id="88413-120">At least numeric.</span></span>|
|<span data-ttu-id="88413-121">numericComplex</span><span class="sxs-lookup"><span data-stu-id="88413-121">numericComplex</span></span>|<span data-ttu-id="88413-122">3</span><span class="sxs-lookup"><span data-stu-id="88413-122">3</span></span>|<span data-ttu-id="88413-123">AT menos numérico com sequências de repetição ou ordenadas.</span><span class="sxs-lookup"><span data-stu-id="88413-123">At least numeric with no repeating or ordered sequences.</span></span>|
|<span data-ttu-id="88413-124">alfabético</span><span class="sxs-lookup"><span data-stu-id="88413-124">alphabetic</span></span>|<span data-ttu-id="88413-125">4</span><span class="sxs-lookup"><span data-stu-id="88413-125">4</span></span>|<span data-ttu-id="88413-126">Senha de pelo menos alfabética.</span><span class="sxs-lookup"><span data-stu-id="88413-126">At least alphabetic password.</span></span>|
|<span data-ttu-id="88413-127">alfanumérico</span><span class="sxs-lookup"><span data-stu-id="88413-127">alphanumeric</span></span>|<span data-ttu-id="88413-128">5</span><span class="sxs-lookup"><span data-stu-id="88413-128">5</span></span>|<span data-ttu-id="88413-129">Senha alfanumérica pelo menos</span><span class="sxs-lookup"><span data-stu-id="88413-129">At least alphanumeric password</span></span>|
|<span data-ttu-id="88413-130">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="88413-130">alphanumericWithSymbols</span></span>|<span data-ttu-id="88413-131">6</span><span class="sxs-lookup"><span data-stu-id="88413-131">6</span></span>|<span data-ttu-id="88413-132">Pelo menos alfanumérico com símbolos.</span><span class="sxs-lookup"><span data-stu-id="88413-132">At least alphanumeric with symbols.</span></span>|





