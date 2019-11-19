---
title: tipo de recurso connectionOperation
description: Descreve o status de uma solicitação assíncrona para criar um esquema de conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9ced1c9bd00e3e865c3663ed6ade936747b9dded
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704140"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="e2afc-103">tipo de recurso connectionOperation</span><span class="sxs-lookup"><span data-stu-id="e2afc-103">connectionOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2afc-104">Descreve o status de uma solicitação assíncrona para criar um [esquema](schema.md)de conexão de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e2afc-104">Describes status of an asynchronous request to create a Microsoft Search connection [schema](schema.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="e2afc-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e2afc-105">Methods</span></span>

| <span data-ttu-id="e2afc-106">Método</span><span class="sxs-lookup"><span data-stu-id="e2afc-106">Method</span></span>       | <span data-ttu-id="e2afc-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e2afc-107">Return Type</span></span> | <span data-ttu-id="e2afc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2afc-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e2afc-109">Obter connectionOperation</span><span class="sxs-lookup"><span data-stu-id="e2afc-109">Get connectionOperation</span></span>](../api/connectionoperation-get.md) | [<span data-ttu-id="e2afc-110">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="e2afc-110">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="e2afc-111">Ler as propriedades de um objeto connectionOperation.</span><span class="sxs-lookup"><span data-stu-id="e2afc-111">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e2afc-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2afc-112">Properties</span></span>

| <span data-ttu-id="e2afc-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2afc-113">Property</span></span> | <span data-ttu-id="e2afc-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2afc-114">Type</span></span>                          | <span data-ttu-id="e2afc-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2afc-115">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="e2afc-116">erro</span><span class="sxs-lookup"><span data-stu-id="e2afc-116">error</span></span>    | [<span data-ttu-id="e2afc-117">errorDetail</span><span class="sxs-lookup"><span data-stu-id="e2afc-117">errorDetail</span></span>](errordetail.md) | <span data-ttu-id="e2afc-118">Se `status` for `failed`, fornecerá mais informações sobre o erro que causou a falha.</span><span class="sxs-lookup"><span data-stu-id="e2afc-118">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="e2afc-119">id</span><span class="sxs-lookup"><span data-stu-id="e2afc-119">id</span></span>       | <span data-ttu-id="e2afc-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2afc-120">String</span></span>                        | <span data-ttu-id="e2afc-121">Identificador exclusivo para o connectionOperation.</span><span class="sxs-lookup"><span data-stu-id="e2afc-121">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="e2afc-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e2afc-122">Read-only.</span></span> |
| <span data-ttu-id="e2afc-123">status</span><span class="sxs-lookup"><span data-stu-id="e2afc-123">status</span></span>   | <span data-ttu-id="e2afc-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2afc-124">string</span></span>                        | <span data-ttu-id="e2afc-125">Indica o status da operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="e2afc-125">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="e2afc-126">Os valores possíveis são: `unspecified`, `inprogress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="e2afc-126">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e2afc-127">Relações</span><span class="sxs-lookup"><span data-stu-id="e2afc-127">Relationships</span></span>

<span data-ttu-id="e2afc-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e2afc-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2afc-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2afc-129">JSON representation</span></span>

<span data-ttu-id="e2afc-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2afc-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectionOperation",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.errorDetail"},
  "id": "String (identifier)",
  "status": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectionOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
