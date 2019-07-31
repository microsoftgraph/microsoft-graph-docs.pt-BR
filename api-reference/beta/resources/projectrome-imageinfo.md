---
title: tipo de recurso imageInfo
description: Um tipo complexo para representar a propriedade de **atribuição** na parte visualInfo do objeto Activity.
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 53496734f79121edd010a429ec0a8da28b16e836
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008884"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="56893-103">tipo de recurso imageInfo</span><span class="sxs-lookup"><span data-stu-id="56893-103">imageInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56893-104">Um tipo complexo para representar a propriedade de **atribuição** na parte [visualInfo](../resources/projectrome-visualinfo.md) do objeto [Activity](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="56893-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="56893-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56893-105">Properties</span></span>

|<span data-ttu-id="56893-106">Nome</span><span class="sxs-lookup"><span data-stu-id="56893-106">Name</span></span> | <span data-ttu-id="56893-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="56893-107">Type</span></span> | <span data-ttu-id="56893-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="56893-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="56893-109">iconUrl</span><span class="sxs-lookup"><span data-stu-id="56893-109">iconUrl</span></span> | <span data-ttu-id="56893-110">String</span><span class="sxs-lookup"><span data-stu-id="56893-110">String</span></span> | <span data-ttu-id="56893-111">Opcion URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade</span><span class="sxs-lookup"><span data-stu-id="56893-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="56893-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="56893-112">alternateText</span></span> | <span data-ttu-id="56893-113">String</span><span class="sxs-lookup"><span data-stu-id="56893-113">String</span></span> | <span data-ttu-id="56893-114">Opcion Alt-conteúdo de texto acessível para a imagem</span><span class="sxs-lookup"><span data-stu-id="56893-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="56893-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="56893-115">addImageQuery</span></span> | <span data-ttu-id="56893-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="56893-116">Boolean</span></span> | <span data-ttu-id="56893-117">Opcion parâmetro usado para indicar que o servidor é capaz de renderizar a imagem dinamicamente em resposta à parametrização.</span><span class="sxs-lookup"><span data-stu-id="56893-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="56893-118">Por exemplo, uma imagem de alto contraste</span><span class="sxs-lookup"><span data-stu-id="56893-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56893-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56893-119">JSON Representation</span></span>

<span data-ttu-id="56893-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="56893-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
