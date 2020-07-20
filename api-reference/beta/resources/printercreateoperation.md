---
title: tipo de recurso printerCreateOperation
description: Representa uma operação de registro de impressora de longa execução. Derivado de reoperation.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 54f458e14cbda209d9c2d85f08df4c106db6ab00
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007159"
---
# <a name="printercreateoperation-resource-type"></a><span data-ttu-id="69f4f-104">tipo de recurso printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="69f4f-104">printerCreateOperation resource type</span></span>

<span data-ttu-id="69f4f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69f4f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69f4f-106">Representa uma operação de registro de impressora de longa execução.</span><span class="sxs-lookup"><span data-stu-id="69f4f-106">Represents a long-running printer registration operation.</span></span> <span data-ttu-id="69f4f-107">Derivado de [Reoperation](printoperation.md).</span><span class="sxs-lookup"><span data-stu-id="69f4f-107">Derived from [printOperation](printoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="69f4f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="69f4f-108">Methods</span></span>

| <span data-ttu-id="69f4f-109">Método</span><span class="sxs-lookup"><span data-stu-id="69f4f-109">Method</span></span>       | <span data-ttu-id="69f4f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="69f4f-110">Return Type</span></span> | <span data-ttu-id="69f4f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="69f4f-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="69f4f-112">Operação get</span><span class="sxs-lookup"><span data-stu-id="69f4f-112">Get operation</span></span>](../api/printoperation-get.md) | [<span data-ttu-id="69f4f-113">Operação de reoperação</span><span class="sxs-lookup"><span data-stu-id="69f4f-113">printOperation</span></span>](printoperation.md) | <span data-ttu-id="69f4f-114">Recupere uma operação de execução longa dentro do usuário atual ou do locatário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="69f4f-114">Retrieve a long-running operation within current user or app's tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="69f4f-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69f4f-115">Properties</span></span>
| <span data-ttu-id="69f4f-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69f4f-116">Property</span></span>     | <span data-ttu-id="69f4f-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="69f4f-117">Type</span></span>        | <span data-ttu-id="69f4f-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="69f4f-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="69f4f-119">id</span><span class="sxs-lookup"><span data-stu-id="69f4f-119">id</span></span>|<span data-ttu-id="69f4f-120">String</span><span class="sxs-lookup"><span data-stu-id="69f4f-120">String</span></span>|<span data-ttu-id="69f4f-121">O identificador da operação.</span><span class="sxs-lookup"><span data-stu-id="69f4f-121">The operation's identifier.</span></span> <span data-ttu-id="69f4f-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69f4f-122">Read-only.</span></span>|
|<span data-ttu-id="69f4f-123">status</span><span class="sxs-lookup"><span data-stu-id="69f4f-123">status</span></span>|[<span data-ttu-id="69f4f-124">printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="69f4f-124">printOperationStatus</span></span>](printoperationstatus.md)|<span data-ttu-id="69f4f-125">O status da operação de registro.</span><span class="sxs-lookup"><span data-stu-id="69f4f-125">The status of the registration operation.</span></span> <span data-ttu-id="69f4f-126">Contém o andamento da operação e se ela foi concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="69f4f-126">Contains the operation's progress and whether it completed successfully.</span></span> <span data-ttu-id="69f4f-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69f4f-127">Read-only.</span></span>|
|<span data-ttu-id="69f4f-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69f4f-128">createdDateTime</span></span>|<span data-ttu-id="69f4f-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69f4f-129">DateTimeOffset</span></span>|<span data-ttu-id="69f4f-130">O DateTimeOffset quando a operação foi criada.</span><span class="sxs-lookup"><span data-stu-id="69f4f-130">The DateTimeOffset when the operation was created.</span></span> <span data-ttu-id="69f4f-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69f4f-131">Read-only.</span></span>|
|<span data-ttu-id="69f4f-132">certificado</span><span class="sxs-lookup"><span data-stu-id="69f4f-132">certificate</span></span>|<span data-ttu-id="69f4f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69f4f-133">String</span></span>|<span data-ttu-id="69f4f-134">O certificado assinado criado durante o processo de registro.</span><span class="sxs-lookup"><span data-stu-id="69f4f-134">The signed certificate created during the registration process.</span></span> <span data-ttu-id="69f4f-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69f4f-135">Read-only.</span></span>|
|<span data-ttu-id="69f4f-136">impressora</span><span class="sxs-lookup"><span data-stu-id="69f4f-136">printer</span></span>|[<span data-ttu-id="69f4f-137">impressora</span><span class="sxs-lookup"><span data-stu-id="69f4f-137">printer</span></span>](printer.md)|<span data-ttu-id="69f4f-138">A entidade de impressora criada.</span><span class="sxs-lookup"><span data-stu-id="69f4f-138">The created printer entity.</span></span> <span data-ttu-id="69f4f-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69f4f-139">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69f4f-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69f4f-140">JSON representation</span></span>

<span data-ttu-id="69f4f-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69f4f-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerCreateOperation",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
    "id": "String (identifier)",
    "status": {"@odata.type": "microsoft.graph.printOperationStatus"},
    "createdDateTime": "2020-06-15T19:54:14.853Z",
    "certificate": "",
    "printer": {"@odata.type": "microsoft.graph.printer"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerCreateOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->