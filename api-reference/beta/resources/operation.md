---
title: tipo de recurso Operation
description: O status de uma operação de execução longa.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: billbliss
ms.openlocfilehash: e94970609c2ccfb99e61b254b080e1dbaa244ba6
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809310"
---
# <a name="operation-resource-type"></a><span data-ttu-id="f2639-103">tipo de recurso Operation</span><span class="sxs-lookup"><span data-stu-id="f2639-103">operation resource type</span></span>

<span data-ttu-id="f2639-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2639-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2639-105">O status de uma operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="f2639-105">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="f2639-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f2639-106">Methods</span></span>

<span data-ttu-id="f2639-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2639-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="f2639-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2639-108">Properties</span></span>

| <span data-ttu-id="f2639-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2639-109">Property</span></span>           | <span data-ttu-id="f2639-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2639-110">Type</span></span>            | <span data-ttu-id="f2639-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2639-111">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="f2639-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2639-112">createdDateTime</span></span>    | <span data-ttu-id="f2639-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2639-113">DateTimeOffset</span></span>  | <span data-ttu-id="f2639-114">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="f2639-114">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="f2639-115">id</span><span class="sxs-lookup"><span data-stu-id="f2639-115">id</span></span>                 | <span data-ttu-id="f2639-116">String</span><span class="sxs-lookup"><span data-stu-id="f2639-116">String</span></span>          | <span data-ttu-id="f2639-117">A ID da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2639-117">The operation id. Read-only.</span></span> <span data-ttu-id="f2639-118">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="f2639-118">Server generated.</span></span>                                  |
| <span data-ttu-id="f2639-119">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="f2639-119">lastActionDateTime</span></span> | <span data-ttu-id="f2639-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2639-120">DateTimeOffset</span></span>  | <span data-ttu-id="f2639-121">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="f2639-121">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="f2639-122">status</span><span class="sxs-lookup"><span data-stu-id="f2639-122">status</span></span>             | <span data-ttu-id="f2639-123">String</span><span class="sxs-lookup"><span data-stu-id="f2639-123">String</span></span>          | <span data-ttu-id="f2639-124">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="f2639-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="f2639-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2639-125">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f2639-126">Relações</span><span class="sxs-lookup"><span data-stu-id="f2639-126">Relationships</span></span>

<span data-ttu-id="f2639-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2639-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2639-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2639-128">JSON representation</span></span>

<span data-ttu-id="f2639-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2639-129">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="f2639-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2639-130">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "status": "completed"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
