---
title: tipo de enum managementAgentType
description: Tipo de agente de gerenciamento.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9c42d4ea4a5114bc42966891e4cd60ea87ca303e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401002"
---
# <a name="managementagenttype-enum-type"></a><span data-ttu-id="399bd-103">tipo de enum managementAgentType</span><span class="sxs-lookup"><span data-stu-id="399bd-103">managementAgentType enum type</span></span>

> <span data-ttu-id="399bd-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="399bd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="399bd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="399bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="399bd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="399bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="399bd-107">Tipo de agente de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="399bd-107">Management agent type.</span></span>

## <a name="members"></a><span data-ttu-id="399bd-108">Membros</span><span class="sxs-lookup"><span data-stu-id="399bd-108">Members</span></span>
|<span data-ttu-id="399bd-109">Membro</span><span class="sxs-lookup"><span data-stu-id="399bd-109">Member</span></span>|<span data-ttu-id="399bd-110">Valor</span><span class="sxs-lookup"><span data-stu-id="399bd-110">Value</span></span>|<span data-ttu-id="399bd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="399bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="399bd-112">EAs</span><span class="sxs-lookup"><span data-stu-id="399bd-112">eas</span></span>|<span data-ttu-id="399bd-113">1</span><span class="sxs-lookup"><span data-stu-id="399bd-113">1</span></span>|<span data-ttu-id="399bd-114">O dispositivo é gerenciado pelo Exchange server.</span><span class="sxs-lookup"><span data-stu-id="399bd-114">The device is managed by Exchange server.</span></span>|
|<span data-ttu-id="399bd-115">MDM</span><span class="sxs-lookup"><span data-stu-id="399bd-115">mdm</span></span>|<span data-ttu-id="399bd-116">2</span><span class="sxs-lookup"><span data-stu-id="399bd-116">2</span></span>|<span data-ttu-id="399bd-117">O dispositivo é gerenciado pelo MDM. Intune</span><span class="sxs-lookup"><span data-stu-id="399bd-117">The device is managed by Intune MDM.</span></span>|
|<span data-ttu-id="399bd-118">easMdm</span><span class="sxs-lookup"><span data-stu-id="399bd-118">easMdm</span></span>|<span data-ttu-id="399bd-119">3</span><span class="sxs-lookup"><span data-stu-id="399bd-119">3</span></span>|<span data-ttu-id="399bd-120">O dispositivo é gerenciado pelo Exchange server e MDM de Intune.</span><span class="sxs-lookup"><span data-stu-id="399bd-120">The device is managed by both Exchange server and Intune MDM.</span></span>|
|<span data-ttu-id="399bd-121">intuneClient</span><span class="sxs-lookup"><span data-stu-id="399bd-121">intuneClient</span></span>|<span data-ttu-id="399bd-122">4</span><span class="sxs-lookup"><span data-stu-id="399bd-122">4</span></span>|<span data-ttu-id="399bd-123">Cliente Intune gerenciados.</span><span class="sxs-lookup"><span data-stu-id="399bd-123">Intune client managed.</span></span>|
|<span data-ttu-id="399bd-124">easIntuneClient</span><span class="sxs-lookup"><span data-stu-id="399bd-124">easIntuneClient</span></span>|<span data-ttu-id="399bd-125">5</span><span class="sxs-lookup"><span data-stu-id="399bd-125">5</span></span>|<span data-ttu-id="399bd-126">O dispositivo está EAS Intune cliente e dual gerenciado.</span><span class="sxs-lookup"><span data-stu-id="399bd-126">The device is EAS and Intune client dual managed.</span></span>|
|<span data-ttu-id="399bd-127">configurationManagerClient</span><span class="sxs-lookup"><span data-stu-id="399bd-127">configurationManagerClient</span></span>|<span data-ttu-id="399bd-128">8</span><span class="sxs-lookup"><span data-stu-id="399bd-128">8</span></span>|<span data-ttu-id="399bd-129">O dispositivo é gerenciado pelo Gerenciador de configuração.</span><span class="sxs-lookup"><span data-stu-id="399bd-129">The device is managed by Configuration Manager.</span></span>|
|<span data-ttu-id="399bd-130">configurationManagerClientMdm</span><span class="sxs-lookup"><span data-stu-id="399bd-130">configurationManagerClientMdm</span></span>|<span data-ttu-id="399bd-131">10</span><span class="sxs-lookup"><span data-stu-id="399bd-131">10</span></span>|<span data-ttu-id="399bd-132">O dispositivo é gerenciado pelo Gerenciador de configuração e MDM.</span><span class="sxs-lookup"><span data-stu-id="399bd-132">The device is managed by Configuration Manager and MDM.</span></span>|
|<span data-ttu-id="399bd-133">configurationManagerClientMdmEas</span><span class="sxs-lookup"><span data-stu-id="399bd-133">configurationManagerClientMdmEas</span></span>|<span data-ttu-id="399bd-134">11</span><span class="sxs-lookup"><span data-stu-id="399bd-134">11</span></span>|<span data-ttu-id="399bd-135">O dispositivo é gerenciado pelo Gerenciador de configuração, MDM e Eas.</span><span class="sxs-lookup"><span data-stu-id="399bd-135">The device is managed by Configuration Manager, MDM and Eas.</span></span>|
|<span data-ttu-id="399bd-136">unknown</span><span class="sxs-lookup"><span data-stu-id="399bd-136">unknown</span></span>|<span data-ttu-id="399bd-137">16</span><span class="sxs-lookup"><span data-stu-id="399bd-137">16</span></span>|<span data-ttu-id="399bd-138">Tipo de agente de gerenciamento desconhecido.</span><span class="sxs-lookup"><span data-stu-id="399bd-138">Unknown management agent type.</span></span>|
|<span data-ttu-id="399bd-139">jamf</span><span class="sxs-lookup"><span data-stu-id="399bd-139">jamf</span></span>|<span data-ttu-id="399bd-140">32</span><span class="sxs-lookup"><span data-stu-id="399bd-140">32</span></span>|<span data-ttu-id="399bd-141">Os atributos de dispositivo são buscados no Jamf.</span><span class="sxs-lookup"><span data-stu-id="399bd-141">The device attributes are fetched from Jamf.</span></span>|
|<span data-ttu-id="399bd-142">googleCloudDevicePolicyController</span><span class="sxs-lookup"><span data-stu-id="399bd-142">googleCloudDevicePolicyController</span></span>|<span data-ttu-id="399bd-143">64</span><span class="sxs-lookup"><span data-stu-id="399bd-143">64</span></span>|<span data-ttu-id="399bd-144">O dispositivo é gerenciado por CloudDPC do Google.</span><span class="sxs-lookup"><span data-stu-id="399bd-144">The device is managed by Google's CloudDPC.</span></span>|
|<span data-ttu-id="399bd-145">microsoft365ManagedMdm</span><span class="sxs-lookup"><span data-stu-id="399bd-145">microsoft365ManagedMdm</span></span>|<span data-ttu-id="399bd-146">258</span><span class="sxs-lookup"><span data-stu-id="399bd-146">258</span></span>|<span data-ttu-id="399bd-147">Este dispositivo é gerenciado pelo Microsoft 365 através de Intune.</span><span class="sxs-lookup"><span data-stu-id="399bd-147">This device is managed by Microsoft 365 through Intune.</span></span>|




