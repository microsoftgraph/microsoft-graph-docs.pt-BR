---
title: tipo de enum managementAgentType
description: Tipo de agente de gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b76231a2781a153c5384c1dc3efdf8facec04dcc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966164"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="7c8ac-103">tipo de enum managementAgentType</span><span class="sxs-lookup"><span data-stu-id="7c8ac-103">managementAgentType enum type</span></span>

> <span data-ttu-id="7c8ac-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c8ac-105">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-105">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="7c8ac-106">Membros</span><span class="sxs-lookup"><span data-stu-id="7c8ac-106">Members</span></span>
|<span data-ttu-id="7c8ac-107">Membro</span><span class="sxs-lookup"><span data-stu-id="7c8ac-107">Member</span></span>|<span data-ttu-id="7c8ac-108">Valor</span><span class="sxs-lookup"><span data-stu-id="7c8ac-108">Value</span></span>|<span data-ttu-id="7c8ac-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c8ac-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c8ac-110">EAs</span><span class="sxs-lookup"><span data-stu-id="7c8ac-110">eas</span></span>|<span data-ttu-id="7c8ac-111">1</span><span class="sxs-lookup"><span data-stu-id="7c8ac-111">1</span></span>|<span data-ttu-id="7c8ac-112">O dispositivo é gerenciado pelo Exchange server.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-112">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="7c8ac-113">MDM</span><span class="sxs-lookup"><span data-stu-id="7c8ac-113">mdm</span></span>|<span data-ttu-id="7c8ac-114">2</span><span class="sxs-lookup"><span data-stu-id="7c8ac-114">2</span></span>|<span data-ttu-id="7c8ac-115">O dispositivo é gerenciado pelo MDM. Intune</span><span class="sxs-lookup"><span data-stu-id="7c8ac-115">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="7c8ac-116">easMdm</span><span class="sxs-lookup"><span data-stu-id="7c8ac-116">easMdm</span></span>|<span data-ttu-id="7c8ac-117">3</span><span class="sxs-lookup"><span data-stu-id="7c8ac-117">3</span></span>|<span data-ttu-id="7c8ac-118">O dispositivo é gerenciado pelo Exchange server e MDM de Intune.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-118">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="7c8ac-119">intuneClient</span><span class="sxs-lookup"><span data-stu-id="7c8ac-119">intuneClient</span></span>|<span data-ttu-id="7c8ac-120">4</span><span class="sxs-lookup"><span data-stu-id="7c8ac-120">4</span></span>|<span data-ttu-id="7c8ac-121">Cliente Intune gerenciados.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-121">Intune client managed.</span></span>|
|<span data-ttu-id="7c8ac-122">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="7c8ac-122">easIntuneClient</span></span>|<span data-ttu-id="7c8ac-123">5</span><span class="sxs-lookup"><span data-stu-id="7c8ac-123">5</span></span>|<span data-ttu-id="7c8ac-124">O dispositivo está EAS Intune cliente e dual gerenciado.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-124">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="7c8ac-125">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="7c8ac-125">configurationManagerClient</span></span>|<span data-ttu-id="7c8ac-126">8</span><span class="sxs-lookup"><span data-stu-id="7c8ac-126">8</span></span>|<span data-ttu-id="7c8ac-127">O dispositivo é gerenciado pelo Gerenciador de configuração.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-127">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="7c8ac-128">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="7c8ac-128">configurationManagerClientMdm</span></span>|<span data-ttu-id="7c8ac-129">10</span><span class="sxs-lookup"><span data-stu-id="7c8ac-129">10</span></span>|<span data-ttu-id="7c8ac-130">O dispositivo é gerenciado pelo Gerenciador de configuração e MDM.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-130">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="7c8ac-131">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="7c8ac-131">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="7c8ac-132">11</span><span class="sxs-lookup"><span data-stu-id="7c8ac-132">11</span></span>|<span data-ttu-id="7c8ac-133">O dispositivo é gerenciado pelo Gerenciador de configuração, MDM e Eas.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-133">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="7c8ac-134">unknown</span><span class="sxs-lookup"><span data-stu-id="7c8ac-134">unknown</span></span>|<span data-ttu-id="7c8ac-135">16</span><span class="sxs-lookup"><span data-stu-id="7c8ac-135">16</span></span>|<span data-ttu-id="7c8ac-136">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-136">Unknown management agent type.</span></span>|
|<span data-ttu-id="7c8ac-137">jamf</span><span class="sxs-lookup"><span data-stu-id="7c8ac-137">jamf</span></span>|<span data-ttu-id="7c8ac-138">32</span><span class="sxs-lookup"><span data-stu-id="7c8ac-138">32</span></span>|<span data-ttu-id="7c8ac-139">Os atributos de dispositivo são buscados no Jamf.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-139">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="7c8ac-140">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="7c8ac-140">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="7c8ac-141">64</span><span class="sxs-lookup"><span data-stu-id="7c8ac-141">64</span></span>|<span data-ttu-id="7c8ac-142">O dispositivo é gerenciado por CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="7c8ac-142">The device is managed by Google's CloudDPC.</span></span>|



