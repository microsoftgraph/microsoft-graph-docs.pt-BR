---
title: tipo de enumeração mobileAppIntent
description: Indica o status do aplicativo móvel no dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8a530c7b67d4bde5829f11471434341d365d3275
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523342"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="b4d09-103">tipo de enumeração mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="b4d09-103">mobileAppIntent enum type</span></span>

<span data-ttu-id="b4d09-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4d09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4d09-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b4d09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4d09-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4d09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4d09-107">Indica o status do aplicativo móvel no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4d09-107">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="b4d09-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b4d09-108">Members</span></span>
|<span data-ttu-id="b4d09-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b4d09-109">Member</span></span>|<span data-ttu-id="b4d09-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b4d09-110">Value</span></span>|<span data-ttu-id="b4d09-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4d09-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4d09-112">disponível</span><span class="sxs-lookup"><span data-stu-id="b4d09-112">available</span></span>|<span data-ttu-id="b4d09-113">,0</span><span class="sxs-lookup"><span data-stu-id="b4d09-113">0</span></span>|<span data-ttu-id="b4d09-114">Disponível</span><span class="sxs-lookup"><span data-stu-id="b4d09-114">Available</span></span>|
|<span data-ttu-id="b4d09-115">Não disponível</span><span class="sxs-lookup"><span data-stu-id="b4d09-115">notAvailable</span></span>|<span data-ttu-id="b4d09-116">1 </span><span class="sxs-lookup"><span data-stu-id="b4d09-116">1</span></span>|<span data-ttu-id="b4d09-117">Não disponível</span><span class="sxs-lookup"><span data-stu-id="b4d09-117">Not Available</span></span>|
|<span data-ttu-id="b4d09-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="b4d09-118">requiredInstall</span></span>|<span data-ttu-id="b4d09-119">2 </span><span class="sxs-lookup"><span data-stu-id="b4d09-119">2</span></span>|<span data-ttu-id="b4d09-120">Instalação necessária</span><span class="sxs-lookup"><span data-stu-id="b4d09-120">Required Install</span></span>|
|<span data-ttu-id="b4d09-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="b4d09-121">requiredUninstall</span></span>|<span data-ttu-id="b4d09-122">3 </span><span class="sxs-lookup"><span data-stu-id="b4d09-122">3</span></span>|<span data-ttu-id="b4d09-123">Desinstalação necessária</span><span class="sxs-lookup"><span data-stu-id="b4d09-123">Required Uninstall</span></span>|
|<span data-ttu-id="b4d09-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="b4d09-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="b4d09-125">4 </span><span class="sxs-lookup"><span data-stu-id="b4d09-125">4</span></span>|<span data-ttu-id="b4d09-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="b4d09-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="b4d09-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="b4d09-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="b4d09-128">5 </span><span class="sxs-lookup"><span data-stu-id="b4d09-128">5</span></span>|<span data-ttu-id="b4d09-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="b4d09-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="b4d09-130">impedir</span><span class="sxs-lookup"><span data-stu-id="b4d09-130">exclude</span></span>|<span data-ttu-id="b4d09-131">6 </span><span class="sxs-lookup"><span data-stu-id="b4d09-131">6</span></span>|<span data-ttu-id="b4d09-132">Excluir</span><span class="sxs-lookup"><span data-stu-id="b4d09-132">Exclude</span></span>|



