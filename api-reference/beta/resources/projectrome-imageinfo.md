---
title: tipo de recurso de imageInfo
description: Um tipo complexo para representar a propriedade **atribuição** na parte visualInfo do objeto atividade.
ms.openlocfilehash: dbd04c5350d618540ebdffcb38a2bc11bfef6129
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039978"
---
# <a name="imageinfo-resource-type"></a><span data-ttu-id="75448-103">tipo de recurso de imageInfo</span><span class="sxs-lookup"><span data-stu-id="75448-103">imageInfo resource type</span></span>

> <span data-ttu-id="75448-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="75448-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75448-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="75448-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75448-106">Um tipo complexo para representar a propriedade **atribuição** na parte [visualInfo](../resources/projectrome-visualinfo.md) do objeto [atividade](../resources/projectrome-activity.md) .</span><span class="sxs-lookup"><span data-stu-id="75448-106">A complex type for representing the **attribution** property in the [visualInfo](../resources/projectrome-visualinfo.md) part of the [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="75448-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75448-107">Properties</span></span>

|<span data-ttu-id="75448-108">Nome</span><span class="sxs-lookup"><span data-stu-id="75448-108">Name</span></span> | <span data-ttu-id="75448-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="75448-109">Type</span></span> | <span data-ttu-id="75448-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="75448-110">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="75448-111">iconUrl</span><span class="sxs-lookup"><span data-stu-id="75448-111">iconUrl</span></span> | <span data-ttu-id="75448-112">String</span><span class="sxs-lookup"><span data-stu-id="75448-112">String</span></span> | <span data-ttu-id="75448-113">Opcional; URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade</span><span class="sxs-lookup"><span data-stu-id="75448-113">Optional; URI that points to an icon which represents the application used to generate the activity</span></span>|
|<span data-ttu-id="75448-114">alternateText</span><span class="sxs-lookup"><span data-stu-id="75448-114">alternateText</span></span> | <span data-ttu-id="75448-115">String</span><span class="sxs-lookup"><span data-stu-id="75448-115">String</span></span> | <span data-ttu-id="75448-116">Opcional; conteúdo de texto ALT acessível para a imagem</span><span class="sxs-lookup"><span data-stu-id="75448-116">Optional; alt-text accessible content for the image</span></span>|
|<span data-ttu-id="75448-117">addImageQuery</span><span class="sxs-lookup"><span data-stu-id="75448-117">addImageQuery</span></span> | <span data-ttu-id="75448-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="75448-118">Boolean</span></span> | <span data-ttu-id="75448-119">Opcional; parâmetro usado para indicar o servidor é capaz de processar imagem dinamicamente em resposta às parametrização.</span><span class="sxs-lookup"><span data-stu-id="75448-119">Optional; parameter used to indicate the server is able to render image dynamically in response to parameterization.</span></span> <span data-ttu-id="75448-120">Por exemplo, – uma imagem de alto contraste</span><span class="sxs-lookup"><span data-stu-id="75448-120">For example – a high contrast image</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75448-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75448-121">JSON Representation</span></span>

<span data-ttu-id="75448-122">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="75448-122">Here is a JSON representation of the resource</span></span>

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