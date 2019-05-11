---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7bb3c564366e2fa5c4be2c7c7ed75267a4d58275
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941923"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="82eed-103">tipo de enumeração managementAgentType</span><span class="sxs-lookup"><span data-stu-id="82eed-103">managementAgentType enum type</span></span>

> <span data-ttu-id="82eed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="82eed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82eed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82eed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82eed-106">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="82eed-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="82eed-107">Membros</span><span class="sxs-lookup"><span data-stu-id="82eed-107">Members</span></span>
|<span data-ttu-id="82eed-108">Membro</span><span class="sxs-lookup"><span data-stu-id="82eed-108">Member</span></span>|<span data-ttu-id="82eed-109">Valor</span><span class="sxs-lookup"><span data-stu-id="82eed-109">Value</span></span>|<span data-ttu-id="82eed-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="82eed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82eed-111">Estendi</span><span class="sxs-lookup"><span data-stu-id="82eed-111">eas</span></span>|<span data-ttu-id="82eed-112">1</span><span class="sxs-lookup"><span data-stu-id="82eed-112">1</span></span>|<span data-ttu-id="82eed-113">O dispositivo é gerenciado pelo Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="82eed-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="82eed-114">MDM</span><span class="sxs-lookup"><span data-stu-id="82eed-114">mdm</span></span>|<span data-ttu-id="82eed-115">duas</span><span class="sxs-lookup"><span data-stu-id="82eed-115">2</span></span>|<span data-ttu-id="82eed-116">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="82eed-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="82eed-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="82eed-117">easMdm</span></span>|<span data-ttu-id="82eed-118">3D</span><span class="sxs-lookup"><span data-stu-id="82eed-118">3</span></span>|<span data-ttu-id="82eed-119">O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="82eed-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="82eed-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="82eed-120">intuneClient</span></span>|<span data-ttu-id="82eed-121">quatro</span><span class="sxs-lookup"><span data-stu-id="82eed-121">4</span></span>|<span data-ttu-id="82eed-122">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="82eed-122">Intune client managed.</span></span>|
|<span data-ttu-id="82eed-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="82eed-123">easIntuneClient</span></span>|<span data-ttu-id="82eed-124">0,5</span><span class="sxs-lookup"><span data-stu-id="82eed-124">5</span></span>|<span data-ttu-id="82eed-125">O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.</span><span class="sxs-lookup"><span data-stu-id="82eed-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="82eed-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="82eed-126">configurationManagerClient</span></span>|<span data-ttu-id="82eed-127">8 </span><span class="sxs-lookup"><span data-stu-id="82eed-127">8</span></span>|<span data-ttu-id="82eed-128">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="82eed-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="82eed-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="82eed-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="82eed-130">10 </span><span class="sxs-lookup"><span data-stu-id="82eed-130">10</span></span>|<span data-ttu-id="82eed-131">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="82eed-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="82eed-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="82eed-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="82eed-133">11</span><span class="sxs-lookup"><span data-stu-id="82eed-133">11</span></span>|<span data-ttu-id="82eed-134">O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.</span><span class="sxs-lookup"><span data-stu-id="82eed-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="82eed-135">desconhecido</span><span class="sxs-lookup"><span data-stu-id="82eed-135">unknown</span></span>|<span data-ttu-id="82eed-136">dezesseis</span><span class="sxs-lookup"><span data-stu-id="82eed-136">16</span></span>|<span data-ttu-id="82eed-137">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="82eed-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="82eed-138">jamf</span><span class="sxs-lookup"><span data-stu-id="82eed-138">jamf</span></span>|<span data-ttu-id="82eed-139">32</span><span class="sxs-lookup"><span data-stu-id="82eed-139">32</span></span>|<span data-ttu-id="82eed-140">Os atributos do dispositivo são buscados do JAMF.</span><span class="sxs-lookup"><span data-stu-id="82eed-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="82eed-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="82eed-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="82eed-142">64</span><span class="sxs-lookup"><span data-stu-id="82eed-142">64</span></span>|<span data-ttu-id="82eed-143">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="82eed-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="82eed-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="82eed-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="82eed-145">258</span><span class="sxs-lookup"><span data-stu-id="82eed-145">258</span></span>|<span data-ttu-id="82eed-146">Este dispositivo é gerenciado pelo Microsoft 365 por meio do Intune.</span><span class="sxs-lookup"><span data-stu-id="82eed-146">This device is managed by Microsoft 365 through Intune.</span></span>|




