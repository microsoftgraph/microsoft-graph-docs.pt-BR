---
title: Tipo de recurso resource
description: 'Uma imagem ou outro recurso de arquivo em uma página do OneNote. '
localization_priority: Normal
ms.openlocfilehash: c85897af91290df83f4d6fccaf0552513b4f0535
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510278"
---
# <a name="resource-resource-type"></a><span data-ttu-id="b2331-103">Tipo de recurso resource</span><span class="sxs-lookup"><span data-stu-id="b2331-103">resource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2331-104">Uma imagem ou outro recurso de arquivo em uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="b2331-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="b2331-105">É possível obter os dados binários de um recurso, mas não há suporte para obter uma representação JSON de um objeto de recurso ou uma coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="b2331-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="b2331-106">Obtenha os dados binários de um recurso específico enviando uma solicitação GET para o ponto de extremidade `content` do recurso:</span><span class="sxs-lookup"><span data-stu-id="b2331-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="b2331-107">O URI de recurso do arquivo é retornado quando você recebe um conteúdo HTML da página usando a seguinte solicitação:</span><span class="sxs-lookup"><span data-stu-id="b2331-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="b2331-108">Na página HTML, uma marca `img` inclui os pontos de extremidade do recurso de imagem original no atributo `data-fullres-src` e a imagem otimizada no atributo `src`:</span><span class="sxs-lookup"><span data-stu-id="b2331-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="b2331-109">Uma marca `object` (que representa arquivos como PDF, DOCX e PNG) inclui o ponto de extremidade para o recurso do arquivo no atributo `data`:</span><span class="sxs-lookup"><span data-stu-id="b2331-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="b2331-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2331-110">Properties</span></span>
<span data-ttu-id="b2331-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b2331-111">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="b2331-112">Relações</span><span class="sxs-lookup"><span data-stu-id="b2331-112">Relationships</span></span>
<span data-ttu-id="b2331-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2331-113">None.</span></span>


## <a name="methods"></a><span data-ttu-id="b2331-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="b2331-114">Methods</span></span>
| <span data-ttu-id="b2331-115">Método</span><span class="sxs-lookup"><span data-stu-id="b2331-115">Method</span></span>           | <span data-ttu-id="b2331-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b2331-116">Return Type</span></span>    |<span data-ttu-id="b2331-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2331-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b2331-118">Get resource binary data</span><span class="sxs-lookup"><span data-stu-id="b2331-118">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="b2331-119">Fluxo</span><span class="sxs-lookup"><span data-stu-id="b2331-119">Stream</span></span> |<span data-ttu-id="b2331-120">Recupere os dados binários de um recurso de arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="b2331-120">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
