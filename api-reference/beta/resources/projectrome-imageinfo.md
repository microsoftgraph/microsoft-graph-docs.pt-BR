---
title: tipo de recurso imageInfo
description: Um tipo complexo para representar a propriedade de **atribuição** na parte visualInfo do objeto Activity.
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ailae
ms.openlocfilehash: a57155a880e9ba4e00dd9a4d17ddae3742bbaa8e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807476"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="7a6f2-103">tipo de recurso imageInfo</span><span class="sxs-lookup"><span data-stu-id="7a6f2-103">imageInfo resource type</span></span>

<span data-ttu-id="7a6f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a6f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a6f2-105">Um tipo complexo para representar a propriedade de **atribuição** na parte [visualInfo](../resources/projectrome-visualinfo.md) do objeto [Activity](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="7a6f2-105">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="7a6f2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a6f2-106">Properties</span></span>

|<span data-ttu-id="7a6f2-107">Nome</span><span class="sxs-lookup"><span data-stu-id="7a6f2-107">Name</span></span> | <span data-ttu-id="7a6f2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a6f2-108">Type</span></span> | <span data-ttu-id="7a6f2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a6f2-109">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="7a6f2-110">iconUrl</span><span class="sxs-lookup"><span data-stu-id="7a6f2-110">iconUrl</span></span> | <span data-ttu-id="7a6f2-111">String</span><span class="sxs-lookup"><span data-stu-id="7a6f2-111">String</span></span> | <span data-ttu-id="7a6f2-112">Opcion URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade</span><span class="sxs-lookup"><span data-stu-id="7a6f2-112">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="7a6f2-113">alternateText</span><span class="sxs-lookup"><span data-stu-id="7a6f2-113">alternateText</span></span> | <span data-ttu-id="7a6f2-114">String</span><span class="sxs-lookup"><span data-stu-id="7a6f2-114">String</span></span> | <span data-ttu-id="7a6f2-115">Opcion Alt-conteúdo de texto acessível para a imagem</span><span class="sxs-lookup"><span data-stu-id="7a6f2-115">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="7a6f2-116">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="7a6f2-116">addImageQuery</span></span> | <span data-ttu-id="7a6f2-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="7a6f2-117">Boolean</span></span> | <span data-ttu-id="7a6f2-118">Opcion parâmetro usado para indicar que o servidor é capaz de renderizar a imagem dinamicamente em resposta à parametrização.</span><span class="sxs-lookup"><span data-stu-id="7a6f2-118">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="7a6f2-119">Por exemplo, uma imagem de alto contraste</span><span class="sxs-lookup"><span data-stu-id="7a6f2-119">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a6f2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a6f2-120">JSON Representation</span></span>

<span data-ttu-id="7a6f2-121">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7a6f2-121">Here is a JSON representation of the resource</span></span>

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
