---
title: Tipo de recurso connectionOperation
description: Descreve o status de uma solicitação assíncrona para criar um Pesquisa da Microsoft de conexão.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1b9e3bf811807213970694ebe4e7748bf59e32ef
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467571"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="cb1ba-103">Tipo de recurso connectionOperation</span><span class="sxs-lookup"><span data-stu-id="cb1ba-103">connectionOperation resource type</span></span>

<span data-ttu-id="cb1ba-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="cb1ba-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb1ba-105">Descreve o status de uma solicitação assíncrona para criar um Pesquisa da Microsoft [de conexão](externalconnectors-schema.md).</span><span class="sxs-lookup"><span data-stu-id="cb1ba-105">Describes status of an asynchronous request to create a Microsoft Search connection [schema](externalconnectors-schema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cb1ba-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="cb1ba-106">Methods</span></span>

| <span data-ttu-id="cb1ba-107">Método</span><span class="sxs-lookup"><span data-stu-id="cb1ba-107">Method</span></span>       | <span data-ttu-id="cb1ba-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cb1ba-108">Return Type</span></span> | <span data-ttu-id="cb1ba-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb1ba-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cb1ba-110">Obter connectionOperation</span><span class="sxs-lookup"><span data-stu-id="cb1ba-110">Get connectionOperation</span></span>](../api/externalconnectors-connectionoperation-get.md) | [<span data-ttu-id="cb1ba-111">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="cb1ba-111">connectionOperation</span></span>](externalconnectors-connectionoperation.md) | <span data-ttu-id="cb1ba-112">Ler propriedades de um objeto connectionOperation.</span><span class="sxs-lookup"><span data-stu-id="cb1ba-112">Read properties of a connectionOperation object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cb1ba-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb1ba-113">Properties</span></span>

| <span data-ttu-id="cb1ba-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb1ba-114">Property</span></span> | <span data-ttu-id="cb1ba-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb1ba-115">Type</span></span>                          | <span data-ttu-id="cb1ba-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb1ba-116">Description</span></span>                       |
|:---------|:------------------------------|:----------------------------------|
| <span data-ttu-id="cb1ba-117">erro</span><span class="sxs-lookup"><span data-stu-id="cb1ba-117">error</span></span>    | [<span data-ttu-id="cb1ba-118">publicError</span><span class="sxs-lookup"><span data-stu-id="cb1ba-118">publicError</span></span>](publicerror.md) | <span data-ttu-id="cb1ba-119">Se `status` for , fornece mais informações sobre o erro que causou a `failed` falha.</span><span class="sxs-lookup"><span data-stu-id="cb1ba-119">If `status` is `failed`, provides more information about the error that caused the failure.</span></span> |
| <span data-ttu-id="cb1ba-120">id</span><span class="sxs-lookup"><span data-stu-id="cb1ba-120">id</span></span>       | <span data-ttu-id="cb1ba-121">String</span><span class="sxs-lookup"><span data-stu-id="cb1ba-121">String</span></span>                        | <span data-ttu-id="cb1ba-122">Identificador exclusivo da connectionOperation.</span><span class="sxs-lookup"><span data-stu-id="cb1ba-122">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="cb1ba-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cb1ba-123">Read-only.</span></span> |
| <span data-ttu-id="cb1ba-124">status</span><span class="sxs-lookup"><span data-stu-id="cb1ba-124">status</span></span>   | <span data-ttu-id="cb1ba-125">String</span><span class="sxs-lookup"><span data-stu-id="cb1ba-125">String</span></span>                        | <span data-ttu-id="cb1ba-126">Indica o status da operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="cb1ba-126">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="cb1ba-127">Os valores possíveis são: `unspecified`, `inprogress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="cb1ba-127">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cb1ba-128">Relações</span><span class="sxs-lookup"><span data-stu-id="cb1ba-128">Relationships</span></span>

<span data-ttu-id="cb1ba-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb1ba-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb1ba-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb1ba-130">JSON representation</span></span>

<span data-ttu-id="cb1ba-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb1ba-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "status": "String"
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
