---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 520b21445d4c5a61755ddc78c65b9999a7e45ff0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027493"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="f9d5d-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f9d5d-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="f9d5d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f9d5d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9d5d-105">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="f9d5d-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="f9d5d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9d5d-106">Properties</span></span>
|<span data-ttu-id="f9d5d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9d5d-107">Property</span></span>|<span data-ttu-id="f9d5d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9d5d-108">Type</span></span>|<span data-ttu-id="f9d5d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9d5d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9d5d-110">inventory</span><span class="sxs-lookup"><span data-stu-id="f9d5d-110">inventory</span></span>|<span data-ttu-id="f9d5d-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9d5d-111">Boolean</span></span>|<span data-ttu-id="f9d5d-112">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="f9d5d-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="f9d5d-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="f9d5d-113">modernApps</span></span>|<span data-ttu-id="f9d5d-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9d5d-114">Boolean</span></span>|<span data-ttu-id="f9d5d-115">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="f9d5d-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="f9d5d-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="f9d5d-116">resourceAccess</span></span>|<span data-ttu-id="f9d5d-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9d5d-117">Boolean</span></span>|<span data-ttu-id="f9d5d-118">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="f9d5d-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="f9d5d-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9d5d-119">deviceConfiguration</span></span>|<span data-ttu-id="f9d5d-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9d5d-120">Boolean</span></span>|<span data-ttu-id="f9d5d-121">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="f9d5d-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="f9d5d-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f9d5d-122">compliancePolicy</span></span>|<span data-ttu-id="f9d5d-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9d5d-123">Boolean</span></span>|<span data-ttu-id="f9d5d-124">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="f9d5d-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="f9d5d-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="f9d5d-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="f9d5d-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9d5d-126">Boolean</span></span>|<span data-ttu-id="f9d5d-127">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="f9d5d-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9d5d-128">Relações</span><span class="sxs-lookup"><span data-stu-id="f9d5d-128">Relationships</span></span>
<span data-ttu-id="f9d5d-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f9d5d-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9d5d-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9d5d-130">JSON Representation</span></span>
<span data-ttu-id="f9d5d-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9d5d-131">Here is a JSON representation of the resource.</span></span>
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
  "windowsUpdateForBusiness": true
}
```



