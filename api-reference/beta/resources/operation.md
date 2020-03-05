---
title: tipo de recurso Operation
description: O status de uma operação de execução longa.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 44d1bdfdca902652d77d978b0eae4cffdf359f39
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522155"
---
# <a name="operation-resource-type"></a><span data-ttu-id="11dba-103">tipo de recurso Operation</span><span class="sxs-lookup"><span data-stu-id="11dba-103">operation resource type</span></span>

<span data-ttu-id="11dba-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="11dba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11dba-105">O status de uma operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="11dba-105">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="11dba-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="11dba-106">Methods</span></span>

<span data-ttu-id="11dba-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11dba-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="11dba-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11dba-108">Properties</span></span>

| <span data-ttu-id="11dba-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11dba-109">Property</span></span>           | <span data-ttu-id="11dba-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="11dba-110">Type</span></span>            | <span data-ttu-id="11dba-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="11dba-111">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="11dba-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11dba-112">createdDateTime</span></span>    | <span data-ttu-id="11dba-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11dba-113">DateTimeOffset</span></span>  | <span data-ttu-id="11dba-114">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="11dba-114">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="11dba-115">id</span><span class="sxs-lookup"><span data-stu-id="11dba-115">id</span></span>                 | <span data-ttu-id="11dba-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11dba-116">String</span></span>          | <span data-ttu-id="11dba-117">A ID da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11dba-117">The operation id. Read-only.</span></span> <span data-ttu-id="11dba-118">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="11dba-118">Server generated.</span></span>                                  |
| <span data-ttu-id="11dba-119">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="11dba-119">lastActionDateTime</span></span> | <span data-ttu-id="11dba-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11dba-120">DateTimeOffset</span></span>  | <span data-ttu-id="11dba-121">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="11dba-121">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="11dba-122">status</span><span class="sxs-lookup"><span data-stu-id="11dba-122">status</span></span>             | <span data-ttu-id="11dba-123">String</span><span class="sxs-lookup"><span data-stu-id="11dba-123">String</span></span>          | <span data-ttu-id="11dba-124">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="11dba-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="11dba-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="11dba-125">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="11dba-126">Relações</span><span class="sxs-lookup"><span data-stu-id="11dba-126">Relationships</span></span>

<span data-ttu-id="11dba-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11dba-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11dba-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11dba-128">JSON representation</span></span>

<span data-ttu-id="11dba-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11dba-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="11dba-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11dba-130">Example</span></span>

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
