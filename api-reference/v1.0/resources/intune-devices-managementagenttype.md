---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d5f698a2878b0662193128044d7b069c8dfe8b3f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406830"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="2b852-103">tipo de enumeração managementAgentType</span><span class="sxs-lookup"><span data-stu-id="2b852-103">managementAgentType enum type</span></span>

<span data-ttu-id="2b852-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b852-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b852-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b852-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b852-106">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="2b852-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="2b852-107">Membros</span><span class="sxs-lookup"><span data-stu-id="2b852-107">Members</span></span>
|<span data-ttu-id="2b852-108">Membro</span><span class="sxs-lookup"><span data-stu-id="2b852-108">Member</span></span>|<span data-ttu-id="2b852-109">Valor</span><span class="sxs-lookup"><span data-stu-id="2b852-109">Value</span></span>|<span data-ttu-id="2b852-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b852-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b852-111">Estendi</span><span class="sxs-lookup"><span data-stu-id="2b852-111">eas</span></span>|<span data-ttu-id="2b852-112">1</span><span class="sxs-lookup"><span data-stu-id="2b852-112">1</span></span>|<span data-ttu-id="2b852-113">O dispositivo é gerenciado pelo Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="2b852-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="2b852-114">MDM</span><span class="sxs-lookup"><span data-stu-id="2b852-114">mdm</span></span>|<span data-ttu-id="2b852-115">duas</span><span class="sxs-lookup"><span data-stu-id="2b852-115">2</span></span>|<span data-ttu-id="2b852-116">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="2b852-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="2b852-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="2b852-117">easMdm</span></span>|<span data-ttu-id="2b852-118">3D</span><span class="sxs-lookup"><span data-stu-id="2b852-118">3</span></span>|<span data-ttu-id="2b852-119">O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="2b852-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="2b852-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="2b852-120">intuneClient</span></span>|<span data-ttu-id="2b852-121">4 </span><span class="sxs-lookup"><span data-stu-id="2b852-121">4</span></span>|<span data-ttu-id="2b852-122">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="2b852-122">Intune client managed.</span></span>|
|<span data-ttu-id="2b852-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="2b852-123">easIntuneClient</span></span>|<span data-ttu-id="2b852-124">5 </span><span class="sxs-lookup"><span data-stu-id="2b852-124">5</span></span>|<span data-ttu-id="2b852-125">O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.</span><span class="sxs-lookup"><span data-stu-id="2b852-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="2b852-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="2b852-126">configurationManagerClient</span></span>|<span data-ttu-id="2b852-127">8 </span><span class="sxs-lookup"><span data-stu-id="2b852-127">8</span></span>|<span data-ttu-id="2b852-128">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="2b852-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="2b852-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="2b852-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="2b852-130">10 </span><span class="sxs-lookup"><span data-stu-id="2b852-130">10</span></span>|<span data-ttu-id="2b852-131">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="2b852-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="2b852-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="2b852-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="2b852-133">11</span><span class="sxs-lookup"><span data-stu-id="2b852-133">11</span></span>|<span data-ttu-id="2b852-134">O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.</span><span class="sxs-lookup"><span data-stu-id="2b852-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="2b852-135">desconhecido</span><span class="sxs-lookup"><span data-stu-id="2b852-135">unknown</span></span>|<span data-ttu-id="2b852-136">16 </span><span class="sxs-lookup"><span data-stu-id="2b852-136">16</span></span>|<span data-ttu-id="2b852-137">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="2b852-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="2b852-138">jamf</span><span class="sxs-lookup"><span data-stu-id="2b852-138">jamf</span></span>|<span data-ttu-id="2b852-139">32</span><span class="sxs-lookup"><span data-stu-id="2b852-139">32</span></span>|<span data-ttu-id="2b852-140">Os atributos do dispositivo são buscados do JAMF.</span><span class="sxs-lookup"><span data-stu-id="2b852-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="2b852-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="2b852-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="2b852-142">64</span><span class="sxs-lookup"><span data-stu-id="2b852-142">64</span></span>|<span data-ttu-id="2b852-143">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="2b852-143">The device is managed by Google's CloudDPC.</span></span>|







