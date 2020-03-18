---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ce366adec1bcab58df761a6a271a45fbd0510c03
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785067"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="207fc-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="207fc-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="207fc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="207fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="207fc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="207fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="207fc-106">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="207fc-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="207fc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="207fc-107">Properties</span></span>
|<span data-ttu-id="207fc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="207fc-108">Property</span></span>|<span data-ttu-id="207fc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="207fc-109">Type</span></span>|<span data-ttu-id="207fc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="207fc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="207fc-111">inventory</span><span class="sxs-lookup"><span data-stu-id="207fc-111">inventory</span></span>|<span data-ttu-id="207fc-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="207fc-112">Boolean</span></span>|<span data-ttu-id="207fc-113">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="207fc-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="207fc-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="207fc-114">modernApps</span></span>|<span data-ttu-id="207fc-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="207fc-115">Boolean</span></span>|<span data-ttu-id="207fc-116">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="207fc-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="207fc-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="207fc-117">resourceAccess</span></span>|<span data-ttu-id="207fc-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="207fc-118">Boolean</span></span>|<span data-ttu-id="207fc-119">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="207fc-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="207fc-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="207fc-120">deviceConfiguration</span></span>|<span data-ttu-id="207fc-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="207fc-121">Boolean</span></span>|<span data-ttu-id="207fc-122">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="207fc-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="207fc-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="207fc-123">compliancePolicy</span></span>|<span data-ttu-id="207fc-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="207fc-124">Boolean</span></span>|<span data-ttu-id="207fc-125">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="207fc-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="207fc-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="207fc-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="207fc-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="207fc-127">Boolean</span></span>|<span data-ttu-id="207fc-128">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="207fc-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="207fc-129">endpointProtection</span><span class="sxs-lookup"><span data-stu-id="207fc-129">endpointProtection</span></span>|<span data-ttu-id="207fc-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="207fc-130">Boolean</span></span>|<span data-ttu-id="207fc-131">Se o Endpoint Protection é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="207fc-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="207fc-132">Officetreinamento</span><span class="sxs-lookup"><span data-stu-id="207fc-132">officeApps</span></span>|<span data-ttu-id="207fc-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="207fc-133">Boolean</span></span>|<span data-ttu-id="207fc-134">Se o aplicativo do Office é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="207fc-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="207fc-135">Relações</span><span class="sxs-lookup"><span data-stu-id="207fc-135">Relationships</span></span>
<span data-ttu-id="207fc-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="207fc-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="207fc-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="207fc-137">JSON Representation</span></span>
<span data-ttu-id="207fc-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="207fc-138">Here is a JSON representation of the resource.</span></span>
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



