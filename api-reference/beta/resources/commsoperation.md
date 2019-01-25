---
title: tipo de recurso de commsOperation
description: O status de determinadas operações de execução longa.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b7914bd9692b4d9a94294f9a09659467e10550a6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515745"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="0ed4f-103">tipo de recurso de commsOperation</span><span class="sxs-lookup"><span data-stu-id="0ed4f-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ed4f-104">O status de determinadas operações de execução longa.</span><span class="sxs-lookup"><span data-stu-id="0ed4f-104">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="0ed4f-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="0ed4f-105">Methods</span></span>
<span data-ttu-id="0ed4f-106">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0ed4f-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="0ed4f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ed4f-107">Properties</span></span>

| <span data-ttu-id="0ed4f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ed4f-108">Property</span></span>           | <span data-ttu-id="0ed4f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ed4f-109">Type</span></span>                        | <span data-ttu-id="0ed4f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ed4f-110">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="0ed4f-111">ClientContext</span><span class="sxs-lookup"><span data-stu-id="0ed4f-111">clientContext</span></span>      | <span data-ttu-id="0ed4f-112">String</span><span class="sxs-lookup"><span data-stu-id="0ed4f-112">String</span></span>                      | <span data-ttu-id="0ed4f-113">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="0ed4f-113">The client context.</span></span>                                                             |
| <span data-ttu-id="0ed4f-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ed4f-114">createdDateTime</span></span>    | <span data-ttu-id="0ed4f-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ed4f-115">DateTimeOffset</span></span>              | <span data-ttu-id="0ed4f-116">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="0ed4f-116">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="0ed4f-117">id</span><span class="sxs-lookup"><span data-stu-id="0ed4f-117">id</span></span>                 | <span data-ttu-id="0ed4f-118">String</span><span class="sxs-lookup"><span data-stu-id="0ed4f-118">String</span></span>                      | <span data-ttu-id="0ed4f-119">A id da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ed4f-119">The operation id. Read-only.</span></span> <span data-ttu-id="0ed4f-120">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="0ed4f-120">Server generated.</span></span>                                  |
| <span data-ttu-id="0ed4f-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="0ed4f-121">lastActionDateTime</span></span> | <span data-ttu-id="0ed4f-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ed4f-122">DateTimeOffset</span></span>              | <span data-ttu-id="0ed4f-123">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="0ed4f-123">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="0ed4f-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0ed4f-124">resultInfo</span></span>         | [<span data-ttu-id="0ed4f-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="0ed4f-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="0ed4f-126">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="0ed4f-126">The result information.</span></span> <span data-ttu-id="0ed4f-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ed4f-127">Read-only.</span></span> <span data-ttu-id="0ed4f-128">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="0ed4f-128">Server generated.</span></span>                            |
| <span data-ttu-id="0ed4f-129">status</span><span class="sxs-lookup"><span data-stu-id="0ed4f-129">status</span></span>             | <span data-ttu-id="0ed4f-130">String</span><span class="sxs-lookup"><span data-stu-id="0ed4f-130">String</span></span>                      | <span data-ttu-id="0ed4f-131">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0ed4f-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="0ed4f-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ed4f-132">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0ed4f-133">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="0ed4f-133">Relationships</span></span>
<span data-ttu-id="0ed4f-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ed4f-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ed4f-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ed4f-135">JSON representation</span></span>

<span data-ttu-id="0ed4f-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ed4f-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": { "@odata.type": "#microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="0ed4f-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ed4f-137">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "resultInfo": {
    "@odata.type": "#microsoft.graph.resultInfo",
    "code": "200"
  },
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/commsoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
