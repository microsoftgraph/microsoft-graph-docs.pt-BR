---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf8a40b8d6951c13da49766430fdd7fb303cbba0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775300"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="d6e0f-103">tipo de enumeração managementAgentType</span><span class="sxs-lookup"><span data-stu-id="d6e0f-103">managementAgentType enum type</span></span>

> <span data-ttu-id="d6e0f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6e0f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6e0f-106">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="d6e0f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d6e0f-107">Members</span></span>
|<span data-ttu-id="d6e0f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d6e0f-108">Member</span></span>|<span data-ttu-id="d6e0f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d6e0f-109">Value</span></span>|<span data-ttu-id="d6e0f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6e0f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6e0f-111">Estendi</span><span class="sxs-lookup"><span data-stu-id="d6e0f-111">eas</span></span>|<span data-ttu-id="d6e0f-112">1</span><span class="sxs-lookup"><span data-stu-id="d6e0f-112">1</span></span>|<span data-ttu-id="d6e0f-113">O dispositivo é gerenciado pelo Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="d6e0f-114">MDM</span><span class="sxs-lookup"><span data-stu-id="d6e0f-114">mdm</span></span>|<span data-ttu-id="d6e0f-115">duas</span><span class="sxs-lookup"><span data-stu-id="d6e0f-115">2</span></span>|<span data-ttu-id="d6e0f-116">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="d6e0f-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="d6e0f-117">easMdm</span></span>|<span data-ttu-id="d6e0f-118">3D</span><span class="sxs-lookup"><span data-stu-id="d6e0f-118">3</span></span>|<span data-ttu-id="d6e0f-119">O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="d6e0f-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="d6e0f-120">intuneClient</span></span>|<span data-ttu-id="d6e0f-121">quatro</span><span class="sxs-lookup"><span data-stu-id="d6e0f-121">4</span></span>|<span data-ttu-id="d6e0f-122">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-122">Intune client managed.</span></span>|
|<span data-ttu-id="d6e0f-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="d6e0f-123">easIntuneClient</span></span>|<span data-ttu-id="d6e0f-124">0,5</span><span class="sxs-lookup"><span data-stu-id="d6e0f-124">5</span></span>|<span data-ttu-id="d6e0f-125">O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="d6e0f-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="d6e0f-126">configurationManagerClient</span></span>|<span data-ttu-id="d6e0f-127">8</span><span class="sxs-lookup"><span data-stu-id="d6e0f-127">8</span></span>|<span data-ttu-id="d6e0f-128">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="d6e0f-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="d6e0f-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="d6e0f-130">254</span><span class="sxs-lookup"><span data-stu-id="d6e0f-130">10</span></span>|<span data-ttu-id="d6e0f-131">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="d6e0f-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="d6e0f-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="d6e0f-133">11</span><span class="sxs-lookup"><span data-stu-id="d6e0f-133">11</span></span>|<span data-ttu-id="d6e0f-134">O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="d6e0f-135">desconhecido</span><span class="sxs-lookup"><span data-stu-id="d6e0f-135">unknown</span></span>|<span data-ttu-id="d6e0f-136">dezesseis</span><span class="sxs-lookup"><span data-stu-id="d6e0f-136">16</span></span>|<span data-ttu-id="d6e0f-137">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="d6e0f-138">JAMF</span><span class="sxs-lookup"><span data-stu-id="d6e0f-138">jamf</span></span>|<span data-ttu-id="d6e0f-139">32</span><span class="sxs-lookup"><span data-stu-id="d6e0f-139">32</span></span>|<span data-ttu-id="d6e0f-140">Os atributos do dispositivo são buscados do JAMF.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="d6e0f-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="d6e0f-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="d6e0f-142">64</span><span class="sxs-lookup"><span data-stu-id="d6e0f-142">64</span></span>|<span data-ttu-id="d6e0f-143">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-143">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="d6e0f-144">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="d6e0f-144">microsoft365ManagedMdm</span></span>|<span data-ttu-id="d6e0f-145">258</span><span class="sxs-lookup"><span data-stu-id="d6e0f-145">258</span></span>|<span data-ttu-id="d6e0f-146">Este dispositivo é gerenciado pelo Microsoft 365 por meio do Intune.</span><span class="sxs-lookup"><span data-stu-id="d6e0f-146">This device is managed by Microsoft 365 through Intune.</span></span>|





