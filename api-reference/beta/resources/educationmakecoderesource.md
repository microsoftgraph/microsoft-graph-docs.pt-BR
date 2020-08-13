---
title: tipo de recurso educationMakeCodeResource
description: Um recurso MakeCode
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 708efc4e72abeba9ff0acfe6e4768c61518e1a6b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501707"
---
# <a name="educationmakecoderesource-resource-type"></a><span data-ttu-id="3140a-103">tipo de recurso educationMakeCodeResource</span><span class="sxs-lookup"><span data-stu-id="3140a-103">educationMakeCodeResource resource type</span></span>

<span data-ttu-id="3140a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3140a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3140a-105">Um recurso representando um projeto [MakeCode](https://www.microsoft.com/en-us/makecode) .</span><span class="sxs-lookup"><span data-stu-id="3140a-105">A resource representing a [MakeCode](https://www.microsoft.com/en-us/makecode) project.</span></span>

## <a name="properties"></a><span data-ttu-id="3140a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3140a-106">Properties</span></span>

| <span data-ttu-id="3140a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3140a-107">Property</span></span>     | <span data-ttu-id="3140a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3140a-108">Type</span></span>        | <span data-ttu-id="3140a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3140a-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3140a-110">projectId</span><span class="sxs-lookup"><span data-stu-id="3140a-110">projectId</span></span>|<span data-ttu-id="3140a-111">String</span><span class="sxs-lookup"><span data-stu-id="3140a-111">String</span></span>|<span data-ttu-id="3140a-112">ID do projeto MakeCode</span><span class="sxs-lookup"><span data-stu-id="3140a-112">ID of the MakeCode project</span></span>|
|<span data-ttu-id="3140a-113">hostWebUrl</span><span class="sxs-lookup"><span data-stu-id="3140a-113">hostWebUrl</span></span>|<span data-ttu-id="3140a-114">String</span><span class="sxs-lookup"><span data-stu-id="3140a-114">String</span></span>|<span data-ttu-id="3140a-115">Host para o tipo de recurso MakeCode (por exemplo,, MICROBIT)</span><span class="sxs-lookup"><span data-stu-id="3140a-115">Host for the type of MakeCode resource (for example, arcade, microbit)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3140a-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3140a-116">JSON representation</span></span>

<span data-ttu-id="3140a-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3140a-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationMakeCodeResource",
  "baseType": "microsoft.graph.educationResource"
}-->

```json
{
  "projectId": "String",
  "hostWebUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationMakeCodeResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->