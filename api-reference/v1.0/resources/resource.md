---
title: Tipo de recurso OneNoteResource
description: 'Uma imagem ou outro recurso de arquivo em uma página do OneNote. '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cd8ea18047aa3f24343411f8dafd7a79357da87b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034689"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="f912f-103">Tipo de recurso OneNoteResource</span><span class="sxs-lookup"><span data-stu-id="f912f-103">OneNoteResource resource type</span></span>

<span data-ttu-id="f912f-104">Uma imagem ou outro recurso de arquivo em uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f912f-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="f912f-105">Você pode obter os dados binários de um recurso, mas obter uma representação JSON de um objeto Resource ou uma coleção de recursos não é suportada.</span><span class="sxs-lookup"><span data-stu-id="f912f-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

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

<span data-ttu-id="f912f-106">Obtenha os dados binários de um recurso específico enviando uma solicitação GET para o ponto de `content` extremidade do recurso:</span><span class="sxs-lookup"><span data-stu-id="f912f-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="f912f-107">O URI de recurso do arquivo é retornado quando você obtém o conteúdo HTML de uma página usando a seguinte solicitação:</span><span class="sxs-lookup"><span data-stu-id="f912f-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="f912f-108">Na página HTML, uma `img` marca inclui pontos de extremidade do recurso de imagem original no `data-fullres-src` atributo e a imagem otimizada no `src` atributo:</span><span class="sxs-lookup"><span data-stu-id="f912f-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="f912f-109">Uma `object` marca (que representa arquivos como PDF, docx e png) inclui o ponto de extremidade para o recurso de arquivo no `data` atributo:</span><span class="sxs-lookup"><span data-stu-id="f912f-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="f912f-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f912f-110">Properties</span></span>

| <span data-ttu-id="f912f-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f912f-111">Property</span></span>             | <span data-ttu-id="f912f-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="f912f-112">Type</span></span>            | <span data-ttu-id="f912f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f912f-113">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="f912f-114">conteúdo</span><span class="sxs-lookup"><span data-stu-id="f912f-114">content</span></span>              | <span data-ttu-id="f912f-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="f912f-115">Stream</span></span>          | <span data-ttu-id="f912f-116">O fluxo de conteúdo</span><span class="sxs-lookup"><span data-stu-id="f912f-116">The content stream</span></span>
| <span data-ttu-id="f912f-117">contentUrl</span><span class="sxs-lookup"><span data-stu-id="f912f-117">contentUrl</span></span>           | <span data-ttu-id="f912f-118">Cadeia de caracteres (URL)</span><span class="sxs-lookup"><span data-stu-id="f912f-118">String (url)</span></span>    | <span data-ttu-id="f912f-119">A URL para baixar o conteúdo</span><span class="sxs-lookup"><span data-stu-id="f912f-119">The URL for downloading the content</span></span>

## <a name="relationships"></a><span data-ttu-id="f912f-120">Relações</span><span class="sxs-lookup"><span data-stu-id="f912f-120">Relationships</span></span>
<span data-ttu-id="f912f-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f912f-121">None.</span></span>


## <a name="methods"></a><span data-ttu-id="f912f-122">Métodos</span><span class="sxs-lookup"><span data-stu-id="f912f-122">Methods</span></span>
| <span data-ttu-id="f912f-123">Método</span><span class="sxs-lookup"><span data-stu-id="f912f-123">Method</span></span>           | <span data-ttu-id="f912f-124">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f912f-124">Return Type</span></span>    |<span data-ttu-id="f912f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f912f-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f912f-126">Obter dados binários do recurso</span><span class="sxs-lookup"><span data-stu-id="f912f-126">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="f912f-127">Fluxo</span><span class="sxs-lookup"><span data-stu-id="f912f-127">Stream</span></span> |<span data-ttu-id="f912f-128">Recupere os dados binários de um recurso de arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="f912f-128">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
