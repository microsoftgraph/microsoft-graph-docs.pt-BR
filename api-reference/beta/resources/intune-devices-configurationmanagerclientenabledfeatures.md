---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 189751d12f7220dcfa4e3e6985c3913bb7ae0e32
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465057"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="f9a1e-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f9a1e-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="f9a1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9a1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9a1e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f9a1e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9a1e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9a1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9a1e-107">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="f9a1e-107">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="f9a1e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9a1e-108">Properties</span></span>
|<span data-ttu-id="f9a1e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9a1e-109">Property</span></span>|<span data-ttu-id="f9a1e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9a1e-110">Type</span></span>|<span data-ttu-id="f9a1e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9a1e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9a1e-112">inventory</span><span class="sxs-lookup"><span data-stu-id="f9a1e-112">inventory</span></span>|<span data-ttu-id="f9a1e-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9a1e-113">Boolean</span></span>|<span data-ttu-id="f9a1e-114">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="f9a1e-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="f9a1e-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="f9a1e-115">modernApps</span></span>|<span data-ttu-id="f9a1e-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9a1e-116">Boolean</span></span>|<span data-ttu-id="f9a1e-117">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="f9a1e-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="f9a1e-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="f9a1e-118">resourceAccess</span></span>|<span data-ttu-id="f9a1e-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9a1e-119">Boolean</span></span>|<span data-ttu-id="f9a1e-120">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="f9a1e-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="f9a1e-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9a1e-121">deviceConfiguration</span></span>|<span data-ttu-id="f9a1e-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9a1e-122">Boolean</span></span>|<span data-ttu-id="f9a1e-123">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="f9a1e-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="f9a1e-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f9a1e-124">compliancePolicy</span></span>|<span data-ttu-id="f9a1e-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9a1e-125">Boolean</span></span>|<span data-ttu-id="f9a1e-126">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="f9a1e-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="f9a1e-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="f9a1e-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="f9a1e-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9a1e-128">Boolean</span></span>|<span data-ttu-id="f9a1e-129">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="f9a1e-129">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="f9a1e-130">endpointProtection</span><span class="sxs-lookup"><span data-stu-id="f9a1e-130">endpointProtection</span></span>|<span data-ttu-id="f9a1e-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9a1e-131">Boolean</span></span>|<span data-ttu-id="f9a1e-132">Se o Endpoint Protection é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="f9a1e-132">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="f9a1e-133">Officetreinamento</span><span class="sxs-lookup"><span data-stu-id="f9a1e-133">officeApps</span></span>|<span data-ttu-id="f9a1e-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9a1e-134">Boolean</span></span>|<span data-ttu-id="f9a1e-135">Se o aplicativo do Office é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="f9a1e-135">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9a1e-136">Relações</span><span class="sxs-lookup"><span data-stu-id="f9a1e-136">Relationships</span></span>
<span data-ttu-id="f9a1e-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f9a1e-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9a1e-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9a1e-138">JSON Representation</span></span>
<span data-ttu-id="f9a1e-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9a1e-139">Here is a JSON representation of the resource.</span></span>
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



