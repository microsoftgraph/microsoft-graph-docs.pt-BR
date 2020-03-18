---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e6b10c92a2c09505d1e3c5031f1d9046cfa56cb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769007"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="b9f93-103">tipo de enumeração managementAgentType</span><span class="sxs-lookup"><span data-stu-id="b9f93-103">managementAgentType enum type</span></span>

> <span data-ttu-id="b9f93-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9f93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9f93-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9f93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9f93-106">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b9f93-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="b9f93-107">Membros</span><span class="sxs-lookup"><span data-stu-id="b9f93-107">Members</span></span>
|<span data-ttu-id="b9f93-108">Membro</span><span class="sxs-lookup"><span data-stu-id="b9f93-108">Member</span></span>|<span data-ttu-id="b9f93-109">Valor</span><span class="sxs-lookup"><span data-stu-id="b9f93-109">Value</span></span>|<span data-ttu-id="b9f93-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9f93-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9f93-111">Estendi</span><span class="sxs-lookup"><span data-stu-id="b9f93-111">eas</span></span>|<span data-ttu-id="b9f93-112">1</span><span class="sxs-lookup"><span data-stu-id="b9f93-112">1</span></span>|<span data-ttu-id="b9f93-113">O dispositivo é gerenciado pelo Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="b9f93-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="b9f93-114">MDM</span><span class="sxs-lookup"><span data-stu-id="b9f93-114">mdm</span></span>|<span data-ttu-id="b9f93-115">duas</span><span class="sxs-lookup"><span data-stu-id="b9f93-115">2</span></span>|<span data-ttu-id="b9f93-116">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="b9f93-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="b9f93-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="b9f93-117">easMdm</span></span>|<span data-ttu-id="b9f93-118">3D</span><span class="sxs-lookup"><span data-stu-id="b9f93-118">3</span></span>|<span data-ttu-id="b9f93-119">O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="b9f93-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="b9f93-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="b9f93-120">intuneClient</span></span>|<span data-ttu-id="b9f93-121">4 </span><span class="sxs-lookup"><span data-stu-id="b9f93-121">4</span></span>|<span data-ttu-id="b9f93-122">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="b9f93-122">Intune client managed.</span></span>|
|<span data-ttu-id="b9f93-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="b9f93-123">easIntuneClient</span></span>|<span data-ttu-id="b9f93-124">5 </span><span class="sxs-lookup"><span data-stu-id="b9f93-124">5</span></span>|<span data-ttu-id="b9f93-125">O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.</span><span class="sxs-lookup"><span data-stu-id="b9f93-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="b9f93-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="b9f93-126">configurationManagerClient</span></span>|<span data-ttu-id="b9f93-127">8 </span><span class="sxs-lookup"><span data-stu-id="b9f93-127">8</span></span>|<span data-ttu-id="b9f93-128">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="b9f93-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="b9f93-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="b9f93-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="b9f93-130">10 </span><span class="sxs-lookup"><span data-stu-id="b9f93-130">10</span></span>|<span data-ttu-id="b9f93-131">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="b9f93-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="b9f93-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="b9f93-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="b9f93-133">11</span><span class="sxs-lookup"><span data-stu-id="b9f93-133">11</span></span>|<span data-ttu-id="b9f93-134">O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.</span><span class="sxs-lookup"><span data-stu-id="b9f93-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="b9f93-135">desconhecido</span><span class="sxs-lookup"><span data-stu-id="b9f93-135">unknown</span></span>|<span data-ttu-id="b9f93-136">16 </span><span class="sxs-lookup"><span data-stu-id="b9f93-136">16</span></span>|<span data-ttu-id="b9f93-137">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="b9f93-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="b9f93-138">jamf</span><span class="sxs-lookup"><span data-stu-id="b9f93-138">jamf</span></span>|<span data-ttu-id="b9f93-139">32</span><span class="sxs-lookup"><span data-stu-id="b9f93-139">32</span></span>|<span data-ttu-id="b9f93-140">Os atributos do dispositivo são buscados do JAMF.</span><span class="sxs-lookup"><span data-stu-id="b9f93-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="b9f93-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="b9f93-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="b9f93-142">64</span><span class="sxs-lookup"><span data-stu-id="b9f93-142">64</span></span>|<span data-ttu-id="b9f93-143">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="b9f93-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="b9f93-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="b9f93-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="b9f93-145">258</span><span class="sxs-lookup"><span data-stu-id="b9f93-145">258</span></span>|<span data-ttu-id="b9f93-146">Este dispositivo é gerenciado pelo Microsoft 365 por meio do Intune.</span><span class="sxs-lookup"><span data-stu-id="b9f93-146">This device is managed by Microsoft 365 through Intune.</span></span>|
|<span data-ttu-id="b9f93-147">windowsManagementCloudApi</span><span class="sxs-lookup"><span data-stu-id="b9f93-147">windowsManagementCloudApi</span></span>|<span data-ttu-id="b9f93-148">512</span><span class="sxs-lookup"><span data-stu-id="b9f93-148">512</span></span>|<span data-ttu-id="b9f93-149">Este dispositivo é gerenciado pela API de nuvem de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="b9f93-149">This device is managed by Windows Management Cloud API.</span></span>|



