---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e769cd3f270a8ca1d00b6272a90154b925cc771d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48681954"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="91fe4-103">tipo de enumeração managementAgentType</span><span class="sxs-lookup"><span data-stu-id="91fe4-103">managementAgentType enum type</span></span>

<span data-ttu-id="91fe4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91fe4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91fe4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91fe4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91fe4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91fe4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91fe4-107">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="91fe4-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="91fe4-108">Membros</span><span class="sxs-lookup"><span data-stu-id="91fe4-108">Members</span></span>
|<span data-ttu-id="91fe4-109">Membro</span><span class="sxs-lookup"><span data-stu-id="91fe4-109">Member</span></span>|<span data-ttu-id="91fe4-110">Valor</span><span class="sxs-lookup"><span data-stu-id="91fe4-110">Value</span></span>|<span data-ttu-id="91fe4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="91fe4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91fe4-112">Estendi</span><span class="sxs-lookup"><span data-stu-id="91fe4-112">eas</span></span>|<span data-ttu-id="91fe4-113">1</span><span class="sxs-lookup"><span data-stu-id="91fe4-113">1</span></span>|<span data-ttu-id="91fe4-114">O dispositivo é gerenciado pelo Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="91fe4-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="91fe4-115">MDM</span><span class="sxs-lookup"><span data-stu-id="91fe4-115">mdm</span></span>|<span data-ttu-id="91fe4-116">duas</span><span class="sxs-lookup"><span data-stu-id="91fe4-116">2</span></span>|<span data-ttu-id="91fe4-117">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="91fe4-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="91fe4-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="91fe4-118">easMdm</span></span>|<span data-ttu-id="91fe4-119">3D</span><span class="sxs-lookup"><span data-stu-id="91fe4-119">3</span></span>|<span data-ttu-id="91fe4-120">O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="91fe4-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="91fe4-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="91fe4-121">intuneClient</span></span>|<span data-ttu-id="91fe4-122">4 </span><span class="sxs-lookup"><span data-stu-id="91fe4-122">4</span></span>|<span data-ttu-id="91fe4-123">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="91fe4-123">Intune client managed.</span></span>|
|<span data-ttu-id="91fe4-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="91fe4-124">easIntuneClient</span></span>|<span data-ttu-id="91fe4-125">5 </span><span class="sxs-lookup"><span data-stu-id="91fe4-125">5</span></span>|<span data-ttu-id="91fe4-126">O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.</span><span class="sxs-lookup"><span data-stu-id="91fe4-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="91fe4-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="91fe4-127">configurationManagerClient</span></span>|<span data-ttu-id="91fe4-128">8 </span><span class="sxs-lookup"><span data-stu-id="91fe4-128">8</span></span>|<span data-ttu-id="91fe4-129">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="91fe4-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="91fe4-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="91fe4-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="91fe4-131">10 </span><span class="sxs-lookup"><span data-stu-id="91fe4-131">10</span></span>|<span data-ttu-id="91fe4-132">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="91fe4-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="91fe4-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="91fe4-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="91fe4-134">11</span><span class="sxs-lookup"><span data-stu-id="91fe4-134">11</span></span>|<span data-ttu-id="91fe4-135">O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.</span><span class="sxs-lookup"><span data-stu-id="91fe4-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="91fe4-136">desconhecido</span><span class="sxs-lookup"><span data-stu-id="91fe4-136">unknown</span></span>|<span data-ttu-id="91fe4-137">16 </span><span class="sxs-lookup"><span data-stu-id="91fe4-137">16</span></span>|<span data-ttu-id="91fe4-138">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="91fe4-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="91fe4-139">jamf</span><span class="sxs-lookup"><span data-stu-id="91fe4-139">jamf</span></span>|<span data-ttu-id="91fe4-140">32</span><span class="sxs-lookup"><span data-stu-id="91fe4-140">32</span></span>|<span data-ttu-id="91fe4-141">Os atributos do dispositivo são buscados do JAMF.</span><span class="sxs-lookup"><span data-stu-id="91fe4-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="91fe4-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="91fe4-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="91fe4-143">64</span><span class="sxs-lookup"><span data-stu-id="91fe4-143">64</span></span>|<span data-ttu-id="91fe4-144">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="91fe4-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="91fe4-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="91fe4-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="91fe4-146">258</span><span class="sxs-lookup"><span data-stu-id="91fe4-146">258</span></span>|<span data-ttu-id="91fe4-147">Este dispositivo é gerenciado pelo Microsoft 365 por meio do Intune.</span><span class="sxs-lookup"><span data-stu-id="91fe4-147">This device is managed by Microsoft 365 through Intune.</span></span>|
|<span data-ttu-id="91fe4-148">windowsManagementCloudApi</span><span class="sxs-lookup"><span data-stu-id="91fe4-148">windowsManagementCloudApi</span></span>|<span data-ttu-id="91fe4-149">512</span><span class="sxs-lookup"><span data-stu-id="91fe4-149">512</span></span>|<span data-ttu-id="91fe4-150">Este dispositivo é gerenciado pela API de nuvem de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="91fe4-150">This device is managed by Windows Management Cloud API.</span></span>|





