---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9a5835a0a8ca83cef2d5590679ce8aa4e77b0859
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530295"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="ef30a-103">tipo de enumeração managementAgentType</span><span class="sxs-lookup"><span data-stu-id="ef30a-103">managementAgentType enum type</span></span>

<span data-ttu-id="ef30a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef30a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef30a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef30a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef30a-106">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="ef30a-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="ef30a-107">Membros</span><span class="sxs-lookup"><span data-stu-id="ef30a-107">Members</span></span>
|<span data-ttu-id="ef30a-108">Membro</span><span class="sxs-lookup"><span data-stu-id="ef30a-108">Member</span></span>|<span data-ttu-id="ef30a-109">Valor</span><span class="sxs-lookup"><span data-stu-id="ef30a-109">Value</span></span>|<span data-ttu-id="ef30a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef30a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef30a-111">Estendi</span><span class="sxs-lookup"><span data-stu-id="ef30a-111">eas</span></span>|<span data-ttu-id="ef30a-112">1 </span><span class="sxs-lookup"><span data-stu-id="ef30a-112">1</span></span>|<span data-ttu-id="ef30a-113">O dispositivo é gerenciado pelo Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="ef30a-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="ef30a-114">MDM</span><span class="sxs-lookup"><span data-stu-id="ef30a-114">mdm</span></span>|<span data-ttu-id="ef30a-115">2 </span><span class="sxs-lookup"><span data-stu-id="ef30a-115">2</span></span>|<span data-ttu-id="ef30a-116">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="ef30a-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="ef30a-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="ef30a-117">easMdm</span></span>|<span data-ttu-id="ef30a-118">3 </span><span class="sxs-lookup"><span data-stu-id="ef30a-118">3</span></span>|<span data-ttu-id="ef30a-119">O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="ef30a-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="ef30a-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="ef30a-120">intuneClient</span></span>|<span data-ttu-id="ef30a-121">4 </span><span class="sxs-lookup"><span data-stu-id="ef30a-121">4</span></span>|<span data-ttu-id="ef30a-122">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="ef30a-122">Intune client managed.</span></span>|
|<span data-ttu-id="ef30a-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="ef30a-123">easIntuneClient</span></span>|<span data-ttu-id="ef30a-124">5 </span><span class="sxs-lookup"><span data-stu-id="ef30a-124">5</span></span>|<span data-ttu-id="ef30a-125">O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.</span><span class="sxs-lookup"><span data-stu-id="ef30a-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="ef30a-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="ef30a-126">configurationManagerClient</span></span>|<span data-ttu-id="ef30a-127">8 </span><span class="sxs-lookup"><span data-stu-id="ef30a-127">8</span></span>|<span data-ttu-id="ef30a-128">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="ef30a-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="ef30a-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="ef30a-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="ef30a-130">10 </span><span class="sxs-lookup"><span data-stu-id="ef30a-130">10</span></span>|<span data-ttu-id="ef30a-131">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="ef30a-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="ef30a-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="ef30a-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="ef30a-133">11 </span><span class="sxs-lookup"><span data-stu-id="ef30a-133">11</span></span>|<span data-ttu-id="ef30a-134">O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.</span><span class="sxs-lookup"><span data-stu-id="ef30a-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="ef30a-135">desconhecido</span><span class="sxs-lookup"><span data-stu-id="ef30a-135">unknown</span></span>|<span data-ttu-id="ef30a-136">16 </span><span class="sxs-lookup"><span data-stu-id="ef30a-136">16</span></span>|<span data-ttu-id="ef30a-137">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="ef30a-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="ef30a-138">jamf</span><span class="sxs-lookup"><span data-stu-id="ef30a-138">jamf</span></span>|<span data-ttu-id="ef30a-139">32</span><span class="sxs-lookup"><span data-stu-id="ef30a-139">32</span></span>|<span data-ttu-id="ef30a-140">Os atributos do dispositivo são buscados do JAMF.</span><span class="sxs-lookup"><span data-stu-id="ef30a-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="ef30a-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="ef30a-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="ef30a-142">64</span><span class="sxs-lookup"><span data-stu-id="ef30a-142">64</span></span>|<span data-ttu-id="ef30a-143">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="ef30a-143">The device is managed by Google's CloudDPC.</span></span>|




