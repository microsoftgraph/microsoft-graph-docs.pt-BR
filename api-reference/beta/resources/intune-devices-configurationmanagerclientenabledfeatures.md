---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a90b7f0009b4d9bd617b781338ceee3de2f432c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787922"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="0f837-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0f837-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="0f837-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f837-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f837-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f837-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f837-106">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="0f837-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="0f837-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f837-107">Properties</span></span>
|<span data-ttu-id="0f837-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f837-108">Property</span></span>|<span data-ttu-id="0f837-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f837-109">Type</span></span>|<span data-ttu-id="0f837-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f837-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f837-111">inventory</span><span class="sxs-lookup"><span data-stu-id="0f837-111">inventory</span></span>|<span data-ttu-id="0f837-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f837-112">Boolean</span></span>|<span data-ttu-id="0f837-113">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="0f837-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="0f837-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="0f837-114">modernApps</span></span>|<span data-ttu-id="0f837-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f837-115">Boolean</span></span>|<span data-ttu-id="0f837-116">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="0f837-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="0f837-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="0f837-117">resourceAccess</span></span>|<span data-ttu-id="0f837-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f837-118">Boolean</span></span>|<span data-ttu-id="0f837-119">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="0f837-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="0f837-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f837-120">deviceConfiguration</span></span>|<span data-ttu-id="0f837-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f837-121">Boolean</span></span>|<span data-ttu-id="0f837-122">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="0f837-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="0f837-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0f837-123">compliancePolicy</span></span>|<span data-ttu-id="0f837-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f837-124">Boolean</span></span>|<span data-ttu-id="0f837-125">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="0f837-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="0f837-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="0f837-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="0f837-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f837-127">Boolean</span></span>|<span data-ttu-id="0f837-128">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="0f837-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="0f837-129">endpointProtection</span><span class="sxs-lookup"><span data-stu-id="0f837-129">endpointProtection</span></span>|<span data-ttu-id="0f837-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f837-130">Boolean</span></span>|<span data-ttu-id="0f837-131">Se o Endpoint Protection é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="0f837-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="0f837-132">Officetreinamento</span><span class="sxs-lookup"><span data-stu-id="0f837-132">officeApps</span></span>|<span data-ttu-id="0f837-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f837-133">Boolean</span></span>|<span data-ttu-id="0f837-134">Se o aplicativo do Office é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="0f837-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f837-135">Relações</span><span class="sxs-lookup"><span data-stu-id="0f837-135">Relationships</span></span>
<span data-ttu-id="0f837-136">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0f837-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f837-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f837-137">JSON Representation</span></span>
<span data-ttu-id="0f837-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f837-138">Here is a JSON representation of the resource.</span></span>
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





