---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo - OneDrive API
localization_priority: Normal
ms.openlocfilehash: 469679e9baa016560f5a02425bc41d628a24dc2c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509760"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="387fd-102">Tipo de recurso de ItemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="387fd-102">ItemPreviewInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="387fd-103">O recurso de **ItemPreviewInfo** contém informações sobre como inserir uma visualização de um [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="387fd-103">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="387fd-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="387fd-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="387fd-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="387fd-105">Properties</span></span>

| <span data-ttu-id="387fd-106">Nome</span><span class="sxs-lookup"><span data-stu-id="387fd-106">Name</span></span>           | <span data-ttu-id="387fd-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="387fd-107">Type</span></span>   | <span data-ttu-id="387fd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="387fd-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="387fd-109">getUrl</span><span class="sxs-lookup"><span data-stu-id="387fd-109">getUrl</span></span>         | <span data-ttu-id="387fd-110">string</span><span class="sxs-lookup"><span data-stu-id="387fd-110">string</span></span> | <span data-ttu-id="387fd-111">URL adequada para incorporação usando HTTP GET (iframes, etc.)</span><span class="sxs-lookup"><span data-stu-id="387fd-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="387fd-112">postUrl</span><span class="sxs-lookup"><span data-stu-id="387fd-112">postUrl</span></span>        | <span data-ttu-id="387fd-113">string</span><span class="sxs-lookup"><span data-stu-id="387fd-113">string</span></span> | <span data-ttu-id="387fd-114">URL adequada para incorporação usando POST HTTP (formulário post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="387fd-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="387fd-115">postParameters</span><span class="sxs-lookup"><span data-stu-id="387fd-115">postParameters</span></span> | <span data-ttu-id="387fd-116">string</span><span class="sxs-lookup"><span data-stu-id="387fd-116">string</span></span> | <span data-ttu-id="387fd-117">Parâmetros de POSTAGEM para incluir se usando postUrl</span><span class="sxs-lookup"><span data-stu-id="387fd-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="387fd-118">GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual do suporte para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="387fd-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="387fd-119">postParameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded`, e se realizar uma POSTAGEM para o postUrl o tipo de conteúdo deve ser definida adequadamente.</span><span class="sxs-lookup"><span data-stu-id="387fd-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="387fd-120">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="387fd-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="387fd-121">Os formatos das URLs e dos parâmetros devem ser considerados opacos.</span><span class="sxs-lookup"><span data-stu-id="387fd-121">The formats of URLs and parameters should be considered opaque.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/itempreviewinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
