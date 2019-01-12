---
title: tipo de enum androidRequiredPasswordType
description: Tipo de senha necessária Android.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dc82ccd0519196495839f533dc09264525ac7fec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957547"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="46f59-103">tipo de enum androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="46f59-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="46f59-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="46f59-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46f59-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="46f59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46f59-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="46f59-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46f59-107">Tipo de senha necessária Android.</span><span class="sxs-lookup"><span data-stu-id="46f59-107">Android required password type.</span></span>
## <a name="members"></a><span data-ttu-id="46f59-108">Membros</span><span class="sxs-lookup"><span data-stu-id="46f59-108">Members</span></span>
|<span data-ttu-id="46f59-109">Membro</span><span class="sxs-lookup"><span data-stu-id="46f59-109">Member</span></span>|<span data-ttu-id="46f59-110">Valor</span><span class="sxs-lookup"><span data-stu-id="46f59-110">Value</span></span>|<span data-ttu-id="46f59-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="46f59-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46f59-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="46f59-112">deviceDefault</span></span>|<span data-ttu-id="46f59-113">0</span><span class="sxs-lookup"><span data-stu-id="46f59-113">0</span></span>|<span data-ttu-id="46f59-114">Valor de padrão de dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="46f59-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="46f59-115">alfabético</span><span class="sxs-lookup"><span data-stu-id="46f59-115">alphabetic</span></span>|<span data-ttu-id="46f59-116">1</span><span class="sxs-lookup"><span data-stu-id="46f59-116">1</span></span>|<span data-ttu-id="46f59-117">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="46f59-117">Alphabetic password required.</span></span>|
|<span data-ttu-id="46f59-118">alfanumérico</span><span class="sxs-lookup"><span data-stu-id="46f59-118">alphanumeric</span></span>|<span data-ttu-id="46f59-119">2</span><span class="sxs-lookup"><span data-stu-id="46f59-119">2</span></span>|<span data-ttu-id="46f59-120">Senha alfanumérica necessária.</span><span class="sxs-lookup"><span data-stu-id="46f59-120">Alphanumeric password required.</span></span>|
|<span data-ttu-id="46f59-121">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="46f59-121">alphanumericWithSymbols</span></span>|<span data-ttu-id="46f59-122">3</span><span class="sxs-lookup"><span data-stu-id="46f59-122">3</span></span>|<span data-ttu-id="46f59-123">Alfanumérico com senha de símbolos necessária.</span><span class="sxs-lookup"><span data-stu-id="46f59-123">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="46f59-124">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="46f59-124">lowSecurityBiometric</span></span>|<span data-ttu-id="46f59-125">4</span><span class="sxs-lookup"><span data-stu-id="46f59-125">4</span></span>|<span data-ttu-id="46f59-126">Biométrica baixa segurança com base em senha necessária.</span><span class="sxs-lookup"><span data-stu-id="46f59-126">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="46f59-127">numéricos</span><span class="sxs-lookup"><span data-stu-id="46f59-127">numeric</span></span>|<span data-ttu-id="46f59-128">5</span><span class="sxs-lookup"><span data-stu-id="46f59-128">5</span></span>|<span data-ttu-id="46f59-129">Senha numérica necessária.</span><span class="sxs-lookup"><span data-stu-id="46f59-129">Numeric password required.</span></span>|
|<span data-ttu-id="46f59-130">numericComplex</span><span class="sxs-lookup"><span data-stu-id="46f59-130">numericComplex</span></span>|<span data-ttu-id="46f59-131">6</span><span class="sxs-lookup"><span data-stu-id="46f59-131">6</span></span>|<span data-ttu-id="46f59-132">Senha complexa numérica necessária.</span><span class="sxs-lookup"><span data-stu-id="46f59-132">Numeric complex password required.</span></span>|
|<span data-ttu-id="46f59-133">qualquer</span><span class="sxs-lookup"><span data-stu-id="46f59-133">any</span></span>|<span data-ttu-id="46f59-134">7</span><span class="sxs-lookup"><span data-stu-id="46f59-134">7</span></span>|<span data-ttu-id="46f59-135">É necessária uma senha ou padrão e quaisquer é aceitável.</span><span class="sxs-lookup"><span data-stu-id="46f59-135">A password or pattern is required, and any is acceptable.</span></span>|





