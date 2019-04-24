---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9743c9c83e34a0c58dee78e73839f8fdcaaf2cda
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522710"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="f4915-103">tipo de enumeração managementAgentType</span><span class="sxs-lookup"><span data-stu-id="f4915-103">managementAgentType enum type</span></span>

> <span data-ttu-id="f4915-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4915-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4915-105">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f4915-105">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="f4915-106">Membros</span><span class="sxs-lookup"><span data-stu-id="f4915-106">Members</span></span>
|<span data-ttu-id="f4915-107">Membro</span><span class="sxs-lookup"><span data-stu-id="f4915-107">Member</span></span>|<span data-ttu-id="f4915-108">Valor</span><span class="sxs-lookup"><span data-stu-id="f4915-108">Value</span></span>|<span data-ttu-id="f4915-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4915-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4915-110">Estendi</span><span class="sxs-lookup"><span data-stu-id="f4915-110">eas</span></span>|<span data-ttu-id="f4915-111">1 </span><span class="sxs-lookup"><span data-stu-id="f4915-111">1</span></span>|<span data-ttu-id="f4915-112">O dispositivo é gerenciado pelo Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="f4915-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="f4915-113">MDM</span><span class="sxs-lookup"><span data-stu-id="f4915-113">mdm</span></span>|<span data-ttu-id="f4915-114">2 </span><span class="sxs-lookup"><span data-stu-id="f4915-114">2</span></span>|<span data-ttu-id="f4915-115">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="f4915-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="f4915-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="f4915-116">easMdm</span></span>|<span data-ttu-id="f4915-117">3 </span><span class="sxs-lookup"><span data-stu-id="f4915-117">3</span></span>|<span data-ttu-id="f4915-118">O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="f4915-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="f4915-119">intuneClient</span><span class="sxs-lookup"><span data-stu-id="f4915-119">intuneClient</span></span>|<span data-ttu-id="f4915-120">4 </span><span class="sxs-lookup"><span data-stu-id="f4915-120">4</span></span>|<span data-ttu-id="f4915-121">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f4915-121">Intune client managed.</span></span>|
|<span data-ttu-id="f4915-122">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="f4915-122">easIntuneClient</span></span>|<span data-ttu-id="f4915-123">5 </span><span class="sxs-lookup"><span data-stu-id="f4915-123">5</span></span>|<span data-ttu-id="f4915-124">O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.</span><span class="sxs-lookup"><span data-stu-id="f4915-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="f4915-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="f4915-125">configurationManagerClient</span></span>|<span data-ttu-id="f4915-126">8 </span><span class="sxs-lookup"><span data-stu-id="f4915-126">8</span></span>|<span data-ttu-id="f4915-127">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="f4915-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="f4915-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="f4915-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="f4915-129">10 </span><span class="sxs-lookup"><span data-stu-id="f4915-129">10</span></span>|<span data-ttu-id="f4915-130">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="f4915-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="f4915-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="f4915-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="f4915-132">11 </span><span class="sxs-lookup"><span data-stu-id="f4915-132">11</span></span>|<span data-ttu-id="f4915-133">O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.</span><span class="sxs-lookup"><span data-stu-id="f4915-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="f4915-134">desconhecido</span><span class="sxs-lookup"><span data-stu-id="f4915-134">unknown</span></span>|<span data-ttu-id="f4915-135">16 </span><span class="sxs-lookup"><span data-stu-id="f4915-135">16</span></span>|<span data-ttu-id="f4915-136">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="f4915-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="f4915-137">JAMF</span><span class="sxs-lookup"><span data-stu-id="f4915-137">jamf</span></span>|<span data-ttu-id="f4915-138">32</span><span class="sxs-lookup"><span data-stu-id="f4915-138">32</span></span>|<span data-ttu-id="f4915-139">Os atributos do dispositivo são buscados do JAMF.</span><span class="sxs-lookup"><span data-stu-id="f4915-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="f4915-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="f4915-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="f4915-141">64</span><span class="sxs-lookup"><span data-stu-id="f4915-141">64</span></span>|<span data-ttu-id="f4915-142">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="f4915-142">The device is managed by Google's CloudDPC.</span></span>|



