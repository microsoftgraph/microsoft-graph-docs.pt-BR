---
title: tipo de recurso de multioperação
description: Representa uma operação de impressão universal de execução longa. Classe base para tipos de operação, como printerCreateOperation.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7b8f147106c6914fe8fbbb404ca0c78210c02026
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007145"
---
# <a name="printoperation-resource-type"></a><span data-ttu-id="4028d-104">tipo de recurso de multioperação</span><span class="sxs-lookup"><span data-stu-id="4028d-104">printOperation resource type</span></span>

<span data-ttu-id="4028d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4028d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4028d-106">Representa uma operação de impressão universal de execução longa.</span><span class="sxs-lookup"><span data-stu-id="4028d-106">Represents a long-running Universal Print operation.</span></span> <span data-ttu-id="4028d-107">Classe base para tipos de operação, como [printerCreateOperation](printercreateoperation.md).</span><span class="sxs-lookup"><span data-stu-id="4028d-107">Base class for operation types such as [printerCreateOperation](printercreateoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4028d-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="4028d-108">Methods</span></span>

| <span data-ttu-id="4028d-109">Método</span><span class="sxs-lookup"><span data-stu-id="4028d-109">Method</span></span>       | <span data-ttu-id="4028d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4028d-110">Return Type</span></span> | <span data-ttu-id="4028d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4028d-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4028d-112">Operação get</span><span class="sxs-lookup"><span data-stu-id="4028d-112">Get operation</span></span>](../api/printoperation-get.md) | [<span data-ttu-id="4028d-113">Operação de reoperação</span><span class="sxs-lookup"><span data-stu-id="4028d-113">printOperation</span></span>](printoperation.md) | <span data-ttu-id="4028d-114">Recupere uma operação de execução longa dentro do usuário atual ou do locatário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4028d-114">Retrieve a long-running operation within current user or app's tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="4028d-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4028d-115">Properties</span></span>
| <span data-ttu-id="4028d-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4028d-116">Property</span></span>     | <span data-ttu-id="4028d-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="4028d-117">Type</span></span>        | <span data-ttu-id="4028d-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="4028d-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4028d-119">id</span><span class="sxs-lookup"><span data-stu-id="4028d-119">id</span></span>|<span data-ttu-id="4028d-120">String</span><span class="sxs-lookup"><span data-stu-id="4028d-120">String</span></span>|<span data-ttu-id="4028d-121">O identificador da operação.</span><span class="sxs-lookup"><span data-stu-id="4028d-121">The operation's identifier.</span></span> <span data-ttu-id="4028d-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4028d-122">Read-only.</span></span>|
|<span data-ttu-id="4028d-123">status</span><span class="sxs-lookup"><span data-stu-id="4028d-123">status</span></span>|[<span data-ttu-id="4028d-124">printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="4028d-124">printOperationStatus</span></span>](printoperationstatus.md)|<span data-ttu-id="4028d-125">O status da operação.</span><span class="sxs-lookup"><span data-stu-id="4028d-125">The status of the operation.</span></span> <span data-ttu-id="4028d-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4028d-126">Read-only.</span></span>|
|<span data-ttu-id="4028d-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4028d-127">createdDateTime</span></span>|<span data-ttu-id="4028d-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4028d-128">DateTimeOffset</span></span>|<span data-ttu-id="4028d-129">O DateTimeOffset quando a operação foi criada.</span><span class="sxs-lookup"><span data-stu-id="4028d-129">The DateTimeOffset when the operation was created.</span></span> <span data-ttu-id="4028d-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4028d-130">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4028d-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4028d-131">JSON representation</span></span>

<span data-ttu-id="4028d-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4028d-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printOperation",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
    "id": "String (identifier)",
    "status": {"@odata.type": "microsoft.graph.printOperationStatus"},
    "createdDateTime": "2020-06-15T19:54:14.853Z"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->