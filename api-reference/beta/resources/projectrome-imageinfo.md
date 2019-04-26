---
title: tipo de recurso imageInfo
description: Um tipo complexo para representar a propriedade de **atribuição** na parte visualInfo do objeto Activity.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 6ffdacefb11f583f8c9529a36472a01537643c3c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344001"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="bbefc-103">tipo de recurso imageInfo</span><span class="sxs-lookup"><span data-stu-id="bbefc-103">imageInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbefc-104">Um tipo complexo para representar a propriedade de **atribuição** na parte [visualInfo](../resources/projectrome-visualinfo.md) do objeto [Activity](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="bbefc-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="bbefc-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bbefc-105">Properties</span></span>

|<span data-ttu-id="bbefc-106">Nome</span><span class="sxs-lookup"><span data-stu-id="bbefc-106">Name</span></span> | <span data-ttu-id="bbefc-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbefc-107">Type</span></span> | <span data-ttu-id="bbefc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbefc-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="bbefc-109">iconUrl</span><span class="sxs-lookup"><span data-stu-id="bbefc-109">iconUrl</span></span> | <span data-ttu-id="bbefc-110">String</span><span class="sxs-lookup"><span data-stu-id="bbefc-110">String</span></span> | <span data-ttu-id="bbefc-111">Opcion URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade</span><span class="sxs-lookup"><span data-stu-id="bbefc-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="bbefc-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="bbefc-112">alternateText</span></span> | <span data-ttu-id="bbefc-113">String</span><span class="sxs-lookup"><span data-stu-id="bbefc-113">String</span></span> | <span data-ttu-id="bbefc-114">Opcion Alt-conteúdo de texto acessível para a imagem</span><span class="sxs-lookup"><span data-stu-id="bbefc-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="bbefc-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="bbefc-115">addImageQuery</span></span> | <span data-ttu-id="bbefc-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbefc-116">Boolean</span></span> | <span data-ttu-id="bbefc-117">Opcion parâmetro usado para indicar que o servidor é capaz de renderizar a imagem dinamicamente em resposta à parametrização.</span><span class="sxs-lookup"><span data-stu-id="bbefc-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="bbefc-118">Por exemplo, uma imagem de alto contraste</span><span class="sxs-lookup"><span data-stu-id="bbefc-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bbefc-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bbefc-119">JSON Representation</span></span>

<span data-ttu-id="bbefc-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bbefc-120">Here is a JSON representation of the resource</span></span>

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
