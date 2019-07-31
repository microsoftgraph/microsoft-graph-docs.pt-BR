---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ae96113e687d406f5c0342b3b71fd63ea6de9918
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999749"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="99823-103">tipo de enumeração managementAgentType</span><span class="sxs-lookup"><span data-stu-id="99823-103">managementAgentType enum type</span></span>

> <span data-ttu-id="99823-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99823-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99823-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99823-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99823-106">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="99823-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="99823-107">Membros</span><span class="sxs-lookup"><span data-stu-id="99823-107">Members</span></span>
|<span data-ttu-id="99823-108">Membro</span><span class="sxs-lookup"><span data-stu-id="99823-108">Member</span></span>|<span data-ttu-id="99823-109">Valor</span><span class="sxs-lookup"><span data-stu-id="99823-109">Value</span></span>|<span data-ttu-id="99823-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="99823-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99823-111">Estendi</span><span class="sxs-lookup"><span data-stu-id="99823-111">eas</span></span>|<span data-ttu-id="99823-112">1</span><span class="sxs-lookup"><span data-stu-id="99823-112">1</span></span>|<span data-ttu-id="99823-113">O dispositivo é gerenciado pelo Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="99823-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="99823-114">MDM</span><span class="sxs-lookup"><span data-stu-id="99823-114">mdm</span></span>|<span data-ttu-id="99823-115">duas</span><span class="sxs-lookup"><span data-stu-id="99823-115">2</span></span>|<span data-ttu-id="99823-116">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="99823-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="99823-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="99823-117">easMdm</span></span>|<span data-ttu-id="99823-118">3D</span><span class="sxs-lookup"><span data-stu-id="99823-118">3</span></span>|<span data-ttu-id="99823-119">O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="99823-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="99823-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="99823-120">intuneClient</span></span>|<span data-ttu-id="99823-121">quatro</span><span class="sxs-lookup"><span data-stu-id="99823-121">4</span></span>|<span data-ttu-id="99823-122">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="99823-122">Intune client managed.</span></span>|
|<span data-ttu-id="99823-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="99823-123">easIntuneClient</span></span>|<span data-ttu-id="99823-124">0,5</span><span class="sxs-lookup"><span data-stu-id="99823-124">5</span></span>|<span data-ttu-id="99823-125">O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.</span><span class="sxs-lookup"><span data-stu-id="99823-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="99823-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="99823-126">configurationManagerClient</span></span>|<span data-ttu-id="99823-127">8 </span><span class="sxs-lookup"><span data-stu-id="99823-127">8</span></span>|<span data-ttu-id="99823-128">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="99823-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="99823-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="99823-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="99823-130">10 </span><span class="sxs-lookup"><span data-stu-id="99823-130">10</span></span>|<span data-ttu-id="99823-131">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="99823-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="99823-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="99823-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="99823-133">11</span><span class="sxs-lookup"><span data-stu-id="99823-133">11</span></span>|<span data-ttu-id="99823-134">O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.</span><span class="sxs-lookup"><span data-stu-id="99823-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="99823-135">desconhecido</span><span class="sxs-lookup"><span data-stu-id="99823-135">unknown</span></span>|<span data-ttu-id="99823-136">dezesseis</span><span class="sxs-lookup"><span data-stu-id="99823-136">16</span></span>|<span data-ttu-id="99823-137">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="99823-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="99823-138">jamf</span><span class="sxs-lookup"><span data-stu-id="99823-138">jamf</span></span>|<span data-ttu-id="99823-139">32</span><span class="sxs-lookup"><span data-stu-id="99823-139">32</span></span>|<span data-ttu-id="99823-140">Os atributos do dispositivo são buscados do JAMF.</span><span class="sxs-lookup"><span data-stu-id="99823-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="99823-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="99823-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="99823-142">64</span><span class="sxs-lookup"><span data-stu-id="99823-142">64</span></span>|<span data-ttu-id="99823-143">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="99823-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="99823-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="99823-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="99823-145">258</span><span class="sxs-lookup"><span data-stu-id="99823-145">258</span></span>|<span data-ttu-id="99823-146">Este dispositivo é gerenciado pelo Microsoft 365 por meio do Intune.</span><span class="sxs-lookup"><span data-stu-id="99823-146">This device is managed by Microsoft 365 through Intune.</span></span>|





