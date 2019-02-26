---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed376bc616c26f1ad6e8a3ea06d3898c051e8d0b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148773"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="e1369-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="e1369-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="e1369-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1369-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1369-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1369-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1369-106">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="e1369-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="e1369-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1369-107">Properties</span></span>
|<span data-ttu-id="e1369-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1369-108">Property</span></span>|<span data-ttu-id="e1369-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1369-109">Type</span></span>|<span data-ttu-id="e1369-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1369-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1369-111">inventory</span><span class="sxs-lookup"><span data-stu-id="e1369-111">inventory</span></span>|<span data-ttu-id="e1369-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1369-112">Boolean</span></span>|<span data-ttu-id="e1369-113">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="e1369-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="e1369-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="e1369-114">modernApps</span></span>|<span data-ttu-id="e1369-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1369-115">Boolean</span></span>|<span data-ttu-id="e1369-116">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="e1369-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="e1369-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="e1369-117">resourceAccess</span></span>|<span data-ttu-id="e1369-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1369-118">Boolean</span></span>|<span data-ttu-id="e1369-119">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="e1369-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="e1369-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1369-120">deviceConfiguration</span></span>|<span data-ttu-id="e1369-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1369-121">Boolean</span></span>|<span data-ttu-id="e1369-122">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="e1369-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="e1369-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e1369-123">compliancePolicy</span></span>|<span data-ttu-id="e1369-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1369-124">Boolean</span></span>|<span data-ttu-id="e1369-125">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="e1369-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="e1369-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="e1369-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="e1369-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="e1369-127">Boolean</span></span>|<span data-ttu-id="e1369-128">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="e1369-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="e1369-129">endpointProtection</span><span class="sxs-lookup"><span data-stu-id="e1369-129">endpointProtection</span></span>|<span data-ttu-id="e1369-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1369-130">Boolean</span></span>|<span data-ttu-id="e1369-131">Se o Endpoint Protection é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="e1369-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="e1369-132">Officetreinamento</span><span class="sxs-lookup"><span data-stu-id="e1369-132">officeApps</span></span>|<span data-ttu-id="e1369-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1369-133">Boolean</span></span>|<span data-ttu-id="e1369-134">Se o aplicativo do Office é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="e1369-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1369-135">Relações</span><span class="sxs-lookup"><span data-stu-id="e1369-135">Relationships</span></span>
<span data-ttu-id="e1369-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1369-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1369-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1369-137">JSON Representation</span></span>
<span data-ttu-id="e1369-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1369-138">Here is a JSON representation of the resource.</span></span>
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




