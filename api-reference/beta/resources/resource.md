---
title: Tipo de recurso resource
description: 'Uma imagem ou outro recurso de arquivo em uma página do OneNote. '
ms.openlocfilehash: 8e0e049cab613c7c1a72c8c96e21bac77c507ae1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038888"
---
# <a name="resource-resource-type"></a><span data-ttu-id="34199-103">Tipo de recurso resource</span><span class="sxs-lookup"><span data-stu-id="34199-103">resource resource type</span></span>

> <span data-ttu-id="34199-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="34199-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34199-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="34199-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34199-106">Uma imagem ou outro recurso de arquivo em uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="34199-106">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="34199-107">É possível obter os dados binários de um recurso, mas não há suporte para obter uma representação JSON de um objeto de recurso ou uma coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="34199-107">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="34199-108">Obtenha os dados binários de um recurso específico enviando uma solicitação GET para o ponto de extremidade `content` do recurso:</span><span class="sxs-lookup"><span data-stu-id="34199-108">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="34199-109">O URI de recurso do arquivo é retornado quando você recebe um conteúdo HTML da página usando a seguinte solicitação:</span><span class="sxs-lookup"><span data-stu-id="34199-109">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="34199-110">Na página HTML, uma marca `img` inclui os pontos de extremidade do recurso de imagem original no atributo `data-fullres-src` e a imagem otimizada no atributo `src`:</span><span class="sxs-lookup"><span data-stu-id="34199-110">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="34199-111">Uma marca `object` (que representa arquivos como PDF, DOCX e PNG) inclui o ponto de extremidade para o recurso do arquivo no atributo `data`:</span><span class="sxs-lookup"><span data-stu-id="34199-111">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="34199-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34199-112">Properties</span></span>
<span data-ttu-id="34199-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="34199-113">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="34199-114">Relações</span><span class="sxs-lookup"><span data-stu-id="34199-114">Relationships</span></span>
<span data-ttu-id="34199-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34199-115">None.</span></span>


## <a name="methods"></a><span data-ttu-id="34199-116">Métodos</span><span class="sxs-lookup"><span data-stu-id="34199-116">Methods</span></span>
| <span data-ttu-id="34199-117">Método</span><span class="sxs-lookup"><span data-stu-id="34199-117">Method</span></span>           | <span data-ttu-id="34199-118">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="34199-118">Return Type</span></span>    |<span data-ttu-id="34199-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="34199-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="34199-120">Get resource binary data</span><span class="sxs-lookup"><span data-stu-id="34199-120">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="34199-121">Fluxo</span><span class="sxs-lookup"><span data-stu-id="34199-121">Stream</span></span> |<span data-ttu-id="34199-122">Recupere os dados binários de um recurso de arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="34199-122">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->