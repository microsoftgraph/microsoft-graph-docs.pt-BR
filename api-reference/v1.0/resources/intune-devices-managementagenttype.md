---
title: tipo de enumeração managementAgentType
description: Tipo de agente de gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9743c9c83e34a0c58dee78e73839f8fdcaaf2cda
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251563"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="8d0c5-103">tipo de enumeração managementAgentType</span><span class="sxs-lookup"><span data-stu-id="8d0c5-103">managementAgentType enum type</span></span>

> <span data-ttu-id="8d0c5-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8d0c5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d0c5-105">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="8d0c5-105">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="8d0c5-106">Membros</span><span class="sxs-lookup"><span data-stu-id="8d0c5-106">Members</span></span>
|<span data-ttu-id="8d0c5-107">Membro</span><span class="sxs-lookup"><span data-stu-id="8d0c5-107">Member</span></span>|<span data-ttu-id="8d0c5-108">Valor</span><span class="sxs-lookup"><span data-stu-id="8d0c5-108">Value</span></span>|<span data-ttu-id="8d0c5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d0c5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d0c5-110">Estendi</span><span class="sxs-lookup"><span data-stu-id="8d0c5-110">eas</span></span>|<span data-ttu-id="8d0c5-111">1</span><span class="sxs-lookup"><span data-stu-id="8d0c5-111">1</span></span>|<span data-ttu-id="8d0c5-112">O dispositivo é gerenciado pelo Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="8d0c5-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="8d0c5-113">MDM</span><span class="sxs-lookup"><span data-stu-id="8d0c5-113">mdm</span></span>|<span data-ttu-id="8d0c5-114">duas</span><span class="sxs-lookup"><span data-stu-id="8d0c5-114">2</span></span>|<span data-ttu-id="8d0c5-115">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="8d0c5-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="8d0c5-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="8d0c5-116">easMdm</span></span>|<span data-ttu-id="8d0c5-117">3D</span><span class="sxs-lookup"><span data-stu-id="8d0c5-117">3</span></span>|<span data-ttu-id="8d0c5-118">O dispositivo é gerenciado pelo Exchange Server e o MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="8d0c5-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="8d0c5-119">intuneClient</span><span class="sxs-lookup"><span data-stu-id="8d0c5-119">intuneClient</span></span>|<span data-ttu-id="8d0c5-120">quatro</span><span class="sxs-lookup"><span data-stu-id="8d0c5-120">4</span></span>|<span data-ttu-id="8d0c5-121">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="8d0c5-121">Intune client managed.</span></span>|
|<span data-ttu-id="8d0c5-122">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="8d0c5-122">easIntuneClient</span></span>|<span data-ttu-id="8d0c5-123">0,5</span><span class="sxs-lookup"><span data-stu-id="8d0c5-123">5</span></span>|<span data-ttu-id="8d0c5-124">O dispositivo é ESTENDIdo e o cliente do Intune é gerenciado duas.</span><span class="sxs-lookup"><span data-stu-id="8d0c5-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="8d0c5-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="8d0c5-125">configurationManagerClient</span></span>|<span data-ttu-id="8d0c5-126">8</span><span class="sxs-lookup"><span data-stu-id="8d0c5-126">8</span></span>|<span data-ttu-id="8d0c5-127">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="8d0c5-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="8d0c5-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="8d0c5-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="8d0c5-129">254</span><span class="sxs-lookup"><span data-stu-id="8d0c5-129">10</span></span>|<span data-ttu-id="8d0c5-130">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="8d0c5-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="8d0c5-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="8d0c5-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="8d0c5-132">11</span><span class="sxs-lookup"><span data-stu-id="8d0c5-132">11</span></span>|<span data-ttu-id="8d0c5-133">O dispositivo é gerenciado pelo Configuration Manager, MDM e EAS.</span><span class="sxs-lookup"><span data-stu-id="8d0c5-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="8d0c5-134">unknown</span><span class="sxs-lookup"><span data-stu-id="8d0c5-134">unknown</span></span>|<span data-ttu-id="8d0c5-135">dezesseis</span><span class="sxs-lookup"><span data-stu-id="8d0c5-135">16</span></span>|<span data-ttu-id="8d0c5-136">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="8d0c5-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="8d0c5-137">JAMF</span><span class="sxs-lookup"><span data-stu-id="8d0c5-137">jamf</span></span>|<span data-ttu-id="8d0c5-138">32</span><span class="sxs-lookup"><span data-stu-id="8d0c5-138">32</span></span>|<span data-ttu-id="8d0c5-139">Os atributos do dispositivo são buscados do JAMF.</span><span class="sxs-lookup"><span data-stu-id="8d0c5-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="8d0c5-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="8d0c5-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="8d0c5-141">64</span><span class="sxs-lookup"><span data-stu-id="8d0c5-141">64</span></span>|<span data-ttu-id="8d0c5-142">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="8d0c5-142">The device is managed by Google's CloudDPC.</span></span>|



