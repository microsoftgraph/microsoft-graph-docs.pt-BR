---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
description: O recurso itemPreviewInfo contém informações sobre como inserir uma visualização de um driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 71d660a71bce09f198a0feb9c3acbb9a69a23a5f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036558"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="fe976-103">tipo de recurso itemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="fe976-103">itemPreviewInfo resource type</span></span>

<span data-ttu-id="fe976-104">O recurso **itemPreviewInfo** contém informações sobre como inserir uma visualização de um [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="fe976-104">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe976-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe976-105">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="fe976-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe976-106">Properties</span></span>

| <span data-ttu-id="fe976-107">Nome</span><span class="sxs-lookup"><span data-stu-id="fe976-107">Name</span></span>           | <span data-ttu-id="fe976-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe976-108">Type</span></span>   | <span data-ttu-id="fe976-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe976-109">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="fe976-110">getUrl</span><span class="sxs-lookup"><span data-stu-id="fe976-110">getUrl</span></span>         | <span data-ttu-id="fe976-111">string</span><span class="sxs-lookup"><span data-stu-id="fe976-111">string</span></span> | <span data-ttu-id="fe976-112">URL adequada para incorporação usando HTTP GET (IFrames, etc.)</span><span class="sxs-lookup"><span data-stu-id="fe976-112">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="fe976-113">postUrl</span><span class="sxs-lookup"><span data-stu-id="fe976-113">postUrl</span></span>        | <span data-ttu-id="fe976-114">string</span><span class="sxs-lookup"><span data-stu-id="fe976-114">string</span></span> | <span data-ttu-id="fe976-115">URL adequada para incorporação usando HTTP POST (Form Post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="fe976-115">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="fe976-116">postparameters</span><span class="sxs-lookup"><span data-stu-id="fe976-116">postParameters</span></span> | <span data-ttu-id="fe976-117">string</span><span class="sxs-lookup"><span data-stu-id="fe976-117">string</span></span> | <span data-ttu-id="fe976-118">LANÇAR parâmetros para incluir se estiver usando postUrl</span><span class="sxs-lookup"><span data-stu-id="fe976-118">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="fe976-119">Segeturl, postUrl ou ambos podem ser retornados, dependendo do estado atual de suporte para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="fe976-119">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="fe976-120">postparameters é uma cadeia de caracteres `application/x-www-form-urlencoded`formatada como e, se estiver executando uma postagem no postUrl, o tipo de conteúdo deve ser definido de acordo.</span><span class="sxs-lookup"><span data-stu-id="fe976-120">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="fe976-121">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="fe976-121">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="fe976-122">Os formatos das URLs e dos parâmetros devem ser considerados opacos.</span><span class="sxs-lookup"><span data-stu-id="fe976-122">The formats of URLs and parameters should be considered opaque.</span></span>
