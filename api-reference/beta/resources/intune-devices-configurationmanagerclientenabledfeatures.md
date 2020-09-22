---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 317378e58c870e77140ae961925aeb59a001daff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060640"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="1e5f7-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="1e5f7-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="1e5f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e5f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e5f7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e5f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e5f7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e5f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e5f7-107">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="1e5f7-107">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="1e5f7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e5f7-108">Properties</span></span>
|<span data-ttu-id="1e5f7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e5f7-109">Property</span></span>|<span data-ttu-id="1e5f7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e5f7-110">Type</span></span>|<span data-ttu-id="1e5f7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e5f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e5f7-112">inventory</span><span class="sxs-lookup"><span data-stu-id="1e5f7-112">inventory</span></span>|<span data-ttu-id="1e5f7-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e5f7-113">Boolean</span></span>|<span data-ttu-id="1e5f7-114">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="1e5f7-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="1e5f7-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="1e5f7-115">modernApps</span></span>|<span data-ttu-id="1e5f7-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e5f7-116">Boolean</span></span>|<span data-ttu-id="1e5f7-117">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="1e5f7-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="1e5f7-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="1e5f7-118">resourceAccess</span></span>|<span data-ttu-id="1e5f7-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e5f7-119">Boolean</span></span>|<span data-ttu-id="1e5f7-120">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="1e5f7-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="1e5f7-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e5f7-121">deviceConfiguration</span></span>|<span data-ttu-id="1e5f7-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e5f7-122">Boolean</span></span>|<span data-ttu-id="1e5f7-123">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="1e5f7-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="1e5f7-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="1e5f7-124">compliancePolicy</span></span>|<span data-ttu-id="1e5f7-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e5f7-125">Boolean</span></span>|<span data-ttu-id="1e5f7-126">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="1e5f7-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="1e5f7-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="1e5f7-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="1e5f7-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e5f7-128">Boolean</span></span>|<span data-ttu-id="1e5f7-129">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="1e5f7-129">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="1e5f7-130">endpointProtection</span><span class="sxs-lookup"><span data-stu-id="1e5f7-130">endpointProtection</span></span>|<span data-ttu-id="1e5f7-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e5f7-131">Boolean</span></span>|<span data-ttu-id="1e5f7-132">Se o Endpoint Protection é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="1e5f7-132">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="1e5f7-133">Officetreinamento</span><span class="sxs-lookup"><span data-stu-id="1e5f7-133">officeApps</span></span>|<span data-ttu-id="1e5f7-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e5f7-134">Boolean</span></span>|<span data-ttu-id="1e5f7-135">Se o aplicativo do Office é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="1e5f7-135">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e5f7-136">Relações</span><span class="sxs-lookup"><span data-stu-id="1e5f7-136">Relationships</span></span>
<span data-ttu-id="1e5f7-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1e5f7-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e5f7-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e5f7-138">JSON Representation</span></span>
<span data-ttu-id="1e5f7-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e5f7-139">Here is a JSON representation of the resource.</span></span>
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






