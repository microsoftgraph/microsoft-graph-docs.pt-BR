---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d9407e1d035a5cd50db7b071f562acb4eb2d007b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371982"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="3df28-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="3df28-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="3df28-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3df28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3df28-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3df28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3df28-106">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="3df28-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="3df28-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3df28-107">Properties</span></span>
|<span data-ttu-id="3df28-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3df28-108">Property</span></span>|<span data-ttu-id="3df28-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3df28-109">Type</span></span>|<span data-ttu-id="3df28-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3df28-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3df28-111">inventory</span><span class="sxs-lookup"><span data-stu-id="3df28-111">inventory</span></span>|<span data-ttu-id="3df28-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="3df28-112">Boolean</span></span>|<span data-ttu-id="3df28-113">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="3df28-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="3df28-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="3df28-114">modernApps</span></span>|<span data-ttu-id="3df28-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="3df28-115">Boolean</span></span>|<span data-ttu-id="3df28-116">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="3df28-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="3df28-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="3df28-117">resourceAccess</span></span>|<span data-ttu-id="3df28-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="3df28-118">Boolean</span></span>|<span data-ttu-id="3df28-119">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="3df28-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="3df28-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3df28-120">deviceConfiguration</span></span>|<span data-ttu-id="3df28-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="3df28-121">Boolean</span></span>|<span data-ttu-id="3df28-122">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="3df28-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="3df28-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3df28-123">compliancePolicy</span></span>|<span data-ttu-id="3df28-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="3df28-124">Boolean</span></span>|<span data-ttu-id="3df28-125">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="3df28-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="3df28-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="3df28-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="3df28-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="3df28-127">Boolean</span></span>|<span data-ttu-id="3df28-128">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="3df28-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="3df28-129">endpointProtection</span><span class="sxs-lookup"><span data-stu-id="3df28-129">endpointProtection</span></span>|<span data-ttu-id="3df28-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="3df28-130">Boolean</span></span>|<span data-ttu-id="3df28-131">Se o Endpoint Protection é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="3df28-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="3df28-132">Officetreinamento</span><span class="sxs-lookup"><span data-stu-id="3df28-132">officeApps</span></span>|<span data-ttu-id="3df28-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="3df28-133">Boolean</span></span>|<span data-ttu-id="3df28-134">Se o aplicativo do Office é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="3df28-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="3df28-135">Relações</span><span class="sxs-lookup"><span data-stu-id="3df28-135">Relationships</span></span>
<span data-ttu-id="3df28-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3df28-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3df28-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3df28-137">JSON Representation</span></span>
<span data-ttu-id="3df28-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3df28-138">Here is a JSON representation of the resource.</span></span>
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



