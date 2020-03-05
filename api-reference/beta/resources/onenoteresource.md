---
title: tipo de recurso onenoteResource
description: 'Uma imagem ou outro recurso de arquivo em uma página do OneNote. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0f87d5f9606f0d178d4a92ad6b4d3038799f5c5f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522320"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="62873-103">tipo de recurso onenoteResource</span><span class="sxs-lookup"><span data-stu-id="62873-103">onenoteResource resource type</span></span>

<span data-ttu-id="62873-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="62873-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62873-105">Uma imagem ou outro recurso de arquivo em uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="62873-105">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="62873-106">Você pode obter os dados binários de um recurso, mas obter uma representação JSON de um objeto Resource ou uma coleção de recursos não é suportada.</span><span class="sxs-lookup"><span data-stu-id="62873-106">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": "String (Stream)",
  "contentUrl": "String"
}

```
<span data-ttu-id="62873-107">Obtenha os dados binários de um recurso específico enviando uma solicitação GET para o ponto de `content` extremidade do recurso:</span><span class="sxs-lookup"><span data-stu-id="62873-107">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="62873-108">O URI de recurso do arquivo é retornado quando você obtém o conteúdo HTML de uma página usando a seguinte solicitação:</span><span class="sxs-lookup"><span data-stu-id="62873-108">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="62873-109">Na página HTML, uma `img` marca inclui pontos de extremidade do recurso de imagem original no `data-fullres-src` atributo e a imagem otimizada no `src` atributo:</span><span class="sxs-lookup"><span data-stu-id="62873-109">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="62873-110">Uma `object` marca (que representa arquivos como PDF, docx e png) inclui o ponto de extremidade para o recurso de arquivo no `data` atributo:</span><span class="sxs-lookup"><span data-stu-id="62873-110">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="62873-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62873-111">Properties</span></span>
| <span data-ttu-id="62873-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62873-112">Property</span></span>     | <span data-ttu-id="62873-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="62873-113">Type</span></span>   |<span data-ttu-id="62873-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="62873-114">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="62873-115">content</span><span class="sxs-lookup"><span data-stu-id="62873-115">content</span></span> | <span data-ttu-id="62873-116">EDM. Stream</span><span class="sxs-lookup"><span data-stu-id="62873-116">Edm.Stream</span></span>||
| <span data-ttu-id="62873-117">contentUrl</span><span class="sxs-lookup"><span data-stu-id="62873-117">contentUrl</span></span> | <span data-ttu-id="62873-118">String</span><span class="sxs-lookup"><span data-stu-id="62873-118">String</span></span> ||

## <a name="relationships"></a><span data-ttu-id="62873-119">Relações</span><span class="sxs-lookup"><span data-stu-id="62873-119">Relationships</span></span>
<span data-ttu-id="62873-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="62873-120">None.</span></span>


## <a name="methods"></a><span data-ttu-id="62873-121">Métodos</span><span class="sxs-lookup"><span data-stu-id="62873-121">Methods</span></span>
| <span data-ttu-id="62873-122">Método</span><span class="sxs-lookup"><span data-stu-id="62873-122">Method</span></span>           | <span data-ttu-id="62873-123">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="62873-123">Return Type</span></span>    |<span data-ttu-id="62873-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="62873-124">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="62873-125">Obter dados binários do recurso</span><span class="sxs-lookup"><span data-stu-id="62873-125">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="62873-126">Stream</span><span class="sxs-lookup"><span data-stu-id="62873-126">Stream</span></span> |<span data-ttu-id="62873-127">Recupere os dados binários de um recurso de arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="62873-127">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
