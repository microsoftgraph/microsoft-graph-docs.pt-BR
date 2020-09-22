---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
description: O recurso itemPreviewInfo contém informações sobre como inserir uma visualização de um driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4d04384ba8efe27b369bfd4d73a560baf920cd53
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009237"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="d4356-103">tipo de recurso itemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="d4356-103">itemPreviewInfo resource type</span></span>

<span data-ttu-id="d4356-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4356-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4356-105">O recurso **itemPreviewInfo** contém informações sobre como inserir uma visualização de um [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d4356-105">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4356-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4356-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="d4356-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4356-107">Properties</span></span>

| <span data-ttu-id="d4356-108">Nome</span><span class="sxs-lookup"><span data-stu-id="d4356-108">Name</span></span>           | <span data-ttu-id="d4356-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4356-109">Type</span></span>   | <span data-ttu-id="d4356-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4356-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="d4356-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="d4356-111">getUrl</span></span>         | <span data-ttu-id="d4356-112">string</span><span class="sxs-lookup"><span data-stu-id="d4356-112">string</span></span> | <span data-ttu-id="d4356-113">URL adequada para incorporação usando HTTP GET (IFrames, etc.)</span><span class="sxs-lookup"><span data-stu-id="d4356-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="d4356-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="d4356-114">postUrl</span></span>        | <span data-ttu-id="d4356-115">string</span><span class="sxs-lookup"><span data-stu-id="d4356-115">string</span></span> | <span data-ttu-id="d4356-116">URL adequada para incorporação usando HTTP POST (Form Post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="d4356-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="d4356-117">postparameters</span><span class="sxs-lookup"><span data-stu-id="d4356-117">postParameters</span></span> | <span data-ttu-id="d4356-118">string</span><span class="sxs-lookup"><span data-stu-id="d4356-118">string</span></span> | <span data-ttu-id="d4356-119">LANÇAR parâmetros para incluir se estiver usando postUrl</span><span class="sxs-lookup"><span data-stu-id="d4356-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="d4356-120">Segeturl, postUrl ou ambos podem ser retornados, dependendo do estado atual de suporte para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="d4356-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="d4356-121">postparameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded` e, se estiver executando uma postagem no postUrl, o tipo de conteúdo deve ser definido de acordo.</span><span class="sxs-lookup"><span data-stu-id="d4356-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="d4356-122">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="d4356-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="d4356-123">Os formatos das URLs e dos parâmetros devem ser considerados opacos.</span><span class="sxs-lookup"><span data-stu-id="d4356-123">The formats of URLs and parameters should be considered opaque.</span></span>

