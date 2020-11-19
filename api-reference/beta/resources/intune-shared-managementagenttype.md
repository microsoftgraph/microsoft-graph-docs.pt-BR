---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 282915b085107d5367a0b7f8bd8f4f3ea84b7c23
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49258938"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="ddb6c-103">tipo de enumeração managementAgentType</span><span class="sxs-lookup"><span data-stu-id="ddb6c-103">managementAgentType enum type</span></span>

<span data-ttu-id="ddb6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddb6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddb6c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddb6c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddb6c-107">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="ddb6c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="ddb6c-108">Members</span></span>
|<span data-ttu-id="ddb6c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="ddb6c-109">Member</span></span>|<span data-ttu-id="ddb6c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="ddb6c-110">Value</span></span>|<span data-ttu-id="ddb6c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddb6c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddb6c-112">Estendi</span><span class="sxs-lookup"><span data-stu-id="ddb6c-112">eas</span></span>|<span data-ttu-id="ddb6c-113">1</span><span class="sxs-lookup"><span data-stu-id="ddb6c-113">1</span></span>|<span data-ttu-id="ddb6c-114">O dispositivo é gerenciado pelo Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="ddb6c-115">MDM</span><span class="sxs-lookup"><span data-stu-id="ddb6c-115">mdm</span></span>|<span data-ttu-id="ddb6c-116">duas</span><span class="sxs-lookup"><span data-stu-id="ddb6c-116">2</span></span>|<span data-ttu-id="ddb6c-117">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="ddb6c-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="ddb6c-118">easMdm</span></span>|<span data-ttu-id="ddb6c-119">3D</span><span class="sxs-lookup"><span data-stu-id="ddb6c-119">3</span></span>|<span data-ttu-id="ddb6c-120">O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="ddb6c-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="ddb6c-121">intuneClient</span></span>|<span data-ttu-id="ddb6c-122">4 </span><span class="sxs-lookup"><span data-stu-id="ddb6c-122">4</span></span>|<span data-ttu-id="ddb6c-123">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-123">Intune client managed.</span></span>|
|<span data-ttu-id="ddb6c-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="ddb6c-124">easIntuneClient</span></span>|<span data-ttu-id="ddb6c-125">5 </span><span class="sxs-lookup"><span data-stu-id="ddb6c-125">5</span></span>|<span data-ttu-id="ddb6c-126">O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="ddb6c-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="ddb6c-127">configurationManagerClient</span></span>|<span data-ttu-id="ddb6c-128">8 </span><span class="sxs-lookup"><span data-stu-id="ddb6c-128">8</span></span>|<span data-ttu-id="ddb6c-129">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="ddb6c-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="ddb6c-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="ddb6c-131">10 </span><span class="sxs-lookup"><span data-stu-id="ddb6c-131">10</span></span>|<span data-ttu-id="ddb6c-132">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="ddb6c-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="ddb6c-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="ddb6c-134">11 </span><span class="sxs-lookup"><span data-stu-id="ddb6c-134">11</span></span>|<span data-ttu-id="ddb6c-135">O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="ddb6c-136">desconhecido</span><span class="sxs-lookup"><span data-stu-id="ddb6c-136">unknown</span></span>|<span data-ttu-id="ddb6c-137">16 </span><span class="sxs-lookup"><span data-stu-id="ddb6c-137">16</span></span>|<span data-ttu-id="ddb6c-138">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="ddb6c-139">jamf</span><span class="sxs-lookup"><span data-stu-id="ddb6c-139">jamf</span></span>|<span data-ttu-id="ddb6c-140">32</span><span class="sxs-lookup"><span data-stu-id="ddb6c-140">32</span></span>|<span data-ttu-id="ddb6c-141">Os atributos do dispositivo são buscados do JAMF.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="ddb6c-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="ddb6c-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="ddb6c-143">64</span><span class="sxs-lookup"><span data-stu-id="ddb6c-143">64</span></span>|<span data-ttu-id="ddb6c-144">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="ddb6c-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="ddb6c-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="ddb6c-146">258</span><span class="sxs-lookup"><span data-stu-id="ddb6c-146">258</span></span>|<span data-ttu-id="ddb6c-147">Este dispositivo é gerenciado pelo Microsoft 365 por meio do Intune.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-147">This device is managed by Microsoft 365 through Intune.</span></span>|
|<span data-ttu-id="ddb6c-148">windowsManagementCloudApi</span><span class="sxs-lookup"><span data-stu-id="ddb6c-148">windowsManagementCloudApi</span></span>|<span data-ttu-id="ddb6c-149">512</span><span class="sxs-lookup"><span data-stu-id="ddb6c-149">512</span></span>|<span data-ttu-id="ddb6c-150">Este dispositivo é gerenciado pela API de nuvem de gerenciamento do Windows.</span><span class="sxs-lookup"><span data-stu-id="ddb6c-150">This device is managed by Windows Management Cloud API.</span></span>|




