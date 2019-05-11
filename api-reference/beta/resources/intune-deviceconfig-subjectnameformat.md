---
title: tipo de enumeração subjectNameFormat
description: Opções de formato de nome de entidade.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b1dd107db00ea871c1055e7a17bec1792076c68
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944660"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="3a41c-103">tipo de enumeração subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="3a41c-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="3a41c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a41c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a41c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a41c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a41c-106">Opções de formato de nome de entidade.</span><span class="sxs-lookup"><span data-stu-id="3a41c-106">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="3a41c-107">Membros</span><span class="sxs-lookup"><span data-stu-id="3a41c-107">Members</span></span>
|<span data-ttu-id="3a41c-108">Membro</span><span class="sxs-lookup"><span data-stu-id="3a41c-108">Member</span></span>|<span data-ttu-id="3a41c-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3a41c-109">Value</span></span>|<span data-ttu-id="3a41c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a41c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a41c-111">CommonName</span><span class="sxs-lookup"><span data-stu-id="3a41c-111">commonName</span></span>|<span data-ttu-id="3a41c-112">,0</span><span class="sxs-lookup"><span data-stu-id="3a41c-112">0</span></span>|<span data-ttu-id="3a41c-113">Nome comum.</span><span class="sxs-lookup"><span data-stu-id="3a41c-113">Common name.</span></span>|
|<span data-ttu-id="3a41c-114">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="3a41c-114">commonNameIncludingEmail</span></span>|<span data-ttu-id="3a41c-115">1</span><span class="sxs-lookup"><span data-stu-id="3a41c-115">1</span></span>|<span data-ttu-id="3a41c-116">Nome comum incluindo email.</span><span class="sxs-lookup"><span data-stu-id="3a41c-116">Common Name Including Email.</span></span>|
|<span data-ttu-id="3a41c-117">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="3a41c-117">commonNameAsEmail</span></span>|<span data-ttu-id="3a41c-118">duas</span><span class="sxs-lookup"><span data-stu-id="3a41c-118">2</span></span>|<span data-ttu-id="3a41c-119">Nome comum como email.</span><span class="sxs-lookup"><span data-stu-id="3a41c-119">Common Name As Email.</span></span>|
|<span data-ttu-id="3a41c-120">cliente</span><span class="sxs-lookup"><span data-stu-id="3a41c-120">custom</span></span>|<span data-ttu-id="3a41c-121">3D</span><span class="sxs-lookup"><span data-stu-id="3a41c-121">3</span></span>|<span data-ttu-id="3a41c-122">Formato de nome de entidade personalizado.</span><span class="sxs-lookup"><span data-stu-id="3a41c-122">Custom subject name format.</span></span>|
|<span data-ttu-id="3a41c-123">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="3a41c-123">commonNameAsIMEI</span></span>|<span data-ttu-id="3a41c-124">0,5</span><span class="sxs-lookup"><span data-stu-id="3a41c-124">5</span></span>|<span data-ttu-id="3a41c-125">Nome comum como IMEI.</span><span class="sxs-lookup"><span data-stu-id="3a41c-125">Common Name As IMEI.</span></span>|
|<span data-ttu-id="3a41c-126">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="3a41c-126">commonNameAsSerialNumber</span></span>|<span data-ttu-id="3a41c-127">6</span><span class="sxs-lookup"><span data-stu-id="3a41c-127">6</span></span>|<span data-ttu-id="3a41c-128">Nome comum como número de série.</span><span class="sxs-lookup"><span data-stu-id="3a41c-128">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="3a41c-129">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="3a41c-129">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="3a41c-130">178</span><span class="sxs-lookup"><span data-stu-id="3a41c-130">7</span></span>|<span data-ttu-id="3a41c-131">Nome comum como número de série.</span><span class="sxs-lookup"><span data-stu-id="3a41c-131">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="3a41c-132">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="3a41c-132">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="3a41c-133">8 </span><span class="sxs-lookup"><span data-stu-id="3a41c-133">8</span></span>|<span data-ttu-id="3a41c-134">Nome comum como número de série.</span><span class="sxs-lookup"><span data-stu-id="3a41c-134">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="3a41c-135">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="3a41c-135">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="3a41c-136">9 </span><span class="sxs-lookup"><span data-stu-id="3a41c-136">9</span></span>|<span data-ttu-id="3a41c-137">Nome comum como número de série.</span><span class="sxs-lookup"><span data-stu-id="3a41c-137">Common Name As Serial Number.</span></span>|




