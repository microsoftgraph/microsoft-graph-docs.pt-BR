---
title: tipo de recurso commsOperation
description: O status de determinadas operações de longa duração.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 34e6ff32c250308e71e05cb5d5c4d04d5671535d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341355"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="3a70b-103">tipo de recurso commsOperation</span><span class="sxs-lookup"><span data-stu-id="3a70b-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a70b-104">O status de determinadas operações de longa duração.</span><span class="sxs-lookup"><span data-stu-id="3a70b-104">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="3a70b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="3a70b-105">Methods</span></span>
<span data-ttu-id="3a70b-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a70b-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="3a70b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a70b-107">Properties</span></span>

| <span data-ttu-id="3a70b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a70b-108">Property</span></span>           | <span data-ttu-id="3a70b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a70b-109">Type</span></span>                        | <span data-ttu-id="3a70b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a70b-110">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="3a70b-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="3a70b-111">clientContext</span></span>      | <span data-ttu-id="3a70b-112">String</span><span class="sxs-lookup"><span data-stu-id="3a70b-112">String</span></span>                      | <span data-ttu-id="3a70b-113">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="3a70b-113">The client context.</span></span>                                                             |
| <span data-ttu-id="3a70b-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a70b-114">createdDateTime</span></span>    | <span data-ttu-id="3a70b-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a70b-115">DateTimeOffset</span></span>              | <span data-ttu-id="3a70b-116">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="3a70b-116">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="3a70b-117">id</span><span class="sxs-lookup"><span data-stu-id="3a70b-117">id</span></span>                 | <span data-ttu-id="3a70b-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a70b-118">String</span></span>                      | <span data-ttu-id="3a70b-119">A ID da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3a70b-119">The operation id. Read-only.</span></span> <span data-ttu-id="3a70b-120">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="3a70b-120">Server generated.</span></span>                                  |
| <span data-ttu-id="3a70b-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="3a70b-121">lastActionDateTime</span></span> | <span data-ttu-id="3a70b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a70b-122">DateTimeOffset</span></span>              | <span data-ttu-id="3a70b-123">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="3a70b-123">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="3a70b-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="3a70b-124">resultInfo</span></span>         | [<span data-ttu-id="3a70b-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="3a70b-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="3a70b-126">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="3a70b-126">The result information.</span></span> <span data-ttu-id="3a70b-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3a70b-127">Read-only.</span></span> <span data-ttu-id="3a70b-128">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="3a70b-128">Server generated.</span></span>                            |
| <span data-ttu-id="3a70b-129">status</span><span class="sxs-lookup"><span data-stu-id="3a70b-129">status</span></span>             | <span data-ttu-id="3a70b-130">String</span><span class="sxs-lookup"><span data-stu-id="3a70b-130">String</span></span>                      | <span data-ttu-id="3a70b-131">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="3a70b-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="3a70b-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3a70b-132">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3a70b-133">Relações</span><span class="sxs-lookup"><span data-stu-id="3a70b-133">Relationships</span></span>
<span data-ttu-id="3a70b-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a70b-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a70b-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a70b-135">JSON representation</span></span>

<span data-ttu-id="3a70b-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a70b-136">The following is a JSON representation of the resource.</span></span>

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
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="3a70b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a70b-137">Example</span></span>

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
    "@odata.type": "microsoft.graph.resultInfo",
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
  "suppressions": []
}
-->
