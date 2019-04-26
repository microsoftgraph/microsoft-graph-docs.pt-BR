---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo-API do OneDrive
localization_priority: Normal
ms.openlocfilehash: c43626292cd07ad14d27202255a499b413dbae63
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345502"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="fd453-102">Tipo de recurso ItemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="fd453-102">ItemPreviewInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd453-103">O recurso **ItemPreviewInfo** contém informações sobre como inserir uma visualização de um [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="fd453-103">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd453-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd453-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="fd453-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd453-105">Properties</span></span>

| <span data-ttu-id="fd453-106">Nome</span><span class="sxs-lookup"><span data-stu-id="fd453-106">Name</span></span>           | <span data-ttu-id="fd453-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd453-107">Type</span></span>   | <span data-ttu-id="fd453-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd453-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="fd453-109">getUrl</span><span class="sxs-lookup"><span data-stu-id="fd453-109">getUrl</span></span>         | <span data-ttu-id="fd453-110">string</span><span class="sxs-lookup"><span data-stu-id="fd453-110">string</span></span> | <span data-ttu-id="fd453-111">URL adequada para incorporação usando HTTP GET (IFrames, etc.)</span><span class="sxs-lookup"><span data-stu-id="fd453-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="fd453-112">postUrl</span><span class="sxs-lookup"><span data-stu-id="fd453-112">postUrl</span></span>        | <span data-ttu-id="fd453-113">string</span><span class="sxs-lookup"><span data-stu-id="fd453-113">string</span></span> | <span data-ttu-id="fd453-114">URL adequada para incorporação usando HTTP POST (Form Post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="fd453-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="fd453-115">postparameters</span><span class="sxs-lookup"><span data-stu-id="fd453-115">postParameters</span></span> | <span data-ttu-id="fd453-116">string</span><span class="sxs-lookup"><span data-stu-id="fd453-116">string</span></span> | <span data-ttu-id="fd453-117">LANÇAR parâmetros para incluir se estiver usando postUrl</span><span class="sxs-lookup"><span data-stu-id="fd453-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="fd453-118">SegetUrl, postUrl ou ambos podem ser retornados, dependendo do estado atual de suporte para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="fd453-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="fd453-119">postparameters é uma cadeia de caracteres `application/x-www-form-urlencoded`formatada como e, se estiver executando uma postaGem no postUrl, o tipo de conteúdo deve ser definido de acordo.</span><span class="sxs-lookup"><span data-stu-id="fd453-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="fd453-120">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="fd453-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="fd453-121">Os formatos das URLs e dos parâmetros devem ser considerados opacos.</span><span class="sxs-lookup"><span data-stu-id="fd453-121">The formats of URLs and parameters should be considered opaque.</span></span>
