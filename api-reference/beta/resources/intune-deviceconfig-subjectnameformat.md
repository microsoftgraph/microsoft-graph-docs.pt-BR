---
title: tipo de enum subjectNameFormat
description: Opções de formato de nome de entidade.
author: tfitzmac
ms.openlocfilehash: 61aeddb1e751885c3a0ba39fd5628b71830dded5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307004"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="016f9-103">tipo de enum subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="016f9-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="016f9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="016f9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="016f9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="016f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="016f9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="016f9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="016f9-107">Opções de formato de nome de entidade.</span><span class="sxs-lookup"><span data-stu-id="016f9-107">Subject Name Format Options.</span></span>
## <a name="members"></a><span data-ttu-id="016f9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="016f9-108">Members</span></span>
|<span data-ttu-id="016f9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="016f9-109">Member</span></span>|<span data-ttu-id="016f9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="016f9-110">Value</span></span>|<span data-ttu-id="016f9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="016f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="016f9-112">commonName</span><span class="sxs-lookup"><span data-stu-id="016f9-112">commonName</span></span>|<span data-ttu-id="016f9-113">0</span><span class="sxs-lookup"><span data-stu-id="016f9-113">0</span></span>|<span data-ttu-id="016f9-114">Nome comum.</span><span class="sxs-lookup"><span data-stu-id="016f9-114">Common name.</span></span>|
|<span data-ttu-id="016f9-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="016f9-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="016f9-116">1</span><span class="sxs-lookup"><span data-stu-id="016f9-116">1</span></span>|<span data-ttu-id="016f9-117">Nome comum, incluindo Email.</span><span class="sxs-lookup"><span data-stu-id="016f9-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="016f9-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="016f9-118">commonNameAsEmail</span></span>|<span data-ttu-id="016f9-119">2</span><span class="sxs-lookup"><span data-stu-id="016f9-119">2</span></span>|<span data-ttu-id="016f9-120">Nome comum como Email.</span><span class="sxs-lookup"><span data-stu-id="016f9-120">Common Name As Email.</span></span>|
|<span data-ttu-id="016f9-121">custom</span><span class="sxs-lookup"><span data-stu-id="016f9-121">custom</span></span>|<span data-ttu-id="016f9-122">3</span><span class="sxs-lookup"><span data-stu-id="016f9-122">3</span></span>|<span data-ttu-id="016f9-123">Formato de nome de entidade personalizada.</span><span class="sxs-lookup"><span data-stu-id="016f9-123">Custom subject name format.</span></span>|
|<span data-ttu-id="016f9-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="016f9-124">commonNameAsIMEI</span></span>|<span data-ttu-id="016f9-125">5</span><span class="sxs-lookup"><span data-stu-id="016f9-125">5</span></span>|<span data-ttu-id="016f9-126">Nome comum como IMEI.</span><span class="sxs-lookup"><span data-stu-id="016f9-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="016f9-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="016f9-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="016f9-128">6</span><span class="sxs-lookup"><span data-stu-id="016f9-128">6</span></span>|<span data-ttu-id="016f9-129">Nome comum como número de série.</span><span class="sxs-lookup"><span data-stu-id="016f9-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="016f9-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="016f9-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="016f9-131">7</span><span class="sxs-lookup"><span data-stu-id="016f9-131">7</span></span>|<span data-ttu-id="016f9-132">Nome comum como número de série.</span><span class="sxs-lookup"><span data-stu-id="016f9-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="016f9-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="016f9-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="016f9-134">8</span><span class="sxs-lookup"><span data-stu-id="016f9-134">8</span></span>|<span data-ttu-id="016f9-135">Nome comum como número de série.</span><span class="sxs-lookup"><span data-stu-id="016f9-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="016f9-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="016f9-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="016f9-137">9</span><span class="sxs-lookup"><span data-stu-id="016f9-137">9</span></span>|<span data-ttu-id="016f9-138">Nome comum como número de série.</span><span class="sxs-lookup"><span data-stu-id="016f9-138">Common Name As Serial Number.</span></span>|





