---
title: tipo de enumeração androidRequiredPasswordType
description: Tipo de senha exigido pelo Android.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59a95c74f19fa6e14440eaedd06d385b05d81e5d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255399"
---
# <a name="androidrequiredpasswordtype-enum-type"></a><span data-ttu-id="9a99a-103">tipo de enumeração androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9a99a-103">androidRequiredPasswordType enum type</span></span>

> <span data-ttu-id="9a99a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a99a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a99a-105">Tipo de senha exigido pelo Android.</span><span class="sxs-lookup"><span data-stu-id="9a99a-105">Android required password type.</span></span>

## <a name="members"></a><span data-ttu-id="9a99a-106">Membros</span><span class="sxs-lookup"><span data-stu-id="9a99a-106">Members</span></span>
|<span data-ttu-id="9a99a-107">Membro</span><span class="sxs-lookup"><span data-stu-id="9a99a-107">Member</span></span>|<span data-ttu-id="9a99a-108">Valor</span><span class="sxs-lookup"><span data-stu-id="9a99a-108">Value</span></span>|<span data-ttu-id="9a99a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a99a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a99a-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9a99a-110">deviceDefault</span></span>|<span data-ttu-id="9a99a-111">,0</span><span class="sxs-lookup"><span data-stu-id="9a99a-111">0</span></span>|<span data-ttu-id="9a99a-112">Valor padrão do dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="9a99a-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="9a99a-113">caracteres</span><span class="sxs-lookup"><span data-stu-id="9a99a-113">alphabetic</span></span>|<span data-ttu-id="9a99a-114">1</span><span class="sxs-lookup"><span data-stu-id="9a99a-114">1</span></span>|<span data-ttu-id="9a99a-115">Senha alfabética necessária.</span><span class="sxs-lookup"><span data-stu-id="9a99a-115">Alphabetic password required.</span></span>|
|<span data-ttu-id="9a99a-116">tecla</span><span class="sxs-lookup"><span data-stu-id="9a99a-116">alphanumeric</span></span>|<span data-ttu-id="9a99a-117">duas</span><span class="sxs-lookup"><span data-stu-id="9a99a-117">2</span></span>|<span data-ttu-id="9a99a-118">Senha alfanumérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="9a99a-118">Alphanumeric password required.</span></span>|
|<span data-ttu-id="9a99a-119">alphanumericWithSymbols</span><span class="sxs-lookup"><span data-stu-id="9a99a-119">alphanumericWithSymbols</span></span>|<span data-ttu-id="9a99a-120">3D</span><span class="sxs-lookup"><span data-stu-id="9a99a-120">3</span></span>|<span data-ttu-id="9a99a-121">Alfanumérica com símbolos de senha necessários.</span><span class="sxs-lookup"><span data-stu-id="9a99a-121">Alphanumeric with symbols password required.</span></span>|
|<span data-ttu-id="9a99a-122">lowSecurityBiometric</span><span class="sxs-lookup"><span data-stu-id="9a99a-122">lowSecurityBiometric</span></span>|<span data-ttu-id="9a99a-123">quatro</span><span class="sxs-lookup"><span data-stu-id="9a99a-123">4</span></span>|<span data-ttu-id="9a99a-124">Senha com base em Biometria de segurança baixa necessária.</span><span class="sxs-lookup"><span data-stu-id="9a99a-124">Low security biometrics based password required.</span></span>|
|<span data-ttu-id="9a99a-125">numéricos</span><span class="sxs-lookup"><span data-stu-id="9a99a-125">numeric</span></span>|<span data-ttu-id="9a99a-126">0,5</span><span class="sxs-lookup"><span data-stu-id="9a99a-126">5</span></span>|<span data-ttu-id="9a99a-127">Senha numérica obrigatória.</span><span class="sxs-lookup"><span data-stu-id="9a99a-127">Numeric password required.</span></span>|
|<span data-ttu-id="9a99a-128">numericComplex</span><span class="sxs-lookup"><span data-stu-id="9a99a-128">numericComplex</span></span>|<span data-ttu-id="9a99a-129">6</span><span class="sxs-lookup"><span data-stu-id="9a99a-129">6</span></span>|<span data-ttu-id="9a99a-130">Senha numérica complexa obrigatória.</span><span class="sxs-lookup"><span data-stu-id="9a99a-130">Numeric complex password required.</span></span>|
|<span data-ttu-id="9a99a-131">qualquer</span><span class="sxs-lookup"><span data-stu-id="9a99a-131">any</span></span>|<span data-ttu-id="9a99a-132">178</span><span class="sxs-lookup"><span data-stu-id="9a99a-132">7</span></span>|<span data-ttu-id="9a99a-133">Uma senha ou um padrão é necessário, e qualquer um é aceitável.</span><span class="sxs-lookup"><span data-stu-id="9a99a-133">A password or pattern is required, and any is acceptable.</span></span>|



