---
author: kevinlam
description: O recurso ItemPreviewInfo contém informações sobre como inserir uma visualização de um DriveItem.
ms.date: 3/16/2018
title: ItemPreviewInfo-API do OneDrive
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 2d789dacb0f1c1d3daca988f334fca2e8da4b0d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010053"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="e52ba-103">Tipo de recurso ItemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="e52ba-103">ItemPreviewInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e52ba-104">O recurso **ItemPreviewInfo** contém informações sobre como inserir uma visualização de um [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e52ba-104">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e52ba-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e52ba-105">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="e52ba-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e52ba-106">Properties</span></span>

| <span data-ttu-id="e52ba-107">Nome</span><span class="sxs-lookup"><span data-stu-id="e52ba-107">Name</span></span>           | <span data-ttu-id="e52ba-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e52ba-108">Type</span></span>   | <span data-ttu-id="e52ba-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e52ba-109">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="e52ba-110">getUrl</span><span class="sxs-lookup"><span data-stu-id="e52ba-110">getUrl</span></span>         | <span data-ttu-id="e52ba-111">string</span><span class="sxs-lookup"><span data-stu-id="e52ba-111">string</span></span> | <span data-ttu-id="e52ba-112">URL adequada para incorporação usando HTTP GET (IFrames, etc.)</span><span class="sxs-lookup"><span data-stu-id="e52ba-112">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="e52ba-113">postUrl</span><span class="sxs-lookup"><span data-stu-id="e52ba-113">postUrl</span></span>        | <span data-ttu-id="e52ba-114">string</span><span class="sxs-lookup"><span data-stu-id="e52ba-114">string</span></span> | <span data-ttu-id="e52ba-115">URL adequada para incorporação usando HTTP POST (Form Post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="e52ba-115">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="e52ba-116">postparameters</span><span class="sxs-lookup"><span data-stu-id="e52ba-116">postParameters</span></span> | <span data-ttu-id="e52ba-117">string</span><span class="sxs-lookup"><span data-stu-id="e52ba-117">string</span></span> | <span data-ttu-id="e52ba-118">LANÇAR parâmetros para incluir se estiver usando postUrl</span><span class="sxs-lookup"><span data-stu-id="e52ba-118">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="e52ba-119">Segeturl, postUrl ou ambos podem ser retornados, dependendo do estado atual de suporte para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="e52ba-119">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="e52ba-120">postparameters é uma cadeia de caracteres `application/x-www-form-urlencoded`formatada como e, se estiver executando uma postagem no postUrl, o tipo de conteúdo deve ser definido de acordo.</span><span class="sxs-lookup"><span data-stu-id="e52ba-120">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="e52ba-121">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="e52ba-121">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="e52ba-122">Os formatos das URLs e dos parâmetros devem ser considerados opacos.</span><span class="sxs-lookup"><span data-stu-id="e52ba-122">The formats of URLs and parameters should be considered opaque.</span></span>
