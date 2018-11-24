---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
ms.openlocfilehash: 8b8f7a962e237cc20a42503efd31f083996ad715
ms.sourcegitcommit: ebac77d2ca32438e552831de0258fe5e86fa225a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2018
ms.locfileid: "26605864"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="fffba-102">tipo de recurso de itemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="fffba-102">itemPreviewInfo resource type</span></span>

<span data-ttu-id="fffba-103">O recurso de **itemPreviewInfo** contém informações sobre como inserir uma visualização de um [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="fffba-103">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="fffba-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fffba-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="fffba-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fffba-105">Properties</span></span>

| <span data-ttu-id="fffba-106">Nome</span><span class="sxs-lookup"><span data-stu-id="fffba-106">Name</span></span>           | <span data-ttu-id="fffba-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fffba-107">Type</span></span>   | <span data-ttu-id="fffba-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fffba-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="fffba-109">getUrl</span><span class="sxs-lookup"><span data-stu-id="fffba-109">getUrl</span></span>         | <span data-ttu-id="fffba-110">string</span><span class="sxs-lookup"><span data-stu-id="fffba-110">string</span></span> | <span data-ttu-id="fffba-111">URL adequada para incorporação usando HTTP GET (iframes, etc.)</span><span class="sxs-lookup"><span data-stu-id="fffba-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="fffba-112">postUrl</span><span class="sxs-lookup"><span data-stu-id="fffba-112">postUrl</span></span>        | <span data-ttu-id="fffba-113">string</span><span class="sxs-lookup"><span data-stu-id="fffba-113">string</span></span> | <span data-ttu-id="fffba-114">URL adequada para incorporação usando POST HTTP (formulário post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="fffba-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="fffba-115">postParameters</span><span class="sxs-lookup"><span data-stu-id="fffba-115">postParameters</span></span> | <span data-ttu-id="fffba-116">string</span><span class="sxs-lookup"><span data-stu-id="fffba-116">string</span></span> | <span data-ttu-id="fffba-117">Parâmetros de POSTAGEM para incluir se usando postUrl</span><span class="sxs-lookup"><span data-stu-id="fffba-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="fffba-118">GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual do suporte para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="fffba-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="fffba-119">postParameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded`, e se realizar uma POSTAGEM para o postUrl o tipo de conteúdo deve ser definida adequadamente.</span><span class="sxs-lookup"><span data-stu-id="fffba-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="fffba-120">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="fffba-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="fffba-121">Os formatos das URLs e dos parâmetros devem ser considerados opacos.</span><span class="sxs-lookup"><span data-stu-id="fffba-121">The formats of URLs and parameters should be considered opaque.</span></span>
