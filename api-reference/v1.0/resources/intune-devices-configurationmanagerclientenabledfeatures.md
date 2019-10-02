---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c68fa195584c8d30cbe6a9b942a453b4f6a9218
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357035"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="a088b-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="a088b-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="a088b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a088b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a088b-105">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="a088b-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="a088b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a088b-106">Properties</span></span>
|<span data-ttu-id="a088b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a088b-107">Property</span></span>|<span data-ttu-id="a088b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a088b-108">Type</span></span>|<span data-ttu-id="a088b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a088b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a088b-110">inventory</span><span class="sxs-lookup"><span data-stu-id="a088b-110">inventory</span></span>|<span data-ttu-id="a088b-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="a088b-111">Boolean</span></span>|<span data-ttu-id="a088b-112">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="a088b-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="a088b-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="a088b-113">modernApps</span></span>|<span data-ttu-id="a088b-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="a088b-114">Boolean</span></span>|<span data-ttu-id="a088b-115">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="a088b-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="a088b-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="a088b-116">resourceAccess</span></span>|<span data-ttu-id="a088b-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="a088b-117">Boolean</span></span>|<span data-ttu-id="a088b-118">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="a088b-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="a088b-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a088b-119">deviceConfiguration</span></span>|<span data-ttu-id="a088b-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="a088b-120">Boolean</span></span>|<span data-ttu-id="a088b-121">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="a088b-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="a088b-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="a088b-122">compliancePolicy</span></span>|<span data-ttu-id="a088b-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="a088b-123">Boolean</span></span>|<span data-ttu-id="a088b-124">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="a088b-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="a088b-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="a088b-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="a088b-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="a088b-126">Boolean</span></span>|<span data-ttu-id="a088b-127">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="a088b-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="a088b-128">Relações</span><span class="sxs-lookup"><span data-stu-id="a088b-128">Relationships</span></span>
<span data-ttu-id="a088b-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a088b-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a088b-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a088b-130">JSON Representation</span></span>
<span data-ttu-id="a088b-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a088b-131">Here is a JSON representation of the resource.</span></span>
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




