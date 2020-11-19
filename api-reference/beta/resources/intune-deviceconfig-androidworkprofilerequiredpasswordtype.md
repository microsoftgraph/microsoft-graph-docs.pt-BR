---
title: tipo de enumeração androidWorkProfileRequiredPasswordType
description: Perfil de trabalho do Android tipo de senha exigido.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: aa7ab836addd205d0b39c14fa0dcb42dd71bb81a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256957"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a><span data-ttu-id="bb465-103">tipo de enumeração androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bb465-103">androidWorkProfileRequiredPasswordType enum type</span></span>

<span data-ttu-id="bb465-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb465-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb465-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb465-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb465-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb465-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb465-107">Perfil de trabalho do Android tipo de senha exigido.</span><span class="sxs-lookup"><span data-stu-id="bb465-107">Android Work Profile required password type.</span></span>

## <a name="members"></a><span data-ttu-id="bb465-108">Membros</span><span class="sxs-lookup"><span data-stu-id="bb465-108">Members</span></span>
|<span data-ttu-id="bb465-109">Membro</span><span class="sxs-lookup"><span data-stu-id="bb465-109">Member</span></span>|<span data-ttu-id="bb465-110">Valor</span><span class="sxs-lookup"><span data-stu-id="bb465-110">Value</span></span>|<span data-ttu-id="bb465-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb465-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb465-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="bb465-112">deviceDefault</span></span>|<span data-ttu-id="bb465-113">,0</span><span class="sxs-lookup"><span data-stu-id="bb465-113">0</span></span>|<span data-ttu-id="bb465-114">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="bb465-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="bb465-115">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="bb465-115">lowSecurityBiometric</span></span>|<span data-ttu-id="bb465-116">1</span><span class="sxs-lookup"><span data-stu-id="bb465-116">1</span></span>|<span data-ttu-id="bb465-117">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="bb465-117">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="bb465-118">obrigatório</span><span class="sxs-lookup"><span data-stu-id="bb465-118">required</span></span>|<span data-ttu-id="bb465-119">duas</span><span class="sxs-lookup"><span data-stu-id="bb465-119">2</span></span>|<span data-ttu-id="bb465-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb465-120">Required.</span></span>|
|<span data-ttu-id="bb465-121">atLeastNumeric</span><span class="sxs-lookup"><span data-stu-id="bb465-121">atLeastNumeric</span></span>|<span data-ttu-id="bb465-122">3D</span><span class="sxs-lookup"><span data-stu-id="bb465-122">3</span></span>|<span data-ttu-id="bb465-123">É necessário pelo menos a senha numérica.</span><span class="sxs-lookup"><span data-stu-id="bb465-123">At least numeric password required.</span></span>|
|<span data-ttu-id="bb465-124">numericComplex</span><span class="sxs-lookup"><span data-stu-id="bb465-124">numericComplex</span></span>|<span data-ttu-id="bb465-125">4 </span><span class="sxs-lookup"><span data-stu-id="bb465-125">4</span></span>|<span data-ttu-id="bb465-126">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="bb465-126">Numeric complex password required.</span></span>|
|<span data-ttu-id="bb465-127">atLeastAlphabetic</span><span class="sxs-lookup"><span data-stu-id="bb465-127">atLeastAlphabetic</span></span>|<span data-ttu-id="bb465-128">5 </span><span class="sxs-lookup"><span data-stu-id="bb465-128">5</span></span>|<span data-ttu-id="bb465-129">É necessária pelo menos a senha alfabética.</span><span class="sxs-lookup"><span data-stu-id="bb465-129">At least alphabetic password required.</span></span>|
|<span data-ttu-id="bb465-130">atLeastAlphanumeric</span><span class="sxs-lookup"><span data-stu-id="bb465-130">atLeastAlphanumeric</span></span>|<span data-ttu-id="bb465-131">6 </span><span class="sxs-lookup"><span data-stu-id="bb465-131">6</span></span>|<span data-ttu-id="bb465-132">É necessária pelo menos a senha alfanumérica.</span><span class="sxs-lookup"><span data-stu-id="bb465-132">At least alphanumeric password required.</span></span>|
|<span data-ttu-id="bb465-133">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="bb465-133">alphanumericWithSymbols</span></span>|<span data-ttu-id="bb465-134">7 </span><span class="sxs-lookup"><span data-stu-id="bb465-134">7</span></span>|<span data-ttu-id="bb465-135">É necessário pelo menos alfanumérico com senha de símbolo.</span><span class="sxs-lookup"><span data-stu-id="bb465-135">At least alphanumeric with symbols password required.</span></span>|




