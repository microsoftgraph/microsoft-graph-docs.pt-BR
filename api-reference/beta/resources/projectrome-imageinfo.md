---
title: tipo de recurso de imageInfo
description: Um tipo complexo para representar a propriedade **atribuição** na parte visualInfo do objeto atividade.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 112b1dc3d1db45f3fe470c1c21d483b09c00202c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514912"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="7baa4-103">tipo de recurso de imageInfo</span><span class="sxs-lookup"><span data-stu-id="7baa4-103">imageInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7baa4-104">Um tipo complexo para representar a propriedade **atribuição** na parte [visualInfo](../resources/projectrome-visualinfo.md) do objeto [atividade](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="7baa4-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="7baa4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7baa4-105">Properties</span></span>

|<span data-ttu-id="7baa4-106">Nome</span><span class="sxs-lookup"><span data-stu-id="7baa4-106">Name</span></span> | <span data-ttu-id="7baa4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7baa4-107">Type</span></span> | <span data-ttu-id="7baa4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7baa4-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="7baa4-109">IconUrl</span><span class="sxs-lookup"><span data-stu-id="7baa4-109">iconUrl</span></span> | <span data-ttu-id="7baa4-110">String</span><span class="sxs-lookup"><span data-stu-id="7baa4-110">String</span></span> | <span data-ttu-id="7baa4-111">Opcional; URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade</span><span class="sxs-lookup"><span data-stu-id="7baa4-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="7baa4-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="7baa4-112">alternateText</span></span> | <span data-ttu-id="7baa4-113">String</span><span class="sxs-lookup"><span data-stu-id="7baa4-113">String</span></span> | <span data-ttu-id="7baa4-114">Opcional; conteúdo de texto ALT acessível para a imagem</span><span class="sxs-lookup"><span data-stu-id="7baa4-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="7baa4-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="7baa4-115">addImageQuery</span></span> | <span data-ttu-id="7baa4-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="7baa4-116">Boolean</span></span> | <span data-ttu-id="7baa4-117">Opcional; parâmetro usado para indicar o servidor é capaz de processar imagem dinamicamente em resposta às parametrização.</span><span class="sxs-lookup"><span data-stu-id="7baa4-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="7baa4-118">Por exemplo, – uma imagem de alto contraste</span><span class="sxs-lookup"><span data-stu-id="7baa4-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7baa4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7baa4-119">JSON Representation</span></span>

<span data-ttu-id="7baa4-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7baa4-120">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-imageinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
