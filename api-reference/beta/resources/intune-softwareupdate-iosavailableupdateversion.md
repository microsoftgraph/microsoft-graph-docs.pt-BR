---
title: tipo de recurso iosAvailableUpdateVersion
description: detalhes da versão da atualização disponível do iOS
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91fa2d9d6c770d67b185d94c91200ce6fc5b23b7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455027"
---
# <a name="iosavailableupdateversion-resource-type"></a><span data-ttu-id="79292-103">tipo de recurso iosAvailableUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="79292-103">iosAvailableUpdateVersion resource type</span></span>

<span data-ttu-id="79292-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79292-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79292-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79292-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79292-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79292-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79292-107">detalhes da versão da atualização disponível do iOS</span><span class="sxs-lookup"><span data-stu-id="79292-107">iOS available update version details</span></span>

## <a name="properties"></a><span data-ttu-id="79292-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79292-108">Properties</span></span>
|<span data-ttu-id="79292-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79292-109">Property</span></span>|<span data-ttu-id="79292-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="79292-110">Type</span></span>|<span data-ttu-id="79292-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="79292-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79292-112">productVersion</span><span class="sxs-lookup"><span data-stu-id="79292-112">productVersion</span></span>|<span data-ttu-id="79292-113">String</span><span class="sxs-lookup"><span data-stu-id="79292-113">String</span></span>|<span data-ttu-id="79292-114">A versão da atualização.</span><span class="sxs-lookup"><span data-stu-id="79292-114">The version of the update.</span></span>|
|<span data-ttu-id="79292-115">postingDateTime</span><span class="sxs-lookup"><span data-stu-id="79292-115">postingDateTime</span></span>|<span data-ttu-id="79292-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79292-116">DateTimeOffset</span></span>|<span data-ttu-id="79292-117">A data de lançamento da atualização.</span><span class="sxs-lookup"><span data-stu-id="79292-117">The posting date of the update.</span></span>|
|<span data-ttu-id="79292-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="79292-118">expirationDateTime</span></span>|<span data-ttu-id="79292-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79292-119">DateTimeOffset</span></span>|<span data-ttu-id="79292-120">A data de expiração da atualização.</span><span class="sxs-lookup"><span data-stu-id="79292-120">The expiration date of the update.</span></span>|
|<span data-ttu-id="79292-121">supportedDevices</span><span class="sxs-lookup"><span data-stu-id="79292-121">supportedDevices</span></span>|<span data-ttu-id="79292-122">Coleção String</span><span class="sxs-lookup"><span data-stu-id="79292-122">String collection</span></span>|<span data-ttu-id="79292-123">Lista de dispositivos com suporte para a atualização.</span><span class="sxs-lookup"><span data-stu-id="79292-123">List of supported devices for the update.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79292-124">Relações</span><span class="sxs-lookup"><span data-stu-id="79292-124">Relationships</span></span>
<span data-ttu-id="79292-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79292-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79292-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79292-126">JSON Representation</span></span>
<span data-ttu-id="79292-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79292-127">Here is a JSON representation of the resource.</span></span>
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



