---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da8a32960b1a8e82f60161e329abcf68916b4f37
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451269"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="41b85-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="41b85-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="41b85-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41b85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41b85-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41b85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41b85-106">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="41b85-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="41b85-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41b85-107">Properties</span></span>
|<span data-ttu-id="41b85-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41b85-108">Property</span></span>|<span data-ttu-id="41b85-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="41b85-109">Type</span></span>|<span data-ttu-id="41b85-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="41b85-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41b85-111">inventory</span><span class="sxs-lookup"><span data-stu-id="41b85-111">inventory</span></span>|<span data-ttu-id="41b85-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="41b85-112">Boolean</span></span>|<span data-ttu-id="41b85-113">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="41b85-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="41b85-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="41b85-114">modernApps</span></span>|<span data-ttu-id="41b85-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="41b85-115">Boolean</span></span>|<span data-ttu-id="41b85-116">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="41b85-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="41b85-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="41b85-117">resourceAccess</span></span>|<span data-ttu-id="41b85-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="41b85-118">Boolean</span></span>|<span data-ttu-id="41b85-119">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="41b85-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="41b85-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="41b85-120">deviceConfiguration</span></span>|<span data-ttu-id="41b85-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="41b85-121">Boolean</span></span>|<span data-ttu-id="41b85-122">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="41b85-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="41b85-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="41b85-123">compliancePolicy</span></span>|<span data-ttu-id="41b85-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="41b85-124">Boolean</span></span>|<span data-ttu-id="41b85-125">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="41b85-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="41b85-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="41b85-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="41b85-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="41b85-127">Boolean</span></span>|<span data-ttu-id="41b85-128">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="41b85-128">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="41b85-129">Relações</span><span class="sxs-lookup"><span data-stu-id="41b85-129">Relationships</span></span>
<span data-ttu-id="41b85-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41b85-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41b85-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41b85-131">JSON Representation</span></span>
<span data-ttu-id="41b85-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41b85-132">Here is a JSON representation of the resource.</span></span>
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







