---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf8a40b8d6951c13da49766430fdd7fb303cbba0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521296"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="9ed58-103">tipo de enumeração managementAgentType</span><span class="sxs-lookup"><span data-stu-id="9ed58-103">managementAgentType enum type</span></span>

> <span data-ttu-id="9ed58-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ed58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ed58-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ed58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ed58-106">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="9ed58-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="9ed58-107">Membros</span><span class="sxs-lookup"><span data-stu-id="9ed58-107">Members</span></span>
|<span data-ttu-id="9ed58-108">Membro</span><span class="sxs-lookup"><span data-stu-id="9ed58-108">Member</span></span>|<span data-ttu-id="9ed58-109">Valor</span><span class="sxs-lookup"><span data-stu-id="9ed58-109">Value</span></span>|<span data-ttu-id="9ed58-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ed58-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ed58-111">Estendi</span><span class="sxs-lookup"><span data-stu-id="9ed58-111">eas</span></span>|<span data-ttu-id="9ed58-112">1 </span><span class="sxs-lookup"><span data-stu-id="9ed58-112">1</span></span>|<span data-ttu-id="9ed58-113">O dispositivo é gerenciado pelo Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="9ed58-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="9ed58-114">MDM</span><span class="sxs-lookup"><span data-stu-id="9ed58-114">mdm</span></span>|<span data-ttu-id="9ed58-115">2 </span><span class="sxs-lookup"><span data-stu-id="9ed58-115">2</span></span>|<span data-ttu-id="9ed58-116">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="9ed58-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="9ed58-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="9ed58-117">easMdm</span></span>|<span data-ttu-id="9ed58-118">3 </span><span class="sxs-lookup"><span data-stu-id="9ed58-118">3</span></span>|<span data-ttu-id="9ed58-119">O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="9ed58-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="9ed58-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="9ed58-120">intuneClient</span></span>|<span data-ttu-id="9ed58-121">4 </span><span class="sxs-lookup"><span data-stu-id="9ed58-121">4</span></span>|<span data-ttu-id="9ed58-122">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="9ed58-122">Intune client managed.</span></span>|
|<span data-ttu-id="9ed58-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="9ed58-123">easIntuneClient</span></span>|<span data-ttu-id="9ed58-124">5 </span><span class="sxs-lookup"><span data-stu-id="9ed58-124">5</span></span>|<span data-ttu-id="9ed58-125">O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.</span><span class="sxs-lookup"><span data-stu-id="9ed58-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="9ed58-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="9ed58-126">configurationManagerClient</span></span>|<span data-ttu-id="9ed58-127">8 </span><span class="sxs-lookup"><span data-stu-id="9ed58-127">8</span></span>|<span data-ttu-id="9ed58-128">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="9ed58-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="9ed58-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="9ed58-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="9ed58-130">10 </span><span class="sxs-lookup"><span data-stu-id="9ed58-130">10</span></span>|<span data-ttu-id="9ed58-131">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="9ed58-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="9ed58-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="9ed58-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="9ed58-133">11 </span><span class="sxs-lookup"><span data-stu-id="9ed58-133">11</span></span>|<span data-ttu-id="9ed58-134">O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.</span><span class="sxs-lookup"><span data-stu-id="9ed58-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="9ed58-135">desconhecido</span><span class="sxs-lookup"><span data-stu-id="9ed58-135">unknown</span></span>|<span data-ttu-id="9ed58-136">16 </span><span class="sxs-lookup"><span data-stu-id="9ed58-136">16</span></span>|<span data-ttu-id="9ed58-137">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="9ed58-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="9ed58-138">JAMF</span><span class="sxs-lookup"><span data-stu-id="9ed58-138">jamf</span></span>|<span data-ttu-id="9ed58-139">32</span><span class="sxs-lookup"><span data-stu-id="9ed58-139">32</span></span>|<span data-ttu-id="9ed58-140">Os atributos do dispositivo são buscados do JAMF.</span><span class="sxs-lookup"><span data-stu-id="9ed58-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="9ed58-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="9ed58-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="9ed58-142">64</span><span class="sxs-lookup"><span data-stu-id="9ed58-142">64</span></span>|<span data-ttu-id="9ed58-143">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="9ed58-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="9ed58-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="9ed58-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="9ed58-145">258</span><span class="sxs-lookup"><span data-stu-id="9ed58-145">258</span></span>|<span data-ttu-id="9ed58-146">Este dispositivo é gerenciado pelo Microsoft 365 por meio do Intune.</span><span class="sxs-lookup"><span data-stu-id="9ed58-146">This device is managed by Microsoft 365 through Intune.</span></span>|





