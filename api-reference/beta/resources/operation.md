---
title: tipo de recurso Operation
description: O status de uma operação de execução longa.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: billbliss
ms.openlocfilehash: f57b9f14603fdeae539e872d87b5af2645cedef0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998506"
---
# <a name="operation-resource-type"></a><span data-ttu-id="26754-103">tipo de recurso Operation</span><span class="sxs-lookup"><span data-stu-id="26754-103">operation resource type</span></span>

<span data-ttu-id="26754-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26754-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26754-105">O status de uma operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="26754-105">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="26754-106">Methods</span><span class="sxs-lookup"><span data-stu-id="26754-106">Methods</span></span>

<span data-ttu-id="26754-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26754-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="26754-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26754-108">Properties</span></span>

| <span data-ttu-id="26754-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26754-109">Property</span></span>           | <span data-ttu-id="26754-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="26754-110">Type</span></span>            | <span data-ttu-id="26754-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="26754-111">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="26754-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26754-112">createdDateTime</span></span>    | <span data-ttu-id="26754-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26754-113">DateTimeOffset</span></span>  | <span data-ttu-id="26754-114">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="26754-114">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="26754-115">id</span><span class="sxs-lookup"><span data-stu-id="26754-115">id</span></span>                 | <span data-ttu-id="26754-116">String</span><span class="sxs-lookup"><span data-stu-id="26754-116">String</span></span>          | <span data-ttu-id="26754-117">A ID da operação. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26754-117">The operation id. Read-only.</span></span> <span data-ttu-id="26754-118">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="26754-118">Server generated.</span></span>                                  |
| <span data-ttu-id="26754-119">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="26754-119">lastActionDateTime</span></span> | <span data-ttu-id="26754-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26754-120">DateTimeOffset</span></span>  | <span data-ttu-id="26754-121">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="26754-121">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="26754-122">status</span><span class="sxs-lookup"><span data-stu-id="26754-122">status</span></span>             | <span data-ttu-id="26754-123">String</span><span class="sxs-lookup"><span data-stu-id="26754-123">String</span></span>          | <span data-ttu-id="26754-124">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="26754-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="26754-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26754-125">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="26754-126">Relações</span><span class="sxs-lookup"><span data-stu-id="26754-126">Relationships</span></span>

<span data-ttu-id="26754-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26754-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26754-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26754-128">JSON representation</span></span>

<span data-ttu-id="26754-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="26754-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="26754-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26754-130">Example</span></span>

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


