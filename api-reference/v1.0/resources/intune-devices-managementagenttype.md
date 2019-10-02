---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: df4f3cbe6237471548dced1c13cfef601cbe7965
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356909"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="ddf5e-103">tipo de enumeração managementAgentType</span><span class="sxs-lookup"><span data-stu-id="ddf5e-103">managementAgentType enum type</span></span>

> <span data-ttu-id="ddf5e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ddf5e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddf5e-105">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ddf5e-105">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="ddf5e-106">Membros</span><span class="sxs-lookup"><span data-stu-id="ddf5e-106">Members</span></span>
|<span data-ttu-id="ddf5e-107">Membro</span><span class="sxs-lookup"><span data-stu-id="ddf5e-107">Member</span></span>|<span data-ttu-id="ddf5e-108">Valor</span><span class="sxs-lookup"><span data-stu-id="ddf5e-108">Value</span></span>|<span data-ttu-id="ddf5e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddf5e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddf5e-110">Estendi</span><span class="sxs-lookup"><span data-stu-id="ddf5e-110">eas</span></span>|<span data-ttu-id="ddf5e-111">1</span><span class="sxs-lookup"><span data-stu-id="ddf5e-111">1</span></span>|<span data-ttu-id="ddf5e-112">O dispositivo é gerenciado pelo Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="ddf5e-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="ddf5e-113">MDM</span><span class="sxs-lookup"><span data-stu-id="ddf5e-113">mdm</span></span>|<span data-ttu-id="ddf5e-114">duas</span><span class="sxs-lookup"><span data-stu-id="ddf5e-114">2</span></span>|<span data-ttu-id="ddf5e-115">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="ddf5e-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="ddf5e-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="ddf5e-116">easMdm</span></span>|<span data-ttu-id="ddf5e-117">3D</span><span class="sxs-lookup"><span data-stu-id="ddf5e-117">3</span></span>|<span data-ttu-id="ddf5e-118">O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="ddf5e-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="ddf5e-119">intuneClient</span><span class="sxs-lookup"><span data-stu-id="ddf5e-119">intuneClient</span></span>|<span data-ttu-id="ddf5e-120">quatro</span><span class="sxs-lookup"><span data-stu-id="ddf5e-120">4</span></span>|<span data-ttu-id="ddf5e-121">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="ddf5e-121">Intune client managed.</span></span>|
|<span data-ttu-id="ddf5e-122">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="ddf5e-122">easIntuneClient</span></span>|<span data-ttu-id="ddf5e-123">0,5</span><span class="sxs-lookup"><span data-stu-id="ddf5e-123">5</span></span>|<span data-ttu-id="ddf5e-124">O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.</span><span class="sxs-lookup"><span data-stu-id="ddf5e-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="ddf5e-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="ddf5e-125">configurationManagerClient</span></span>|<span data-ttu-id="ddf5e-126">8 </span><span class="sxs-lookup"><span data-stu-id="ddf5e-126">8</span></span>|<span data-ttu-id="ddf5e-127">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="ddf5e-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="ddf5e-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="ddf5e-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="ddf5e-129">10 </span><span class="sxs-lookup"><span data-stu-id="ddf5e-129">10</span></span>|<span data-ttu-id="ddf5e-130">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="ddf5e-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="ddf5e-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="ddf5e-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="ddf5e-132">11</span><span class="sxs-lookup"><span data-stu-id="ddf5e-132">11</span></span>|<span data-ttu-id="ddf5e-133">O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.</span><span class="sxs-lookup"><span data-stu-id="ddf5e-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="ddf5e-134">desconhecido</span><span class="sxs-lookup"><span data-stu-id="ddf5e-134">unknown</span></span>|<span data-ttu-id="ddf5e-135">dezesseis</span><span class="sxs-lookup"><span data-stu-id="ddf5e-135">16</span></span>|<span data-ttu-id="ddf5e-136">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="ddf5e-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="ddf5e-137">jamf</span><span class="sxs-lookup"><span data-stu-id="ddf5e-137">jamf</span></span>|<span data-ttu-id="ddf5e-138">32</span><span class="sxs-lookup"><span data-stu-id="ddf5e-138">32</span></span>|<span data-ttu-id="ddf5e-139">Os atributos do dispositivo são buscados do JAMF.</span><span class="sxs-lookup"><span data-stu-id="ddf5e-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="ddf5e-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="ddf5e-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="ddf5e-141">64</span><span class="sxs-lookup"><span data-stu-id="ddf5e-141">64</span></span>|<span data-ttu-id="ddf5e-142">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="ddf5e-142">The device is managed by Google's CloudDPC.</span></span>|




