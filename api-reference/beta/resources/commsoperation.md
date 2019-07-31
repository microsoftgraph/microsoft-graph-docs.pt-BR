---
title: tipo de recurso commsOperation
description: O status de determinadas operações de longa duração.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a10b652179a8a3d369c07d34cb2681c4986b3abf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012895"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="c7a06-103">tipo de recurso commsOperation</span><span class="sxs-lookup"><span data-stu-id="c7a06-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7a06-104">O status de determinadas operações de longa duração.</span><span class="sxs-lookup"><span data-stu-id="c7a06-104">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="c7a06-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c7a06-105">Methods</span></span>
<span data-ttu-id="c7a06-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7a06-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="c7a06-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7a06-107">Properties</span></span>

| <span data-ttu-id="c7a06-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7a06-108">Property</span></span>           | <span data-ttu-id="c7a06-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7a06-109">Type</span></span>                        | <span data-ttu-id="c7a06-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7a06-110">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="c7a06-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="c7a06-111">clientContext</span></span>      | <span data-ttu-id="c7a06-112">String</span><span class="sxs-lookup"><span data-stu-id="c7a06-112">String</span></span>                      | <span data-ttu-id="c7a06-113">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="c7a06-113">The client context.</span></span>                                                             |
| <span data-ttu-id="c7a06-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7a06-114">createdDateTime</span></span>    | <span data-ttu-id="c7a06-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7a06-115">DateTimeOffset</span></span>              | <span data-ttu-id="c7a06-116">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="c7a06-116">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="c7a06-117">id</span><span class="sxs-lookup"><span data-stu-id="c7a06-117">id</span></span>                 | <span data-ttu-id="c7a06-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7a06-118">String</span></span>                      | <span data-ttu-id="c7a06-119">A ID da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7a06-119">The operation id. Read-only.</span></span> <span data-ttu-id="c7a06-120">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="c7a06-120">Server generated.</span></span>                                  |
| <span data-ttu-id="c7a06-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c7a06-121">lastActionDateTime</span></span> | <span data-ttu-id="c7a06-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7a06-122">DateTimeOffset</span></span>              | <span data-ttu-id="c7a06-123">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="c7a06-123">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="c7a06-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c7a06-124">resultInfo</span></span>         | [<span data-ttu-id="c7a06-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="c7a06-125">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="c7a06-126">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="c7a06-126">The result information.</span></span> <span data-ttu-id="c7a06-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7a06-127">Read-only.</span></span> <span data-ttu-id="c7a06-128">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="c7a06-128">Server generated.</span></span>                            |
| <span data-ttu-id="c7a06-129">status</span><span class="sxs-lookup"><span data-stu-id="c7a06-129">status</span></span>             | <span data-ttu-id="c7a06-130">String</span><span class="sxs-lookup"><span data-stu-id="c7a06-130">String</span></span>                      | <span data-ttu-id="c7a06-131">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="c7a06-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="c7a06-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7a06-132">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c7a06-133">Relações</span><span class="sxs-lookup"><span data-stu-id="c7a06-133">Relationships</span></span>
<span data-ttu-id="c7a06-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7a06-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7a06-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7a06-135">JSON representation</span></span>

<span data-ttu-id="c7a06-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7a06-136">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="c7a06-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7a06-137">Example</span></span>

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
