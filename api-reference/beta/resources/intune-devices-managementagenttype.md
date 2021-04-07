---
title: tipo de número managementAgentType
description: Tipo de agente de gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 331fd26e009fce708d13f4422c8eef0e6d19d0f8
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612093"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="5708d-103">tipo de número managementAgentType</span><span class="sxs-lookup"><span data-stu-id="5708d-103">managementAgentType enum type</span></span>

<span data-ttu-id="5708d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5708d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5708d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5708d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5708d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5708d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5708d-107">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="5708d-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="5708d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5708d-108">Members</span></span>
|<span data-ttu-id="5708d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5708d-109">Member</span></span>|<span data-ttu-id="5708d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5708d-110">Value</span></span>|<span data-ttu-id="5708d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5708d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5708d-112">eas</span><span class="sxs-lookup"><span data-stu-id="5708d-112">eas</span></span>|<span data-ttu-id="5708d-113">1</span><span class="sxs-lookup"><span data-stu-id="5708d-113">1</span></span>|<span data-ttu-id="5708d-114">O dispositivo é gerenciado pelo servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="5708d-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="5708d-115">mdm</span><span class="sxs-lookup"><span data-stu-id="5708d-115">mdm</span></span>|<span data-ttu-id="5708d-116">2</span><span class="sxs-lookup"><span data-stu-id="5708d-116">2</span></span>|<span data-ttu-id="5708d-117">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="5708d-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="5708d-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="5708d-118">easMdm</span></span>|<span data-ttu-id="5708d-119">3</span><span class="sxs-lookup"><span data-stu-id="5708d-119">3</span></span>|<span data-ttu-id="5708d-120">O dispositivo é gerenciado pelo servidor Exchange e pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="5708d-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="5708d-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="5708d-121">intuneClient</span></span>|<span data-ttu-id="5708d-122">4 </span><span class="sxs-lookup"><span data-stu-id="5708d-122">4</span></span>|<span data-ttu-id="5708d-123">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="5708d-123">Intune client managed.</span></span>|
|<span data-ttu-id="5708d-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="5708d-124">easIntuneClient</span></span>|<span data-ttu-id="5708d-125">5 </span><span class="sxs-lookup"><span data-stu-id="5708d-125">5</span></span>|<span data-ttu-id="5708d-126">O dispositivo é gerenciado duplo do cliente EAS e do Intune.</span><span class="sxs-lookup"><span data-stu-id="5708d-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="5708d-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="5708d-127">configurationManagerClient</span></span>|<span data-ttu-id="5708d-128">8 </span><span class="sxs-lookup"><span data-stu-id="5708d-128">8</span></span>|<span data-ttu-id="5708d-129">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="5708d-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="5708d-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="5708d-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="5708d-131">10 </span><span class="sxs-lookup"><span data-stu-id="5708d-131">10</span></span>|<span data-ttu-id="5708d-132">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="5708d-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="5708d-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="5708d-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="5708d-134">11</span><span class="sxs-lookup"><span data-stu-id="5708d-134">11</span></span>|<span data-ttu-id="5708d-135">O dispositivo é gerenciado pelo Configuration Manager, MDM e Eas.</span><span class="sxs-lookup"><span data-stu-id="5708d-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="5708d-136">desconhecido</span><span class="sxs-lookup"><span data-stu-id="5708d-136">unknown</span></span>|<span data-ttu-id="5708d-137">16 </span><span class="sxs-lookup"><span data-stu-id="5708d-137">16</span></span>|<span data-ttu-id="5708d-138">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="5708d-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="5708d-139">jamf</span><span class="sxs-lookup"><span data-stu-id="5708d-139">jamf</span></span>|<span data-ttu-id="5708d-140">32</span><span class="sxs-lookup"><span data-stu-id="5708d-140">32</span></span>|<span data-ttu-id="5708d-141">Os atributos do dispositivo são buscados do Jamf.</span><span class="sxs-lookup"><span data-stu-id="5708d-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="5708d-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="5708d-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="5708d-143">64</span><span class="sxs-lookup"><span data-stu-id="5708d-143">64</span></span>|<span data-ttu-id="5708d-144">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="5708d-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="5708d-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="5708d-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="5708d-146">258</span><span class="sxs-lookup"><span data-stu-id="5708d-146">258</span></span>|<span data-ttu-id="5708d-147">Esse dispositivo é gerenciado pelo Microsoft 365 por meio do Intune.</span><span class="sxs-lookup"><span data-stu-id="5708d-147">This device is managed by Microsoft 365 through Intune.</span></span>|




