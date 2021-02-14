---
author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
description: O recurso itemPreviewInfo contém informações sobre como inserir uma visualização de um driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fc7ece7ed529a714b2e1262c4e39444639caced1
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240567"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="dbacd-103">Tipo de recurso itemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="dbacd-103">itemPreviewInfo resource type</span></span>

<span data-ttu-id="dbacd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbacd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dbacd-105">O **recurso itemPreviewInfo** contém informações sobre como inserir uma visualização de [um driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="dbacd-105">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbacd-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbacd-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="dbacd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbacd-107">Properties</span></span>

| <span data-ttu-id="dbacd-108">Nome</span><span class="sxs-lookup"><span data-stu-id="dbacd-108">Name</span></span>           | <span data-ttu-id="dbacd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbacd-109">Type</span></span>   | <span data-ttu-id="dbacd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbacd-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="dbacd-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="dbacd-111">getUrl</span></span>         | <span data-ttu-id="dbacd-112">string</span><span class="sxs-lookup"><span data-stu-id="dbacd-112">string</span></span> | <span data-ttu-id="dbacd-113">URL adequada para incorporação usando HTTP GET (iframes, etc.)</span><span class="sxs-lookup"><span data-stu-id="dbacd-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="dbacd-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="dbacd-114">postUrl</span></span>        | <span data-ttu-id="dbacd-115">string</span><span class="sxs-lookup"><span data-stu-id="dbacd-115">string</span></span> | <span data-ttu-id="dbacd-116">URL adequada para incorporação usando HTTP POST (postagem de formulário, JS etc.)</span><span class="sxs-lookup"><span data-stu-id="dbacd-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="dbacd-117">postParameters</span><span class="sxs-lookup"><span data-stu-id="dbacd-117">postParameters</span></span> | <span data-ttu-id="dbacd-118">string</span><span class="sxs-lookup"><span data-stu-id="dbacd-118">string</span></span> | <span data-ttu-id="dbacd-119">Parâmetros POST a incluir se estiver usando postUrl</span><span class="sxs-lookup"><span data-stu-id="dbacd-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="dbacd-120">GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual do suporte para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="dbacd-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="dbacd-121">postParameters é uma cadeia de caracteres formatada como , e se executar um POST para postUrl, o tipo de conteúdo deve `application/x-www-form-urlencoded` ser definido de acordo.</span><span class="sxs-lookup"><span data-stu-id="dbacd-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="dbacd-122">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="dbacd-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="dbacd-123">Os formatos de URLs e parâmetros devem ser considerados opacos.</span><span class="sxs-lookup"><span data-stu-id="dbacd-123">The formats of URLs and parameters should be considered opaque.</span></span>

