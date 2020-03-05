---
title: tipo de recurso iosAvailableUpdateVersion
description: detalhes da versão da atualização disponível do iOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b2174e13cf80e39e1f63f7fb03da6e9b305add30
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523440"
---
# <a name="iosavailableupdateversion-resource-type"></a><span data-ttu-id="37882-103">tipo de recurso iosAvailableUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="37882-103">iosAvailableUpdateVersion resource type</span></span>

<span data-ttu-id="37882-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="37882-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37882-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37882-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37882-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37882-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37882-107">detalhes da versão da atualização disponível do iOS</span><span class="sxs-lookup"><span data-stu-id="37882-107">iOS available update version details</span></span>

## <a name="properties"></a><span data-ttu-id="37882-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37882-108">Properties</span></span>
|<span data-ttu-id="37882-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37882-109">Property</span></span>|<span data-ttu-id="37882-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="37882-110">Type</span></span>|<span data-ttu-id="37882-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="37882-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37882-112">productVersion</span><span class="sxs-lookup"><span data-stu-id="37882-112">productVersion</span></span>|<span data-ttu-id="37882-113">String</span><span class="sxs-lookup"><span data-stu-id="37882-113">String</span></span>|<span data-ttu-id="37882-114">A versão da atualização.</span><span class="sxs-lookup"><span data-stu-id="37882-114">The version of the update.</span></span>|
|<span data-ttu-id="37882-115">postingDateTime</span><span class="sxs-lookup"><span data-stu-id="37882-115">postingDateTime</span></span>|<span data-ttu-id="37882-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37882-116">DateTimeOffset</span></span>|<span data-ttu-id="37882-117">A data de lançamento da atualização.</span><span class="sxs-lookup"><span data-stu-id="37882-117">The posting date of the update.</span></span>|
|<span data-ttu-id="37882-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="37882-118">expirationDateTime</span></span>|<span data-ttu-id="37882-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37882-119">DateTimeOffset</span></span>|<span data-ttu-id="37882-120">A data de expiração da atualização.</span><span class="sxs-lookup"><span data-stu-id="37882-120">The expiration date of the update.</span></span>|
|<span data-ttu-id="37882-121">supportedDevices</span><span class="sxs-lookup"><span data-stu-id="37882-121">supportedDevices</span></span>|<span data-ttu-id="37882-122">String collection</span><span class="sxs-lookup"><span data-stu-id="37882-122">String collection</span></span>|<span data-ttu-id="37882-123">Lista de dispositivos com suporte para a atualização.</span><span class="sxs-lookup"><span data-stu-id="37882-123">List of supported devices for the update.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37882-124">Relações</span><span class="sxs-lookup"><span data-stu-id="37882-124">Relationships</span></span>
<span data-ttu-id="37882-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37882-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37882-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37882-126">JSON Representation</span></span>
<span data-ttu-id="37882-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37882-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAvailableUpdateVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAvailableUpdateVersion",
  "productVersion": "String",
  "postingDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "supportedDevices": [
    "String"
  ]
}
```



