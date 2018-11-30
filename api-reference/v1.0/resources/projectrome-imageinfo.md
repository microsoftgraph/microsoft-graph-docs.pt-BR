---
title: tipo de recurso de imageInfo
description: Um tipo complexo para representar a propriedade **atribuição** na parte visualInfo do objeto atividade.
ms.openlocfilehash: 051338230850da7e754c5e8ad4f7d9c52fe17b32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006364"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="4496a-103">tipo de recurso de imageInfo</span><span class="sxs-lookup"><span data-stu-id="4496a-103">imageInfo resource type</span></span>

<span data-ttu-id="4496a-104">Um tipo complexo para representar a propriedade **atribuição** na parte [visualInfo](../resources/projectrome-visualinfo.md) do objeto [atividade](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="4496a-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="4496a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4496a-105">Properties</span></span>

|<span data-ttu-id="4496a-106">Nome</span><span class="sxs-lookup"><span data-stu-id="4496a-106">Name</span></span> | <span data-ttu-id="4496a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4496a-107">Type</span></span> | <span data-ttu-id="4496a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4496a-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="4496a-109">iconUrl</span><span class="sxs-lookup"><span data-stu-id="4496a-109">iconUrl</span></span> | <span data-ttu-id="4496a-110">String</span><span class="sxs-lookup"><span data-stu-id="4496a-110">String</span></span> | <span data-ttu-id="4496a-111">Opcional; URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade</span><span class="sxs-lookup"><span data-stu-id="4496a-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="4496a-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="4496a-112">alternateText</span></span> | <span data-ttu-id="4496a-113">String</span><span class="sxs-lookup"><span data-stu-id="4496a-113">String</span></span> | <span data-ttu-id="4496a-114">Opcional; conteúdo de texto ALT acessível para a imagem</span><span class="sxs-lookup"><span data-stu-id="4496a-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="4496a-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="4496a-115">addImageQuery</span></span> | <span data-ttu-id="4496a-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="4496a-116">Boolean</span></span> | <span data-ttu-id="4496a-117">Opcional; parâmetro usado para indicar o servidor é capaz de processar imagem dinamicamente em resposta às parametrização.</span><span class="sxs-lookup"><span data-stu-id="4496a-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="4496a-118">Por exemplo, – uma imagem de alto contraste</span><span class="sxs-lookup"><span data-stu-id="4496a-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4496a-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4496a-119">JSON Representation</span></span>

<span data-ttu-id="4496a-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="4496a-120">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->