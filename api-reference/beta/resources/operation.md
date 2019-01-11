---
title: tipo de recurso de operação
description: O status de uma operação de execução longa.
localization_priority: Normal
ms.openlocfilehash: 760aeedb67b987fc22a5eef969e2214f6dfd05b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830342"
---
# <a name="operation-resource-type"></a><span data-ttu-id="c883f-103">tipo de recurso de operação</span><span class="sxs-lookup"><span data-stu-id="c883f-103">operation resource type</span></span>

> <span data-ttu-id="c883f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c883f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c883f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c883f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c883f-106">O status de uma operação de execução longa.</span><span class="sxs-lookup"><span data-stu-id="c883f-106">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="c883f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c883f-107">Methods</span></span>

<span data-ttu-id="c883f-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c883f-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="c883f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c883f-109">Properties</span></span>

| <span data-ttu-id="c883f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c883f-110">Property</span></span>           | <span data-ttu-id="c883f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c883f-111">Type</span></span>            | <span data-ttu-id="c883f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c883f-112">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="c883f-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c883f-113">createdDateTime</span></span>    | <span data-ttu-id="c883f-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c883f-114">DateTimeOffset</span></span>  | <span data-ttu-id="c883f-115">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="c883f-115">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="c883f-116">id</span><span class="sxs-lookup"><span data-stu-id="c883f-116">id</span></span>                 | <span data-ttu-id="c883f-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c883f-117">String</span></span>          | <span data-ttu-id="c883f-118">A id da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c883f-118">The operation id. Read-only.</span></span> <span data-ttu-id="c883f-119">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="c883f-119">Server generated.</span></span>                                  |
| <span data-ttu-id="c883f-120">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="c883f-120">lastActionDateTime</span></span> | <span data-ttu-id="c883f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c883f-121">DateTimeOffset</span></span>  | <span data-ttu-id="c883f-122">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="c883f-122">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="c883f-123">status</span><span class="sxs-lookup"><span data-stu-id="c883f-123">status</span></span>             | <span data-ttu-id="c883f-124">String</span><span class="sxs-lookup"><span data-stu-id="c883f-124">String</span></span>          | <span data-ttu-id="c883f-125">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="c883f-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="c883f-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c883f-126">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c883f-127">Relações</span><span class="sxs-lookup"><span data-stu-id="c883f-127">Relationships</span></span>

<span data-ttu-id="c883f-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c883f-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c883f-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c883f-129">JSON representation</span></span>

<span data-ttu-id="c883f-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c883f-130">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="c883f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c883f-131">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
