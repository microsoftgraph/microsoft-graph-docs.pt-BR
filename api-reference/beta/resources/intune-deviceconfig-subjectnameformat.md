---
title: tipo de enum subjectNameFormat
description: Opções de formato de nome de entidade.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 259af745567a0fc5de004f5a804d8bab00355f8f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969587"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="b59ca-103">tipo de enum subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="b59ca-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="b59ca-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b59ca-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b59ca-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b59ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b59ca-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b59ca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b59ca-107">Opções de formato de nome de entidade.</span><span class="sxs-lookup"><span data-stu-id="b59ca-107">Subject Name Format Options.</span></span>
## <a name="members"></a><span data-ttu-id="b59ca-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b59ca-108">Members</span></span>
|<span data-ttu-id="b59ca-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b59ca-109">Member</span></span>|<span data-ttu-id="b59ca-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b59ca-110">Value</span></span>|<span data-ttu-id="b59ca-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b59ca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b59ca-112">commonName</span><span class="sxs-lookup"><span data-stu-id="b59ca-112">commonName</span></span>|<span data-ttu-id="b59ca-113">0</span><span class="sxs-lookup"><span data-stu-id="b59ca-113">0</span></span>|<span data-ttu-id="b59ca-114">Nome comum.</span><span class="sxs-lookup"><span data-stu-id="b59ca-114">Common name.</span></span>|
|<span data-ttu-id="b59ca-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="b59ca-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="b59ca-116">1</span><span class="sxs-lookup"><span data-stu-id="b59ca-116">1</span></span>|<span data-ttu-id="b59ca-117">Nome comum, incluindo Email.</span><span class="sxs-lookup"><span data-stu-id="b59ca-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="b59ca-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="b59ca-118">commonNameAsEmail</span></span>|<span data-ttu-id="b59ca-119">2</span><span class="sxs-lookup"><span data-stu-id="b59ca-119">2</span></span>|<span data-ttu-id="b59ca-120">Nome comum como Email.</span><span class="sxs-lookup"><span data-stu-id="b59ca-120">Common Name As Email.</span></span>|
|<span data-ttu-id="b59ca-121">custom</span><span class="sxs-lookup"><span data-stu-id="b59ca-121">custom</span></span>|<span data-ttu-id="b59ca-122">3</span><span class="sxs-lookup"><span data-stu-id="b59ca-122">3</span></span>|<span data-ttu-id="b59ca-123">Formato de nome de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="b59ca-123">Custom subject name format.</span></span>|
|<span data-ttu-id="b59ca-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="b59ca-124">commonNameAsIMEI</span></span>|<span data-ttu-id="b59ca-125">5</span><span class="sxs-lookup"><span data-stu-id="b59ca-125">5</span></span>|<span data-ttu-id="b59ca-126">Nome comum como IMEI.</span><span class="sxs-lookup"><span data-stu-id="b59ca-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="b59ca-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="b59ca-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="b59ca-128">6</span><span class="sxs-lookup"><span data-stu-id="b59ca-128">6</span></span>|<span data-ttu-id="b59ca-129">Nome comum como número de série.</span><span class="sxs-lookup"><span data-stu-id="b59ca-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="b59ca-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="b59ca-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="b59ca-131">7</span><span class="sxs-lookup"><span data-stu-id="b59ca-131">7</span></span>|<span data-ttu-id="b59ca-132">Nome comum como número de série.</span><span class="sxs-lookup"><span data-stu-id="b59ca-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="b59ca-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="b59ca-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="b59ca-134">8</span><span class="sxs-lookup"><span data-stu-id="b59ca-134">8</span></span>|<span data-ttu-id="b59ca-135">Nome comum como número de série.</span><span class="sxs-lookup"><span data-stu-id="b59ca-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="b59ca-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="b59ca-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="b59ca-137">9</span><span class="sxs-lookup"><span data-stu-id="b59ca-137">9</span></span>|<span data-ttu-id="b59ca-138">Nome comum como número de série.</span><span class="sxs-lookup"><span data-stu-id="b59ca-138">Common Name As Serial Number.</span></span>|





