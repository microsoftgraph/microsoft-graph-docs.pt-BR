---
title: tipo de número managementAgentType
description: Tipo de agente de gerenciamento.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0a11300891ca4b12b15de26b5be929823b4a8ddf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751353"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="bc4cd-103">tipo de número managementAgentType</span><span class="sxs-lookup"><span data-stu-id="bc4cd-103">managementAgentType enum type</span></span>

<span data-ttu-id="bc4cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc4cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc4cd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc4cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc4cd-106">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="bc4cd-106">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="bc4cd-107">Membros</span><span class="sxs-lookup"><span data-stu-id="bc4cd-107">Members</span></span>
|<span data-ttu-id="bc4cd-108">Membro</span><span class="sxs-lookup"><span data-stu-id="bc4cd-108">Member</span></span>|<span data-ttu-id="bc4cd-109">Valor</span><span class="sxs-lookup"><span data-stu-id="bc4cd-109">Value</span></span>|<span data-ttu-id="bc4cd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc4cd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc4cd-111">eas</span><span class="sxs-lookup"><span data-stu-id="bc4cd-111">eas</span></span>|<span data-ttu-id="bc4cd-112">1</span><span class="sxs-lookup"><span data-stu-id="bc4cd-112">1</span></span>|<span data-ttu-id="bc4cd-113">O dispositivo é gerenciado por Exchange servidor.</span><span class="sxs-lookup"><span data-stu-id="bc4cd-113">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="bc4cd-114">mdm</span><span class="sxs-lookup"><span data-stu-id="bc4cd-114">mdm</span></span>|<span data-ttu-id="bc4cd-115">2</span><span class="sxs-lookup"><span data-stu-id="bc4cd-115">2</span></span>|<span data-ttu-id="bc4cd-116">O dispositivo é gerenciado pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="bc4cd-116">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="bc4cd-117">easMdm</span><span class="sxs-lookup"><span data-stu-id="bc4cd-117">easMdm</span></span>|<span data-ttu-id="bc4cd-118">3</span><span class="sxs-lookup"><span data-stu-id="bc4cd-118">3</span></span>|<span data-ttu-id="bc4cd-119">O dispositivo é gerenciado pelo servidor Exchange e pelo MDM do Intune.</span><span class="sxs-lookup"><span data-stu-id="bc4cd-119">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="bc4cd-120">intuneClient</span><span class="sxs-lookup"><span data-stu-id="bc4cd-120">intuneClient</span></span>|<span data-ttu-id="bc4cd-121">4 </span><span class="sxs-lookup"><span data-stu-id="bc4cd-121">4</span></span>|<span data-ttu-id="bc4cd-122">Cliente do Intune gerenciado.</span><span class="sxs-lookup"><span data-stu-id="bc4cd-122">Intune client managed.</span></span>|
|<span data-ttu-id="bc4cd-123">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="bc4cd-123">easIntuneClient</span></span>|<span data-ttu-id="bc4cd-124">5 </span><span class="sxs-lookup"><span data-stu-id="bc4cd-124">5</span></span>|<span data-ttu-id="bc4cd-125">O dispositivo é gerenciado duplo do cliente EAS e do Intune.</span><span class="sxs-lookup"><span data-stu-id="bc4cd-125">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="bc4cd-126">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="bc4cd-126">configurationManagerClient</span></span>|<span data-ttu-id="bc4cd-127">8 </span><span class="sxs-lookup"><span data-stu-id="bc4cd-127">8</span></span>|<span data-ttu-id="bc4cd-128">O dispositivo é gerenciado pelo Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="bc4cd-128">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="bc4cd-129">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="bc4cd-129">configurationManagerClientMdm</span></span>|<span data-ttu-id="bc4cd-130">10 </span><span class="sxs-lookup"><span data-stu-id="bc4cd-130">10</span></span>|<span data-ttu-id="bc4cd-131">O dispositivo é gerenciado pelo Configuration Manager e pelo MDM.</span><span class="sxs-lookup"><span data-stu-id="bc4cd-131">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="bc4cd-132">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="bc4cd-132">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="bc4cd-133">11</span><span class="sxs-lookup"><span data-stu-id="bc4cd-133">11</span></span>|<span data-ttu-id="bc4cd-134">O dispositivo é gerenciado pelo Configuration Manager, MDM e Eas.</span><span class="sxs-lookup"><span data-stu-id="bc4cd-134">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="bc4cd-135">desconhecido</span><span class="sxs-lookup"><span data-stu-id="bc4cd-135">unknown</span></span>|<span data-ttu-id="bc4cd-136">16 </span><span class="sxs-lookup"><span data-stu-id="bc4cd-136">16</span></span>|<span data-ttu-id="bc4cd-137">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="bc4cd-137">Unknown management agent type.</span></span>|
|<span data-ttu-id="bc4cd-138">jamf</span><span class="sxs-lookup"><span data-stu-id="bc4cd-138">jamf</span></span>|<span data-ttu-id="bc4cd-139">32</span><span class="sxs-lookup"><span data-stu-id="bc4cd-139">32</span></span>|<span data-ttu-id="bc4cd-140">Os atributos do dispositivo são buscados do Jamf.</span><span class="sxs-lookup"><span data-stu-id="bc4cd-140">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="bc4cd-141">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="bc4cd-141">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="bc4cd-142">64</span><span class="sxs-lookup"><span data-stu-id="bc4cd-142">64</span></span>|<span data-ttu-id="bc4cd-143">O dispositivo é gerenciado pelo CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="bc4cd-143">The device is managed by Google's CloudDPC.</span></span>|




