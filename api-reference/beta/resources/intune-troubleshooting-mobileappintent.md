---
title: tipo de enum mobileAppIntent
description: Indica o status do aplicativo no dispositivo móvel.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7cd26912406fc428f28c65abce2169c14d686342
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933376"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="94f1f-103">tipo de enum mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="94f1f-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="94f1f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="94f1f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94f1f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="94f1f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94f1f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="94f1f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94f1f-107">Indica o status do aplicativo no dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="94f1f-107">Indicates the status of the mobile app on the device.</span></span>
## <a name="members"></a><span data-ttu-id="94f1f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="94f1f-108">Members</span></span>
|<span data-ttu-id="94f1f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="94f1f-109">Member</span></span>|<span data-ttu-id="94f1f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="94f1f-110">Value</span></span>|<span data-ttu-id="94f1f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="94f1f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94f1f-112">disponível</span><span class="sxs-lookup"><span data-stu-id="94f1f-112">available</span></span>|<span data-ttu-id="94f1f-113">0</span><span class="sxs-lookup"><span data-stu-id="94f1f-113">0</span></span>|<span data-ttu-id="94f1f-114">Disponível</span><span class="sxs-lookup"><span data-stu-id="94f1f-114">Available</span></span>|
|<span data-ttu-id="94f1f-115">notAvailable</span><span class="sxs-lookup"><span data-stu-id="94f1f-115">notAvailable</span></span>|<span data-ttu-id="94f1f-116">1</span><span class="sxs-lookup"><span data-stu-id="94f1f-116">1</span></span>|<span data-ttu-id="94f1f-117">Não disponível</span><span class="sxs-lookup"><span data-stu-id="94f1f-117">Not Available</span></span>|
|<span data-ttu-id="94f1f-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="94f1f-118">requiredInstall</span></span>|<span data-ttu-id="94f1f-119">2</span><span class="sxs-lookup"><span data-stu-id="94f1f-119">2</span></span>|<span data-ttu-id="94f1f-120">Instalação necessária</span><span class="sxs-lookup"><span data-stu-id="94f1f-120">Required Install</span></span>|
|<span data-ttu-id="94f1f-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="94f1f-121">requiredUninstall</span></span>|<span data-ttu-id="94f1f-122">3</span><span class="sxs-lookup"><span data-stu-id="94f1f-122">3</span></span>|<span data-ttu-id="94f1f-123">Desinstalar necessários</span><span class="sxs-lookup"><span data-stu-id="94f1f-123">Required Uninstall</span></span>|
|<span data-ttu-id="94f1f-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="94f1f-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="94f1f-125">4</span><span class="sxs-lookup"><span data-stu-id="94f1f-125">4</span></span>|<span data-ttu-id="94f1f-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="94f1f-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="94f1f-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="94f1f-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="94f1f-128">5</span><span class="sxs-lookup"><span data-stu-id="94f1f-128">5</span></span>|<span data-ttu-id="94f1f-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="94f1f-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="94f1f-130">Excluir</span><span class="sxs-lookup"><span data-stu-id="94f1f-130">exclude</span></span>|<span data-ttu-id="94f1f-131">6</span><span class="sxs-lookup"><span data-stu-id="94f1f-131">6</span></span>|<span data-ttu-id="94f1f-132">Excluir</span><span class="sxs-lookup"><span data-stu-id="94f1f-132">Exclude</span></span>|





