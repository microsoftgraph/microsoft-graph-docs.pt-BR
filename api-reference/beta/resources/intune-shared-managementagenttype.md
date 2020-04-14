---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 34783f2c586e192d62cdeb0018b82e2df100c958
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466240"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="22524-103">tipo de enumeração managementAgentType</span><span class="sxs-lookup"><span data-stu-id="22524-103">managementAgentType enum type</span></span>

<span data-ttu-id="22524-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22524-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22524-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22524-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22524-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22524-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22524-107">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="22524-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="22524-108">Membros</span><span class="sxs-lookup"><span data-stu-id="22524-108">Members</span></span>
|<span data-ttu-id="22524-109">Membro</span><span class="sxs-lookup"><span data-stu-id="22524-109">Member</span></span>|<span data-ttu-id="22524-110">Valor</span><span class="sxs-lookup"><span data-stu-id="22524-110">Value</span></span>|<span data-ttu-id="22524-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="22524-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22524-112">Estendi</span><span class="sxs-lookup"><span data-stu-id="22524-112">eas</span></span>|<span data-ttu-id="22524-113">1</span><span class="sxs-lookup"><span data-stu-id="22524-113">1</span></span>|<span data-ttu-id="22524-114">O dispositivo é gerenciado pelo Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="22524-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="22524-115">MDM</span><span class="sxs-lookup"><span data-stu-id="22524-115">mdm</span></span>|<span data-ttu-id="22524-116">duas</span><span class="sxs-lookup"><span data-stu-id="22524-116">2</span></span>|<span data-ttu-id="22524-117">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="22524-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="22524-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="22524-118">easMdm</span></span>|<span data-ttu-id="22524-119">3D</span><span class="sxs-lookup"><span data-stu-id="22524-119">3</span></span>|<span data-ttu-id="22524-120">O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="22524-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="22524-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="22524-121">intuneClient</span></span>|<span data-ttu-id="22524-122">4 </span><span class="sxs-lookup"><span data-stu-id="22524-122">4</span></span>|<span data-ttu-id="22524-123">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="22524-123">Intune client managed.</span></span>|
|<span data-ttu-id="22524-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="22524-124">easIntuneClient</span></span>|<span data-ttu-id="22524-125">5 </span><span class="sxs-lookup"><span data-stu-id="22524-125">5</span></span>|<span data-ttu-id="22524-126">O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.</span><span class="sxs-lookup"><span data-stu-id="22524-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="22524-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="22524-127">configurationManagerClient</span></span>|<span data-ttu-id="22524-128">8 </span><span class="sxs-lookup"><span data-stu-id="22524-128">8</span></span>|<span data-ttu-id="22524-129">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="22524-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="22524-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="22524-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="22524-131">10 </span><span class="sxs-lookup"><span data-stu-id="22524-131">10</span></span>|<span data-ttu-id="22524-132">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="22524-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="22524-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="22524-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="22524-134">11</span><span class="sxs-lookup"><span data-stu-id="22524-134">11</span></span>|<span data-ttu-id="22524-135">O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.</span><span class="sxs-lookup"><span data-stu-id="22524-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="22524-136">desconhecido</span><span class="sxs-lookup"><span data-stu-id="22524-136">unknown</span></span>|<span data-ttu-id="22524-137">16 </span><span class="sxs-lookup"><span data-stu-id="22524-137">16</span></span>|<span data-ttu-id="22524-138">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="22524-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="22524-139">jamf</span><span class="sxs-lookup"><span data-stu-id="22524-139">jamf</span></span>|<span data-ttu-id="22524-140">32</span><span class="sxs-lookup"><span data-stu-id="22524-140">32</span></span>|<span data-ttu-id="22524-141">Os atributos do dispositivo são buscados do JAMF.</span><span class="sxs-lookup"><span data-stu-id="22524-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="22524-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="22524-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="22524-143">64</span><span class="sxs-lookup"><span data-stu-id="22524-143">64</span></span>|<span data-ttu-id="22524-144">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="22524-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="22524-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="22524-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="22524-146">258</span><span class="sxs-lookup"><span data-stu-id="22524-146">258</span></span>|<span data-ttu-id="22524-147">Este dispositivo é gerenciado pelo Microsoft 365 por meio do Intune.</span><span class="sxs-lookup"><span data-stu-id="22524-147">This device is managed by Microsoft 365 through Intune.</span></span>|
|<span data-ttu-id="22524-148">windowsManagementCloudApi</span><span class="sxs-lookup"><span data-stu-id="22524-148">windowsManagementCloudApi</span></span>|<span data-ttu-id="22524-149">512</span><span class="sxs-lookup"><span data-stu-id="22524-149">512</span></span>|<span data-ttu-id="22524-150">Este dispositivo é gerenciado pela API de nuvem de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="22524-150">This device is managed by Windows Management Cloud API.</span></span>|



