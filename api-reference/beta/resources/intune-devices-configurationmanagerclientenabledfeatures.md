---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37c098910ec532a1ab23ae8464c03e43cf7a9e29
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943029"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="35ba8-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="35ba8-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="35ba8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="35ba8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35ba8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35ba8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35ba8-106">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="35ba8-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="35ba8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35ba8-107">Properties</span></span>
|<span data-ttu-id="35ba8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35ba8-108">Property</span></span>|<span data-ttu-id="35ba8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="35ba8-109">Type</span></span>|<span data-ttu-id="35ba8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="35ba8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35ba8-111">inventory</span><span class="sxs-lookup"><span data-stu-id="35ba8-111">inventory</span></span>|<span data-ttu-id="35ba8-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="35ba8-112">Boolean</span></span>|<span data-ttu-id="35ba8-113">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="35ba8-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="35ba8-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="35ba8-114">modernApps</span></span>|<span data-ttu-id="35ba8-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="35ba8-115">Boolean</span></span>|<span data-ttu-id="35ba8-116">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="35ba8-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="35ba8-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="35ba8-117">resourceAccess</span></span>|<span data-ttu-id="35ba8-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="35ba8-118">Boolean</span></span>|<span data-ttu-id="35ba8-119">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="35ba8-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="35ba8-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="35ba8-120">deviceConfiguration</span></span>|<span data-ttu-id="35ba8-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="35ba8-121">Boolean</span></span>|<span data-ttu-id="35ba8-122">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="35ba8-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="35ba8-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="35ba8-123">compliancePolicy</span></span>|<span data-ttu-id="35ba8-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="35ba8-124">Boolean</span></span>|<span data-ttu-id="35ba8-125">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="35ba8-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="35ba8-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="35ba8-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="35ba8-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="35ba8-127">Boolean</span></span>|<span data-ttu-id="35ba8-128">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="35ba8-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="35ba8-129">endpointProtection</span><span class="sxs-lookup"><span data-stu-id="35ba8-129">endpointProtection</span></span>|<span data-ttu-id="35ba8-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="35ba8-130">Boolean</span></span>|<span data-ttu-id="35ba8-131">Se o Endpoint Protection é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="35ba8-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="35ba8-132">Officetreinamento</span><span class="sxs-lookup"><span data-stu-id="35ba8-132">officeApps</span></span>|<span data-ttu-id="35ba8-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="35ba8-133">Boolean</span></span>|<span data-ttu-id="35ba8-134">Se o aplicativo do Office é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="35ba8-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="35ba8-135">Relações</span><span class="sxs-lookup"><span data-stu-id="35ba8-135">Relationships</span></span>
<span data-ttu-id="35ba8-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35ba8-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35ba8-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35ba8-137">JSON Representation</span></span>
<span data-ttu-id="35ba8-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35ba8-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true,
  "endpointProtection": true,
  "officeApps": true
}
```




