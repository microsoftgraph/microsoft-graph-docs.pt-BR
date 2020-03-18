---
title: tipo de recurso iosAvailableUpdateVersion
description: detalhes da versão da atualização disponível do iOS
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 29cf7500bc7069af0b2a1184adb0fe28bb0ac891
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42766361"
---
# <a name="iosavailableupdateversion-resource-type"></a><span data-ttu-id="6d205-103">tipo de recurso iosAvailableUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="6d205-103">iosAvailableUpdateVersion resource type</span></span>

> <span data-ttu-id="6d205-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d205-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d205-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d205-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d205-106">detalhes da versão da atualização disponível do iOS</span><span class="sxs-lookup"><span data-stu-id="6d205-106">iOS available update version details</span></span>

## <a name="properties"></a><span data-ttu-id="6d205-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d205-107">Properties</span></span>
|<span data-ttu-id="6d205-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d205-108">Property</span></span>|<span data-ttu-id="6d205-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d205-109">Type</span></span>|<span data-ttu-id="6d205-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d205-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d205-111">productVersion</span><span class="sxs-lookup"><span data-stu-id="6d205-111">productVersion</span></span>|<span data-ttu-id="6d205-112">String</span><span class="sxs-lookup"><span data-stu-id="6d205-112">String</span></span>|<span data-ttu-id="6d205-113">A versão da atualização.</span><span class="sxs-lookup"><span data-stu-id="6d205-113">The version of the update.</span></span>|
|<span data-ttu-id="6d205-114">postingDateTime</span><span class="sxs-lookup"><span data-stu-id="6d205-114">postingDateTime</span></span>|<span data-ttu-id="6d205-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d205-115">DateTimeOffset</span></span>|<span data-ttu-id="6d205-116">A data de lançamento da atualização.</span><span class="sxs-lookup"><span data-stu-id="6d205-116">The posting date of the update.</span></span>|
|<span data-ttu-id="6d205-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6d205-117">expirationDateTime</span></span>|<span data-ttu-id="6d205-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d205-118">DateTimeOffset</span></span>|<span data-ttu-id="6d205-119">A data de expiração da atualização.</span><span class="sxs-lookup"><span data-stu-id="6d205-119">The expiration date of the update.</span></span>|
|<span data-ttu-id="6d205-120">supportedDevices</span><span class="sxs-lookup"><span data-stu-id="6d205-120">supportedDevices</span></span>|<span data-ttu-id="6d205-121">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d205-121">String collection</span></span>|<span data-ttu-id="6d205-122">Lista de dispositivos com suporte para a atualização.</span><span class="sxs-lookup"><span data-stu-id="6d205-122">List of supported devices for the update.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d205-123">Relações</span><span class="sxs-lookup"><span data-stu-id="6d205-123">Relationships</span></span>
<span data-ttu-id="6d205-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6d205-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d205-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d205-125">JSON Representation</span></span>
<span data-ttu-id="6d205-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d205-126">Here is a JSON representation of the resource.</span></span>
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



