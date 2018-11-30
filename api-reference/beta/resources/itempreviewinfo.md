---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo - OneDrive API
ms.openlocfilehash: 3fa9d10ae3aade7be96e81168b34df84698da1c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034800"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="9e815-102">Tipo de recurso de ItemPreviewInfo</span><span class="sxs-lookup"><span data-stu-id="9e815-102">ItemPreviewInfo resource type</span></span>

> <span data-ttu-id="9e815-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9e815-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e815-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9e815-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e815-105">O recurso de **ItemPreviewInfo** contém informações sobre como inserir uma visualização de um [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="9e815-105">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e815-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e815-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="9e815-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e815-107">Properties</span></span>

| <span data-ttu-id="9e815-108">Nome</span><span class="sxs-lookup"><span data-stu-id="9e815-108">Name</span></span>           | <span data-ttu-id="9e815-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e815-109">Type</span></span>   | <span data-ttu-id="9e815-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e815-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="9e815-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="9e815-111">getUrl</span></span>         | <span data-ttu-id="9e815-112">string</span><span class="sxs-lookup"><span data-stu-id="9e815-112">string</span></span> | <span data-ttu-id="9e815-113">URL adequada para incorporação usando HTTP GET (iframes, etc.)</span><span class="sxs-lookup"><span data-stu-id="9e815-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="9e815-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="9e815-114">postUrl</span></span>        | <span data-ttu-id="9e815-115">string</span><span class="sxs-lookup"><span data-stu-id="9e815-115">string</span></span> | <span data-ttu-id="9e815-116">URL adequada para incorporação usando POST HTTP (formulário post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="9e815-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="9e815-117">postParameters</span><span class="sxs-lookup"><span data-stu-id="9e815-117">postParameters</span></span> | <span data-ttu-id="9e815-118">string</span><span class="sxs-lookup"><span data-stu-id="9e815-118">string</span></span> | <span data-ttu-id="9e815-119">Parâmetros de POSTAGEM para incluir se usando postUrl</span><span class="sxs-lookup"><span data-stu-id="9e815-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="9e815-120">GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual do suporte para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="9e815-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="9e815-121">postParameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded`, e se realizar uma POSTAGEM para o postUrl o tipo de conteúdo deve ser definida adequadamente.</span><span class="sxs-lookup"><span data-stu-id="9e815-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="9e815-122">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="9e815-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="9e815-123">Os formatos das URLs e dos parâmetros devem ser considerados opacos.</span><span class="sxs-lookup"><span data-stu-id="9e815-123">The formats of URLs and parameters should be considered opaque.</span></span>