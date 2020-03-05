---
title: tipo de recurso connectionOperation
description: Descreve o status de uma solicitação assíncrona para criar um esquema de conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 21d962bbbfee64c51f11cf1ac3f5e7de2c0497e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507482"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="338bf-103">tipo de recurso connectionOperation</span><span class="sxs-lookup"><span data-stu-id="338bf-103">connectionOperation resource type</span></span>

<span data-ttu-id="338bf-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="338bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="338bf-105">Descreve o status de uma solicitação assíncrona para criar um [esquema](schema.md)de conexão de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="338bf-105">Describes status of an asynchronous request to create a Microsoft Search connection [schema](schema.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="338bf-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="338bf-106">Methods</span></span>

| <span data-ttu-id="338bf-107">Método</span><span class="sxs-lookup"><span data-stu-id="338bf-107">Method</span></span>       | <span data-ttu-id="338bf-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="338bf-108">Return Type</span></span> | <span data-ttu-id="338bf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="338bf-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="338bf-110">Obter connectionOperation</span><span class="sxs-lookup"><span data-stu-id="338bf-110">Get connectionOperation</span></span>](../api/connectionoperation-get.md) | [<span data-ttu-id="338bf-111">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="338bf-111">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="338bf-112">Ler as propriedades de um objeto connectionOperation.</span><span class="sxs-lookup"><span data-stu-id="338bf-112">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="338bf-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="338bf-113">Properties</span></span>

| <span data-ttu-id="338bf-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="338bf-114">Property</span></span> | <span data-ttu-id="338bf-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="338bf-115">Type</span></span>                          | <span data-ttu-id="338bf-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="338bf-116">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="338bf-117">erro</span><span class="sxs-lookup"><span data-stu-id="338bf-117">error</span></span>    | [<span data-ttu-id="338bf-118">errorDetail</span><span class="sxs-lookup"><span data-stu-id="338bf-118">errorDetail</span></span>](errordetail.md) | <span data-ttu-id="338bf-119">Se `status` for `failed`, fornecerá mais informações sobre o erro que causou a falha.</span><span class="sxs-lookup"><span data-stu-id="338bf-119">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="338bf-120">id</span><span class="sxs-lookup"><span data-stu-id="338bf-120">id</span></span>       | <span data-ttu-id="338bf-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="338bf-121">String</span></span>                        | <span data-ttu-id="338bf-122">Identificador exclusivo para o connectionOperation.</span><span class="sxs-lookup"><span data-stu-id="338bf-122">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="338bf-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="338bf-123">Read-only.</span></span> |
| <span data-ttu-id="338bf-124">status</span><span class="sxs-lookup"><span data-stu-id="338bf-124">status</span></span>   | <span data-ttu-id="338bf-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="338bf-125">string</span></span>                        | <span data-ttu-id="338bf-126">Indica o status da operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="338bf-126">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="338bf-127">Os valores possíveis são: `unspecified`, `inprogress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="338bf-127">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="338bf-128">Relações</span><span class="sxs-lookup"><span data-stu-id="338bf-128">Relationships</span></span>

<span data-ttu-id="338bf-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="338bf-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="338bf-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="338bf-130">JSON representation</span></span>

<span data-ttu-id="338bf-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="338bf-131">The following is a JSON representation of the resource.</span></span>

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
