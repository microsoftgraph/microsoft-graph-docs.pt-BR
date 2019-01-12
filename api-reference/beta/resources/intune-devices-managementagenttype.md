---
title: tipo de enum managementAgentType
description: Tipo de agente de gerenciamento.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1711ad647afabc2b8877bd2f99b049bd1c1dd4e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914280"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="c70f2-103">tipo de enum managementAgentType</span><span class="sxs-lookup"><span data-stu-id="c70f2-103">managementAgentType enum type</span></span>

> <span data-ttu-id="c70f2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c70f2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c70f2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c70f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c70f2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c70f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c70f2-107">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c70f2-107">Management agent type.</span></span>
## <a name="members"></a><span data-ttu-id="c70f2-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c70f2-108">Members</span></span>
|<span data-ttu-id="c70f2-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c70f2-109">Member</span></span>|<span data-ttu-id="c70f2-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c70f2-110">Value</span></span>|<span data-ttu-id="c70f2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c70f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c70f2-112">EAs</span><span class="sxs-lookup"><span data-stu-id="c70f2-112">eas</span></span>|<span data-ttu-id="c70f2-113">1</span><span class="sxs-lookup"><span data-stu-id="c70f2-113">1</span></span>|<span data-ttu-id="c70f2-114">O dispositivo é gerenciado pelo Exchange server.</span><span class="sxs-lookup"><span data-stu-id="c70f2-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="c70f2-115">MDM</span><span class="sxs-lookup"><span data-stu-id="c70f2-115">mdm</span></span>|<span data-ttu-id="c70f2-116">2</span><span class="sxs-lookup"><span data-stu-id="c70f2-116">2</span></span>|<span data-ttu-id="c70f2-117">O dispositivo é gerenciado pelo MDM. Intune</span><span class="sxs-lookup"><span data-stu-id="c70f2-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="c70f2-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="c70f2-118">easMdm</span></span>|<span data-ttu-id="c70f2-119">3</span><span class="sxs-lookup"><span data-stu-id="c70f2-119">3</span></span>|<span data-ttu-id="c70f2-120">O dispositivo é gerenciado pelo Exchange server e MDM de Intune.</span><span class="sxs-lookup"><span data-stu-id="c70f2-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="c70f2-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="c70f2-121">intuneClient</span></span>|<span data-ttu-id="c70f2-122">4</span><span class="sxs-lookup"><span data-stu-id="c70f2-122">4</span></span>|<span data-ttu-id="c70f2-123">Cliente Intune gerenciados.</span><span class="sxs-lookup"><span data-stu-id="c70f2-123">Intune client managed.</span></span>|
|<span data-ttu-id="c70f2-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="c70f2-124">easIntuneClient</span></span>|<span data-ttu-id="c70f2-125">5</span><span class="sxs-lookup"><span data-stu-id="c70f2-125">5</span></span>|<span data-ttu-id="c70f2-126">O dispositivo está EAS Intune cliente e dual gerenciado.</span><span class="sxs-lookup"><span data-stu-id="c70f2-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="c70f2-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="c70f2-127">configurationManagerClient</span></span>|<span data-ttu-id="c70f2-128">8</span><span class="sxs-lookup"><span data-stu-id="c70f2-128">8</span></span>|<span data-ttu-id="c70f2-129">O dispositivo é gerenciado pelo Gerenciador de configuração.</span><span class="sxs-lookup"><span data-stu-id="c70f2-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="c70f2-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="c70f2-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="c70f2-131">10</span><span class="sxs-lookup"><span data-stu-id="c70f2-131">10</span></span>|<span data-ttu-id="c70f2-132">O dispositivo é gerenciado pelo Gerenciador de configuração e MDM.</span><span class="sxs-lookup"><span data-stu-id="c70f2-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="c70f2-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="c70f2-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="c70f2-134">11</span><span class="sxs-lookup"><span data-stu-id="c70f2-134">11</span></span>|<span data-ttu-id="c70f2-135">O dispositivo é gerenciado pelo Gerenciador de configuração, MDM e Eas.</span><span class="sxs-lookup"><span data-stu-id="c70f2-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="c70f2-136">unknown</span><span class="sxs-lookup"><span data-stu-id="c70f2-136">unknown</span></span>|<span data-ttu-id="c70f2-137">16</span><span class="sxs-lookup"><span data-stu-id="c70f2-137">16</span></span>|<span data-ttu-id="c70f2-138">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="c70f2-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="c70f2-139">jamf</span><span class="sxs-lookup"><span data-stu-id="c70f2-139">jamf</span></span>|<span data-ttu-id="c70f2-140">32</span><span class="sxs-lookup"><span data-stu-id="c70f2-140">32</span></span>|<span data-ttu-id="c70f2-141">Os atributos de dispositivo são buscados no Jamf.</span><span class="sxs-lookup"><span data-stu-id="c70f2-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="c70f2-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="c70f2-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="c70f2-143">64</span><span class="sxs-lookup"><span data-stu-id="c70f2-143">64</span></span>|<span data-ttu-id="c70f2-144">O dispositivo é gerenciado por CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="c70f2-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="c70f2-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="c70f2-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="c70f2-146">258</span><span class="sxs-lookup"><span data-stu-id="c70f2-146">258</span></span>|<span data-ttu-id="c70f2-147">Este dispositivo é gerenciado pelo Microsoft 365 através de Intune.</span><span class="sxs-lookup"><span data-stu-id="c70f2-147">This device is managed by Microsoft 365 through Intune.</span></span>|





