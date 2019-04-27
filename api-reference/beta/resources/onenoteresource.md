---
title: tipo de recurso onenoteResource
description: 'Uma imagem ou outro recurso de arquivo em uma página do OneNote. '
localization_priority: Normal
ms.openlocfilehash: abb60a52b0f32ac2e1bdc024d07f02233db6043c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348474"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="7c347-103">tipo de recurso onenoteResource</span><span class="sxs-lookup"><span data-stu-id="7c347-103">onenoteResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c347-104">Uma imagem ou outro recurso de arquivo em uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="7c347-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="7c347-105">Você pode obter os dados binários de um recurso, mas obter uma representação JSON de um objeto Resource ou uma coleção de recursos não é suportada.</span><span class="sxs-lookup"><span data-stu-id="7c347-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

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
<span data-ttu-id="7c347-106">Obtenha os dados binários de um recurso específico enviando uma solicitação GET para o ponto de `content` extremidade do recurso:</span><span class="sxs-lookup"><span data-stu-id="7c347-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="7c347-107">O URI de recurso do arquivo é retornado quando você obtém o conteúdo HTML de uma página usando a seguinte solicitação:</span><span class="sxs-lookup"><span data-stu-id="7c347-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="7c347-108">Na página HTML, uma `img` marca inclui pontos de extremidade do recurso de imagem original no `data-fullres-src` atributo e a imagem otimizada no `src` atributo:</span><span class="sxs-lookup"><span data-stu-id="7c347-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="7c347-109">Uma `object` marca (que representa arquivos como PDF, docx e png) inclui o ponto de extremidade para o recurso de arquivo no `data` atributo:</span><span class="sxs-lookup"><span data-stu-id="7c347-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="7c347-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c347-110">Properties</span></span>
| <span data-ttu-id="7c347-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c347-111">Property</span></span>     | <span data-ttu-id="7c347-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c347-112">Type</span></span>   |<span data-ttu-id="7c347-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c347-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7c347-114">content</span><span class="sxs-lookup"><span data-stu-id="7c347-114">content</span></span> | <span data-ttu-id="7c347-115">EDM. Stream</span><span class="sxs-lookup"><span data-stu-id="7c347-115">Edm.Stream</span></span>||
| <span data-ttu-id="7c347-116">contentUrl</span><span class="sxs-lookup"><span data-stu-id="7c347-116">contentUrl</span></span> | <span data-ttu-id="7c347-117">String</span><span class="sxs-lookup"><span data-stu-id="7c347-117">String</span></span> ||

## <a name="relationships"></a><span data-ttu-id="7c347-118">Relações</span><span class="sxs-lookup"><span data-stu-id="7c347-118">Relationships</span></span>
<span data-ttu-id="7c347-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7c347-119">None.</span></span>


## <a name="methods"></a><span data-ttu-id="7c347-120">Métodos</span><span class="sxs-lookup"><span data-stu-id="7c347-120">Methods</span></span>
| <span data-ttu-id="7c347-121">Método</span><span class="sxs-lookup"><span data-stu-id="7c347-121">Method</span></span>           | <span data-ttu-id="7c347-122">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7c347-122">Return Type</span></span>    |<span data-ttu-id="7c347-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c347-123">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7c347-124">Obter dados binários do recurso</span><span class="sxs-lookup"><span data-stu-id="7c347-124">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="7c347-125">Fluxo</span><span class="sxs-lookup"><span data-stu-id="7c347-125">Stream</span></span> |<span data-ttu-id="7c347-126">Recupere os dados binários de um recurso de arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="7c347-126">Retrieve the binary data of a file or image resource.</span></span>|

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
