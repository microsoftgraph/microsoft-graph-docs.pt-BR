---
title: tipo de recurso de commsOperation
description: O status de determinadas operações de execução longa.
author: VinodRavichandran
ms.openlocfilehash: 09d3f81e8f6307850d94cfab43f98426dae47a5f
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380349"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="b6ace-103">tipo de recurso de commsOperation</span><span class="sxs-lookup"><span data-stu-id="b6ace-103">commsOperation resource type</span></span>

> <span data-ttu-id="b6ace-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b6ace-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6ace-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b6ace-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b6ace-106">O status de determinadas operações de execução longa.</span><span class="sxs-lookup"><span data-stu-id="b6ace-106">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="b6ace-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b6ace-107">Methods</span></span>
<span data-ttu-id="b6ace-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6ace-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="b6ace-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6ace-109">Properties</span></span>

| <span data-ttu-id="b6ace-110">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="b6ace-110">Property</span></span>           | <span data-ttu-id="b6ace-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6ace-111">Type</span></span>                        | <span data-ttu-id="b6ace-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6ace-112">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="b6ace-113">clientContext</span><span class="sxs-lookup"><span data-stu-id="b6ace-113">clientContext</span></span>      | <span data-ttu-id="b6ace-114">String</span><span class="sxs-lookup"><span data-stu-id="b6ace-114">String</span></span>                      | <span data-ttu-id="b6ace-115">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="b6ace-115">The client context.</span></span>                                                             |
| <span data-ttu-id="b6ace-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6ace-116">createdDateTime</span></span>    | <span data-ttu-id="b6ace-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6ace-117">DateTimeOffset</span></span>              | <span data-ttu-id="b6ace-118">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="b6ace-118">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="b6ace-119">id</span><span class="sxs-lookup"><span data-stu-id="b6ace-119">id</span></span>                 | <span data-ttu-id="b6ace-120">String</span><span class="sxs-lookup"><span data-stu-id="b6ace-120">String</span></span>                      | <span data-ttu-id="b6ace-121">A id da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6ace-121">The operation id. Read-only.</span></span> <span data-ttu-id="b6ace-122">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="b6ace-122">Server generated.</span></span>                                  |
| <span data-ttu-id="b6ace-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="b6ace-123">lastActionDateTime</span></span> | <span data-ttu-id="b6ace-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6ace-124">DateTimeOffset</span></span>              | <span data-ttu-id="b6ace-125">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="b6ace-125">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="b6ace-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b6ace-126">resultInfo</span></span>         | [<span data-ttu-id="b6ace-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="b6ace-127">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="b6ace-128">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="b6ace-128">The result information.</span></span> <span data-ttu-id="b6ace-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6ace-129">Read-only.</span></span> <span data-ttu-id="b6ace-130">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="b6ace-130">Server generated.</span></span>                            |
| <span data-ttu-id="b6ace-131">status</span><span class="sxs-lookup"><span data-stu-id="b6ace-131">status</span></span>             | <span data-ttu-id="b6ace-132">String</span><span class="sxs-lookup"><span data-stu-id="b6ace-132">String</span></span>                      | <span data-ttu-id="b6ace-133">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="b6ace-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="b6ace-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6ace-134">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b6ace-135">Relações</span><span class="sxs-lookup"><span data-stu-id="b6ace-135">Relationships</span></span>
<span data-ttu-id="b6ace-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6ace-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6ace-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6ace-137">JSON representation</span></span>

<span data-ttu-id="b6ace-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6ace-138">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="b6ace-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6ace-139">Example</span></span>

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
