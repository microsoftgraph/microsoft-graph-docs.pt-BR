---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3b9fd469a787e0afdacb26dc5a07ee114d72bbe
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986120"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="081d1-103">tipo de enumeração managementAgentType</span><span class="sxs-lookup"><span data-stu-id="081d1-103">managementAgentType enum type</span></span>

> <span data-ttu-id="081d1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="081d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="081d1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="081d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="081d1-106">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="081d1-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="081d1-107">Membros</span><span class="sxs-lookup"><span data-stu-id="081d1-107">Members</span></span>
|<span data-ttu-id="081d1-108">Membro</span><span class="sxs-lookup"><span data-stu-id="081d1-108">Member</span></span>|<span data-ttu-id="081d1-109">Valor</span><span class="sxs-lookup"><span data-stu-id="081d1-109">Value</span></span>|<span data-ttu-id="081d1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="081d1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="081d1-111">Estendi</span><span class="sxs-lookup"><span data-stu-id="081d1-111">eas</span></span>|<span data-ttu-id="081d1-112">1</span><span class="sxs-lookup"><span data-stu-id="081d1-112">1</span></span>|<span data-ttu-id="081d1-113">O dispositivo é gerenciado pelo Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="081d1-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="081d1-114">MDM</span><span class="sxs-lookup"><span data-stu-id="081d1-114">mdm</span></span>|<span data-ttu-id="081d1-115">duas</span><span class="sxs-lookup"><span data-stu-id="081d1-115">2</span></span>|<span data-ttu-id="081d1-116">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="081d1-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="081d1-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="081d1-117">easMdm</span></span>|<span data-ttu-id="081d1-118">3D</span><span class="sxs-lookup"><span data-stu-id="081d1-118">3</span></span>|<span data-ttu-id="081d1-119">O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="081d1-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="081d1-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="081d1-120">intuneClient</span></span>|<span data-ttu-id="081d1-121">quatro</span><span class="sxs-lookup"><span data-stu-id="081d1-121">4</span></span>|<span data-ttu-id="081d1-122">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="081d1-122">Intune client managed.</span></span>|
|<span data-ttu-id="081d1-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="081d1-123">easIntuneClient</span></span>|<span data-ttu-id="081d1-124">0,5</span><span class="sxs-lookup"><span data-stu-id="081d1-124">5</span></span>|<span data-ttu-id="081d1-125">O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.</span><span class="sxs-lookup"><span data-stu-id="081d1-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="081d1-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="081d1-126">configurationManagerClient</span></span>|<span data-ttu-id="081d1-127">8 </span><span class="sxs-lookup"><span data-stu-id="081d1-127">8</span></span>|<span data-ttu-id="081d1-128">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="081d1-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="081d1-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="081d1-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="081d1-130">10 </span><span class="sxs-lookup"><span data-stu-id="081d1-130">10</span></span>|<span data-ttu-id="081d1-131">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="081d1-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="081d1-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="081d1-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="081d1-133">11</span><span class="sxs-lookup"><span data-stu-id="081d1-133">11</span></span>|<span data-ttu-id="081d1-134">O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.</span><span class="sxs-lookup"><span data-stu-id="081d1-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="081d1-135">desconhecido</span><span class="sxs-lookup"><span data-stu-id="081d1-135">unknown</span></span>|<span data-ttu-id="081d1-136">dezesseis</span><span class="sxs-lookup"><span data-stu-id="081d1-136">16</span></span>|<span data-ttu-id="081d1-137">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="081d1-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="081d1-138">jamf</span><span class="sxs-lookup"><span data-stu-id="081d1-138">jamf</span></span>|<span data-ttu-id="081d1-139">32</span><span class="sxs-lookup"><span data-stu-id="081d1-139">32</span></span>|<span data-ttu-id="081d1-140">Os atributos do dispositivo são buscados do JAMF.</span><span class="sxs-lookup"><span data-stu-id="081d1-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="081d1-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="081d1-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="081d1-142">64</span><span class="sxs-lookup"><span data-stu-id="081d1-142">64</span></span>|<span data-ttu-id="081d1-143">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="081d1-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="081d1-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="081d1-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="081d1-145">258</span><span class="sxs-lookup"><span data-stu-id="081d1-145">258</span></span>|<span data-ttu-id="081d1-146">Este dispositivo é gerenciado pelo Microsoft 365 por meio do Intune.</span><span class="sxs-lookup"><span data-stu-id="081d1-146">This device is managed by Microsoft 365 through Intune.</span></span>|





