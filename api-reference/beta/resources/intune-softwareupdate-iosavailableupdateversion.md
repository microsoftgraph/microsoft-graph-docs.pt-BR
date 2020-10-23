---
title: tipo de recurso iosAvailableUpdateVersion
description: detalhes da versão da atualização disponível do iOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f2b94a098c70b6d4ac4105b31274f406f058c675
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696045"
---
# <a name="iosavailableupdateversion-resource-type"></a><span data-ttu-id="151b5-103">tipo de recurso iosAvailableUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="151b5-103">iosAvailableUpdateVersion resource type</span></span>

<span data-ttu-id="151b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="151b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="151b5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="151b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="151b5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="151b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="151b5-107">detalhes da versão da atualização disponível do iOS</span><span class="sxs-lookup"><span data-stu-id="151b5-107">iOS available update version details</span></span>

## <a name="properties"></a><span data-ttu-id="151b5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="151b5-108">Properties</span></span>
|<span data-ttu-id="151b5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="151b5-109">Property</span></span>|<span data-ttu-id="151b5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="151b5-110">Type</span></span>|<span data-ttu-id="151b5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="151b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="151b5-112">productVersion</span><span class="sxs-lookup"><span data-stu-id="151b5-112">productVersion</span></span>|<span data-ttu-id="151b5-113">String</span><span class="sxs-lookup"><span data-stu-id="151b5-113">String</span></span>|<span data-ttu-id="151b5-114">A versão da atualização.</span><span class="sxs-lookup"><span data-stu-id="151b5-114">The version of the update.</span></span>|
|<span data-ttu-id="151b5-115">postingDateTime</span><span class="sxs-lookup"><span data-stu-id="151b5-115">postingDateTime</span></span>|<span data-ttu-id="151b5-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="151b5-116">DateTimeOffset</span></span>|<span data-ttu-id="151b5-117">A data de lançamento da atualização.</span><span class="sxs-lookup"><span data-stu-id="151b5-117">The posting date of the update.</span></span>|
|<span data-ttu-id="151b5-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="151b5-118">expirationDateTime</span></span>|<span data-ttu-id="151b5-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="151b5-119">DateTimeOffset</span></span>|<span data-ttu-id="151b5-120">A data de expiração da atualização.</span><span class="sxs-lookup"><span data-stu-id="151b5-120">The expiration date of the update.</span></span>|
|<span data-ttu-id="151b5-121">supportedDevices</span><span class="sxs-lookup"><span data-stu-id="151b5-121">supportedDevices</span></span>|<span data-ttu-id="151b5-122">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="151b5-122">String collection</span></span>|<span data-ttu-id="151b5-123">Lista de dispositivos com suporte para a atualização.</span><span class="sxs-lookup"><span data-stu-id="151b5-123">List of supported devices for the update.</span></span>|

## <a name="relationships"></a><span data-ttu-id="151b5-124">Relações</span><span class="sxs-lookup"><span data-stu-id="151b5-124">Relationships</span></span>
<span data-ttu-id="151b5-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="151b5-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="151b5-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="151b5-126">JSON Representation</span></span>
<span data-ttu-id="151b5-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="151b5-127">Here is a JSON representation of the resource.</span></span>
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





