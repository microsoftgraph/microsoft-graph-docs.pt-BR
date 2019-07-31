---
title: tipo de recurso Operation
description: O status de uma operação de execução longa.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 237e16373db30db9f4a9ed61c6182f6dd826d956
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966360"
---
# <a name="operation-resource-type"></a><span data-ttu-id="124b2-103">tipo de recurso Operation</span><span class="sxs-lookup"><span data-stu-id="124b2-103">operation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="124b2-104">O status de uma operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="124b2-104">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="124b2-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="124b2-105">Methods</span></span>

<span data-ttu-id="124b2-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="124b2-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="124b2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="124b2-107">Properties</span></span>

| <span data-ttu-id="124b2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="124b2-108">Property</span></span>           | <span data-ttu-id="124b2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="124b2-109">Type</span></span>            | <span data-ttu-id="124b2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="124b2-110">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="124b2-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="124b2-111">createdDateTime</span></span>    | <span data-ttu-id="124b2-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="124b2-112">DateTimeOffset</span></span>  | <span data-ttu-id="124b2-113">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="124b2-113">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="124b2-114">id</span><span class="sxs-lookup"><span data-stu-id="124b2-114">id</span></span>                 | <span data-ttu-id="124b2-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="124b2-115">String</span></span>          | <span data-ttu-id="124b2-116">A ID da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="124b2-116">The operation id. Read-only.</span></span> <span data-ttu-id="124b2-117">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="124b2-117">Server generated.</span></span>                                  |
| <span data-ttu-id="124b2-118">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="124b2-118">lastActionDateTime</span></span> | <span data-ttu-id="124b2-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="124b2-119">DateTimeOffset</span></span>  | <span data-ttu-id="124b2-120">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="124b2-120">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="124b2-121">status</span><span class="sxs-lookup"><span data-stu-id="124b2-121">status</span></span>             | <span data-ttu-id="124b2-122">String</span><span class="sxs-lookup"><span data-stu-id="124b2-122">String</span></span>          | <span data-ttu-id="124b2-123">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="124b2-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="124b2-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="124b2-124">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="124b2-125">Relações</span><span class="sxs-lookup"><span data-stu-id="124b2-125">Relationships</span></span>

<span data-ttu-id="124b2-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="124b2-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="124b2-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="124b2-127">JSON representation</span></span>

<span data-ttu-id="124b2-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="124b2-128">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="124b2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="124b2-129">Example</span></span>

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
