---
title: tipo de recurso de operação
description: O status de uma operação de execução longa.
localization_priority: Normal
ms.openlocfilehash: 3ad9848387dab2de928f7ace2fa4b905720be615
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520183"
---
# <a name="operation-resource-type"></a><span data-ttu-id="b75bd-103">tipo de recurso de operação</span><span class="sxs-lookup"><span data-stu-id="b75bd-103">operation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b75bd-104">O status de uma operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="b75bd-104">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="b75bd-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="b75bd-105">Methods</span></span>

<span data-ttu-id="b75bd-106">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b75bd-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="b75bd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b75bd-107">Properties</span></span>

| <span data-ttu-id="b75bd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b75bd-108">Property</span></span>           | <span data-ttu-id="b75bd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b75bd-109">Type</span></span>            | <span data-ttu-id="b75bd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b75bd-110">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="b75bd-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b75bd-111">createdDateTime</span></span>    | <span data-ttu-id="b75bd-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b75bd-112">DateTimeOffset</span></span>  | <span data-ttu-id="b75bd-113">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="b75bd-113">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="b75bd-114">id</span><span class="sxs-lookup"><span data-stu-id="b75bd-114">id</span></span>                 | <span data-ttu-id="b75bd-115">String</span><span class="sxs-lookup"><span data-stu-id="b75bd-115">String</span></span>          | <span data-ttu-id="b75bd-116">A id da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b75bd-116">The operation id. Read-only.</span></span> <span data-ttu-id="b75bd-117">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="b75bd-117">Server generated.</span></span>                                  |
| <span data-ttu-id="b75bd-118">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="b75bd-118">lastActionDateTime</span></span> | <span data-ttu-id="b75bd-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b75bd-119">DateTimeOffset</span></span>  | <span data-ttu-id="b75bd-120">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="b75bd-120">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="b75bd-121">status</span><span class="sxs-lookup"><span data-stu-id="b75bd-121">status</span></span>             | <span data-ttu-id="b75bd-122">String</span><span class="sxs-lookup"><span data-stu-id="b75bd-122">String</span></span>          | <span data-ttu-id="b75bd-123">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="b75bd-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="b75bd-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b75bd-124">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b75bd-125">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="b75bd-125">Relationships</span></span>

<span data-ttu-id="b75bd-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b75bd-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b75bd-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b75bd-127">JSON representation</span></span>

<span data-ttu-id="b75bd-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b75bd-128">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="b75bd-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b75bd-129">Example</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/operation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
