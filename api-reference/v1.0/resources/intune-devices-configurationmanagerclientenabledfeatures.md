---
title: Tipo de recurso configurationManagerClientEnabledFeatures
description: recursos habilitados pelo cliente do Gerenciador de Configurações
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3e8622f6f1772948295f9389cf97aef0b6f260e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533306"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="efa23-103">Tipo de recurso configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="efa23-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="efa23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efa23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efa23-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="efa23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efa23-106">recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="efa23-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="efa23-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="efa23-107">Properties</span></span>
|<span data-ttu-id="efa23-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efa23-108">Property</span></span>|<span data-ttu-id="efa23-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="efa23-109">Type</span></span>|<span data-ttu-id="efa23-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="efa23-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efa23-111">inventory</span><span class="sxs-lookup"><span data-stu-id="efa23-111">inventory</span></span>|<span data-ttu-id="efa23-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="efa23-112">Boolean</span></span>|<span data-ttu-id="efa23-113">Se o estoque é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="efa23-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="efa23-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="efa23-114">modernApps</span></span>|<span data-ttu-id="efa23-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="efa23-115">Boolean</span></span>|<span data-ttu-id="efa23-116">Se o aplicativo moderno é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="efa23-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="efa23-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="efa23-117">resourceAccess</span></span>|<span data-ttu-id="efa23-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="efa23-118">Boolean</span></span>|<span data-ttu-id="efa23-119">Se o acesso ao recurso é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="efa23-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="efa23-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="efa23-120">deviceConfiguration</span></span>|<span data-ttu-id="efa23-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="efa23-121">Boolean</span></span>|<span data-ttu-id="efa23-122">Se a configuração do dispositivo é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="efa23-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="efa23-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="efa23-123">compliancePolicy</span></span>|<span data-ttu-id="efa23-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="efa23-124">Boolean</span></span>|<span data-ttu-id="efa23-125">Se a política de conformidade é gerenciada pelo Intune</span><span class="sxs-lookup"><span data-stu-id="efa23-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="efa23-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="efa23-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="efa23-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="efa23-127">Boolean</span></span>|<span data-ttu-id="efa23-128">Se o Windows Update para Empresas é gerenciado pelo Intune</span><span class="sxs-lookup"><span data-stu-id="efa23-128">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="efa23-129">Relações</span><span class="sxs-lookup"><span data-stu-id="efa23-129">Relationships</span></span>
<span data-ttu-id="efa23-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efa23-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efa23-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efa23-131">JSON Representation</span></span>
<span data-ttu-id="efa23-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="efa23-132">Here is a JSON representation of the resource.</span></span>
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




