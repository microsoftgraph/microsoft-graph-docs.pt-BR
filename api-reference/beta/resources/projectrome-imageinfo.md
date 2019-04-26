---
title: tipo de recurso imageInfo
description: Um tipo complexo para representar a propriedade de **atribuição** na parte visualInfo do objeto Activity.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 112b1dc3d1db45f3fe470c1c21d483b09c00202c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563279"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="4ba82-103">tipo de recurso imageInfo</span><span class="sxs-lookup"><span data-stu-id="4ba82-103">imageInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ba82-104">Um tipo complexo para representar a propriedade de **atribuição** na parte [visualInfo](../resources/projectrome-visualinfo.md) do objeto [Activity](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="4ba82-104">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="4ba82-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ba82-105">Properties</span></span>

|<span data-ttu-id="4ba82-106">Nome</span><span class="sxs-lookup"><span data-stu-id="4ba82-106">Name</span></span> | <span data-ttu-id="4ba82-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ba82-107">Type</span></span> | <span data-ttu-id="4ba82-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ba82-108">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="4ba82-109">iconUrl</span><span class="sxs-lookup"><span data-stu-id="4ba82-109">iconUrl</span></span> | <span data-ttu-id="4ba82-110">String</span><span class="sxs-lookup"><span data-stu-id="4ba82-110">String</span></span> | <span data-ttu-id="4ba82-111">Opcion URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade</span><span class="sxs-lookup"><span data-stu-id="4ba82-111">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="4ba82-112">alternateText</span><span class="sxs-lookup"><span data-stu-id="4ba82-112">alternateText</span></span> | <span data-ttu-id="4ba82-113">String</span><span class="sxs-lookup"><span data-stu-id="4ba82-113">String</span></span> | <span data-ttu-id="4ba82-114">Opcion Alt-conteúdo de texto acessível para a imagem</span><span class="sxs-lookup"><span data-stu-id="4ba82-114">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="4ba82-115">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="4ba82-115">addImageQuery</span></span> | <span data-ttu-id="4ba82-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="4ba82-116">Boolean</span></span> | <span data-ttu-id="4ba82-117">Opcion parâmetro usado para indicar que o servidor é capaz de renderizar a imagem dinamicamente em resposta à parametrização.</span><span class="sxs-lookup"><span data-stu-id="4ba82-117">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="4ba82-118">Por exemplo, uma imagem de alto contraste</span><span class="sxs-lookup"><span data-stu-id="4ba82-118">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ba82-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ba82-119">JSON Representation</span></span>

<span data-ttu-id="4ba82-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="4ba82-120">Here is a JSON representation of the resource</span></span>

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
