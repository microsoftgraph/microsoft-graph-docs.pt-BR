---
title: Tipo de recurso de OneNoteResource
description: 'Uma imagem ou outro recurso de arquivo em uma página do OneNote. '
localization_priority: Normal
ms.openlocfilehash: ed2fb0dd4b6e68c24da1f2441a157f734a5025f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855101"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="a97ee-103">Tipo de recurso de OneNoteResource</span><span class="sxs-lookup"><span data-stu-id="a97ee-103">OneNoteResource resource type</span></span>

<span data-ttu-id="a97ee-104">Uma imagem ou outro recurso de arquivo em uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="a97ee-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="a97ee-105">É possível obter os dados binários de um recurso, mas não há suporte para obter uma representação JSON de um objeto de recurso ou uma coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="a97ee-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "contentUrl": "string (url)"
}
```

<span data-ttu-id="a97ee-106">Obtenha os dados binários de um recurso específico enviando uma solicitação GET para o ponto de extremidade `content` do recurso:</span><span class="sxs-lookup"><span data-stu-id="a97ee-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="a97ee-107">O URI de recurso do arquivo é retornado quando você recebe um conteúdo HTML da página usando a seguinte solicitação:</span><span class="sxs-lookup"><span data-stu-id="a97ee-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="a97ee-108">Na página HTML, uma marca `img` inclui os pontos de extremidade do recurso de imagem original no atributo `data-fullres-src` e a imagem otimizada no atributo `src`:</span><span class="sxs-lookup"><span data-stu-id="a97ee-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="a97ee-109">Uma marca `object` (que representa arquivos como PDF, DOCX e PNG) inclui o ponto de extremidade para o recurso do arquivo no atributo `data`:</span><span class="sxs-lookup"><span data-stu-id="a97ee-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="a97ee-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a97ee-110">Properties</span></span>

| <span data-ttu-id="a97ee-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a97ee-111">Property</span></span>             | <span data-ttu-id="a97ee-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="a97ee-112">Type</span></span>            | <span data-ttu-id="a97ee-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="a97ee-113">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="a97ee-114">content</span><span class="sxs-lookup"><span data-stu-id="a97ee-114">content</span></span>              | <span data-ttu-id="a97ee-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="a97ee-115">Stream</span></span>          | <span data-ttu-id="a97ee-116">O fluxo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="a97ee-116">The content stream</span></span>
| <span data-ttu-id="a97ee-117">contentUrl</span><span class="sxs-lookup"><span data-stu-id="a97ee-117">contentUrl</span></span>           | <span data-ttu-id="a97ee-118">Cadeia de caracteres (url)</span><span class="sxs-lookup"><span data-stu-id="a97ee-118">String (url)</span></span>    | <span data-ttu-id="a97ee-119">A URL para baixar o conteúdo</span><span class="sxs-lookup"><span data-stu-id="a97ee-119">The URL for downloading the content</span></span>

## <a name="relationships"></a><span data-ttu-id="a97ee-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a97ee-120">Relationships</span></span>
<span data-ttu-id="a97ee-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a97ee-121">None.</span></span>


## <a name="methods"></a><span data-ttu-id="a97ee-122">Métodos</span><span class="sxs-lookup"><span data-stu-id="a97ee-122">Methods</span></span>
| <span data-ttu-id="a97ee-123">Método</span><span class="sxs-lookup"><span data-stu-id="a97ee-123">Method</span></span>           | <span data-ttu-id="a97ee-124">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a97ee-124">Return Type</span></span>    |<span data-ttu-id="a97ee-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a97ee-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a97ee-126">Get resource binary data</span><span class="sxs-lookup"><span data-stu-id="a97ee-126">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="a97ee-127">Fluxo</span><span class="sxs-lookup"><span data-stu-id="a97ee-127">Stream</span></span> |<span data-ttu-id="a97ee-128">Recupere os dados binários de um recurso de arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="a97ee-128">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
