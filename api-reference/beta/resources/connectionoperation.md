---
title: tipo de recurso connectionOperation
description: Descreve o status de uma solicitação assíncrona para criar um esquema de conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 657d71dc6b1671b2af6011778c0b14bb299e3cf9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938881"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="24406-103">tipo de recurso connectionOperation</span><span class="sxs-lookup"><span data-stu-id="24406-103">connectionOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24406-104">Descreve o status de uma solicitação assíncrona para criar um [esquema](schema.md)de conexão de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="24406-104">Describes status of an asynchronous request to create a Microsoft Search connection [schema](schema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="24406-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="24406-105">Methods</span></span>

| <span data-ttu-id="24406-106">Método</span><span class="sxs-lookup"><span data-stu-id="24406-106">Method</span></span>       | <span data-ttu-id="24406-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="24406-107">Return Type</span></span> | <span data-ttu-id="24406-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="24406-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="24406-109">Obter connectionOperation</span><span class="sxs-lookup"><span data-stu-id="24406-109">Get connectionOperation</span></span>](../api/connectionoperation-get.md) | [<span data-ttu-id="24406-110">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="24406-110">connectionOperation</span></span>](connectionoperation.md) | <span data-ttu-id="24406-111">Ler as propriedades de um objeto connectionOperation.</span><span class="sxs-lookup"><span data-stu-id="24406-111">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="24406-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24406-112">Properties</span></span>

| <span data-ttu-id="24406-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24406-113">Property</span></span> | <span data-ttu-id="24406-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="24406-114">Type</span></span>                          | <span data-ttu-id="24406-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="24406-115">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="24406-116">erro</span><span class="sxs-lookup"><span data-stu-id="24406-116">error</span></span>    | [<span data-ttu-id="24406-117">errorDetail</span><span class="sxs-lookup"><span data-stu-id="24406-117">errorDetail</span></span>](errordetail.md) | <span data-ttu-id="24406-118">Se `status` for `failed`, fornecerá mais informações sobre o erro que causou a falha.</span><span class="sxs-lookup"><span data-stu-id="24406-118">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="24406-119">id</span><span class="sxs-lookup"><span data-stu-id="24406-119">id</span></span>       | <span data-ttu-id="24406-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24406-120">String</span></span>                        | <span data-ttu-id="24406-121">Identificador exclusivo para o connectionOperation.</span><span class="sxs-lookup"><span data-stu-id="24406-121">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="24406-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="24406-122">Read-only.</span></span> |
| <span data-ttu-id="24406-123">status</span><span class="sxs-lookup"><span data-stu-id="24406-123">status</span></span>   | <span data-ttu-id="24406-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24406-124">string</span></span>                        | <span data-ttu-id="24406-125">Indica o status da operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="24406-125">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="24406-126">Os valores possíveis são: `unspecified`, `inprogress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="24406-126">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="24406-127">Relações</span><span class="sxs-lookup"><span data-stu-id="24406-127">Relationships</span></span>

<span data-ttu-id="24406-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="24406-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24406-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24406-129">JSON representation</span></span>

<span data-ttu-id="24406-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="24406-130">The following is a JSON representation of the resource.</span></span>

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
