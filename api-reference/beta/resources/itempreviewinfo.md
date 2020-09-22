---
author: kevinlam
description: O recurso ItemPreviewInfo contém informações sobre como inserir uma visualização de um DriveItem.
ms.date: 3/16/2018
title: ItemPreviewInfo-API do OneDrive
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ab62e2a41d257adcb8f763b77e42f0d7e515ee5b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033690"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="8b588-103">Tipo de recurso ItemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="8b588-103">ItemPreviewInfo resource type</span></span>

<span data-ttu-id="8b588-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b588-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b588-105">O recurso **ItemPreviewInfo** contém informações sobre como inserir uma visualização de um [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="8b588-105">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b588-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b588-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="8b588-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b588-107">Properties</span></span>

| <span data-ttu-id="8b588-108">Nome</span><span class="sxs-lookup"><span data-stu-id="8b588-108">Name</span></span>           | <span data-ttu-id="8b588-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b588-109">Type</span></span>   | <span data-ttu-id="8b588-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b588-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="8b588-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="8b588-111">getUrl</span></span>         | <span data-ttu-id="8b588-112">string</span><span class="sxs-lookup"><span data-stu-id="8b588-112">string</span></span> | <span data-ttu-id="8b588-113">URL adequada para incorporação usando HTTP GET (IFrames, etc.)</span><span class="sxs-lookup"><span data-stu-id="8b588-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="8b588-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="8b588-114">postUrl</span></span>        | <span data-ttu-id="8b588-115">string</span><span class="sxs-lookup"><span data-stu-id="8b588-115">string</span></span> | <span data-ttu-id="8b588-116">URL adequada para incorporação usando HTTP POST (Form Post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="8b588-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="8b588-117">postparameters</span><span class="sxs-lookup"><span data-stu-id="8b588-117">postParameters</span></span> | <span data-ttu-id="8b588-118">string</span><span class="sxs-lookup"><span data-stu-id="8b588-118">string</span></span> | <span data-ttu-id="8b588-119">LANÇAR parâmetros para incluir se estiver usando postUrl</span><span class="sxs-lookup"><span data-stu-id="8b588-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="8b588-120">Segeturl, postUrl ou ambos podem ser retornados, dependendo do estado atual de suporte para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="8b588-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="8b588-121">postparameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded` e, se estiver executando uma postagem no postUrl, o tipo de conteúdo deve ser definido de acordo.</span><span class="sxs-lookup"><span data-stu-id="8b588-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="8b588-122">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="8b588-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="8b588-123">Os formatos das URLs e dos parâmetros devem ser considerados opacos.</span><span class="sxs-lookup"><span data-stu-id="8b588-123">The formats of URLs and parameters should be considered opaque.</span></span>


