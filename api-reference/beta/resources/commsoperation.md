---
title: tipo de recurso de commsOperation
description: O status de determinadas operações de execução longa.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 79fc6801e95854b2530f8a28c13f7180ed02203f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957722"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="822b8-103">tipo de recurso de commsOperation</span><span class="sxs-lookup"><span data-stu-id="822b8-103">commsOperation resource type</span></span>

> <span data-ttu-id="822b8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="822b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="822b8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="822b8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="822b8-106">O status de determinadas operações de execução longa.</span><span class="sxs-lookup"><span data-stu-id="822b8-106">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="822b8-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="822b8-107">Methods</span></span>
<span data-ttu-id="822b8-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="822b8-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="822b8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="822b8-109">Properties</span></span>

| <span data-ttu-id="822b8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="822b8-110">Property</span></span>           | <span data-ttu-id="822b8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="822b8-111">Type</span></span>                        | <span data-ttu-id="822b8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="822b8-112">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="822b8-113">clientContext</span><span class="sxs-lookup"><span data-stu-id="822b8-113">clientContext</span></span>      | <span data-ttu-id="822b8-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="822b8-114">String</span></span>                      | <span data-ttu-id="822b8-115">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="822b8-115">The client context.</span></span>                                                             |
| <span data-ttu-id="822b8-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="822b8-116">createdDateTime</span></span>    | <span data-ttu-id="822b8-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="822b8-117">DateTimeOffset</span></span>              | <span data-ttu-id="822b8-118">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="822b8-118">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="822b8-119">id</span><span class="sxs-lookup"><span data-stu-id="822b8-119">id</span></span>                 | <span data-ttu-id="822b8-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="822b8-120">String</span></span>                      | <span data-ttu-id="822b8-121">A id da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="822b8-121">The operation id. Read-only.</span></span> <span data-ttu-id="822b8-122">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="822b8-122">Server generated.</span></span>                                  |
| <span data-ttu-id="822b8-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="822b8-123">lastActionDateTime</span></span> | <span data-ttu-id="822b8-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="822b8-124">DateTimeOffset</span></span>              | <span data-ttu-id="822b8-125">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="822b8-125">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="822b8-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="822b8-126">resultInfo</span></span>         | [<span data-ttu-id="822b8-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="822b8-127">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="822b8-128">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="822b8-128">The result information.</span></span> <span data-ttu-id="822b8-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="822b8-129">Read-only.</span></span> <span data-ttu-id="822b8-130">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="822b8-130">Server generated.</span></span>                            |
| <span data-ttu-id="822b8-131">status</span><span class="sxs-lookup"><span data-stu-id="822b8-131">status</span></span>             | <span data-ttu-id="822b8-132">String</span><span class="sxs-lookup"><span data-stu-id="822b8-132">String</span></span>                      | <span data-ttu-id="822b8-133">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="822b8-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="822b8-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="822b8-134">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="822b8-135">Relações</span><span class="sxs-lookup"><span data-stu-id="822b8-135">Relationships</span></span>
<span data-ttu-id="822b8-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="822b8-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="822b8-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="822b8-137">JSON representation</span></span>

<span data-ttu-id="822b8-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="822b8-138">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="822b8-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="822b8-139">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
