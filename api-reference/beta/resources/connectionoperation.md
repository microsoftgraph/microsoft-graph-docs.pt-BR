---
title: Tipo de recurso connectionOperation
description: Descreve o status de uma solicitação assíncrona para criar um esquema de conexão da Pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e17b1f55b00fd7b9bdc69eb7a7a34d3453ab332d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158300"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="37446-103">Tipo de recurso connectionOperation</span><span class="sxs-lookup"><span data-stu-id="37446-103">connectionOperation resource type</span></span>

<span data-ttu-id="37446-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37446-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37446-105">Descreve o status de uma solicitação assíncrona para criar um esquema de conexão da Pesquisa [da](schema.md)Microsoft.</span><span class="sxs-lookup"><span data-stu-id="37446-105">Describes status of an asynchronous request to create a Microsoft Search connection [schema](schema.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="37446-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="37446-106">Methods</span></span>

| <span data-ttu-id="37446-107">Método</span><span class="sxs-lookup"><span data-stu-id="37446-107">Method</span></span>       | <span data-ttu-id="37446-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="37446-108">Return Type</span></span> | <span data-ttu-id="37446-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="37446-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="37446-110">Obter connectionOperation</span><span class="sxs-lookup"><span data-stu-id="37446-110">Get connectionOperation</span></span>](../api/connectionoperation-get.md) | [<span data-ttu-id="37446-111">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="37446-111">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="37446-112">Leia as propriedades de um objeto connectionOperation.</span><span class="sxs-lookup"><span data-stu-id="37446-112">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="37446-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37446-113">Properties</span></span>

| <span data-ttu-id="37446-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37446-114">Property</span></span> | <span data-ttu-id="37446-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="37446-115">Type</span></span>                          | <span data-ttu-id="37446-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="37446-116">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="37446-117">erro</span><span class="sxs-lookup"><span data-stu-id="37446-117">error</span></span>    | [<span data-ttu-id="37446-118">errorDetail</span><span class="sxs-lookup"><span data-stu-id="37446-118">errorDetail</span></span>](errordetail.md) | <span data-ttu-id="37446-119">Se `status` `failed` for, fornece mais informações sobre o erro que causou a falha.</span><span class="sxs-lookup"><span data-stu-id="37446-119">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="37446-120">id</span><span class="sxs-lookup"><span data-stu-id="37446-120">id</span></span>       | <span data-ttu-id="37446-121">String</span><span class="sxs-lookup"><span data-stu-id="37446-121">String</span></span>                        | <span data-ttu-id="37446-122">Identificador exclusivo da connectionOperation.</span><span class="sxs-lookup"><span data-stu-id="37446-122">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="37446-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37446-123">Read-only.</span></span> |
| <span data-ttu-id="37446-124">status</span><span class="sxs-lookup"><span data-stu-id="37446-124">status</span></span>   | <span data-ttu-id="37446-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37446-125">string</span></span>                        | <span data-ttu-id="37446-126">Indica o status da operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="37446-126">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="37446-127">Os valores possíveis são: `unspecified`, `inprogress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="37446-127">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="37446-128">Relações</span><span class="sxs-lookup"><span data-stu-id="37446-128">Relationships</span></span>

<span data-ttu-id="37446-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37446-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37446-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37446-130">JSON representation</span></span>

<span data-ttu-id="37446-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37446-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectionOperation",
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


