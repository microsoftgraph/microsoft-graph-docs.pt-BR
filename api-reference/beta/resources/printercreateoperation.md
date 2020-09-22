---
title: tipo de recurso printerCreateOperation
description: Representa uma operação de registro de impressora de longa execução. Derivado de reoperation.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 3ae18e201f5b768de9cc1456de186fdd6b9336b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048852"
---
# <a name="printercreateoperation-resource-type"></a><span data-ttu-id="8359b-104">tipo de recurso printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="8359b-104">printerCreateOperation resource type</span></span>

<span data-ttu-id="8359b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8359b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8359b-106">Representa uma operação de registro de impressora de longa execução.</span><span class="sxs-lookup"><span data-stu-id="8359b-106">Represents a long-running printer registration operation.</span></span> <span data-ttu-id="8359b-107">Derivado de [Reoperation](printoperation.md).</span><span class="sxs-lookup"><span data-stu-id="8359b-107">Derived from [printOperation](printoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8359b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="8359b-108">Methods</span></span>

| <span data-ttu-id="8359b-109">Método</span><span class="sxs-lookup"><span data-stu-id="8359b-109">Method</span></span>       | <span data-ttu-id="8359b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8359b-110">Return Type</span></span> | <span data-ttu-id="8359b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8359b-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8359b-112">Operação get</span><span class="sxs-lookup"><span data-stu-id="8359b-112">Get operation</span></span>](../api/printoperation-get.md) | [<span data-ttu-id="8359b-113">printOperation</span><span class="sxs-lookup"><span data-stu-id="8359b-113">printOperation</span></span>](printoperation.md) | <span data-ttu-id="8359b-114">Recupere uma operação de execução longa dentro do usuário atual ou do locatário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8359b-114">Retrieve a long-running operation within current user or app's tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="8359b-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8359b-115">Properties</span></span>
| <span data-ttu-id="8359b-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8359b-116">Property</span></span>     | <span data-ttu-id="8359b-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="8359b-117">Type</span></span>        | <span data-ttu-id="8359b-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="8359b-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8359b-119">id</span><span class="sxs-lookup"><span data-stu-id="8359b-119">id</span></span>|<span data-ttu-id="8359b-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8359b-120">String</span></span>|<span data-ttu-id="8359b-121">O identificador da operação.</span><span class="sxs-lookup"><span data-stu-id="8359b-121">The operation's identifier.</span></span> <span data-ttu-id="8359b-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8359b-122">Read-only.</span></span>|
|<span data-ttu-id="8359b-123">status</span><span class="sxs-lookup"><span data-stu-id="8359b-123">status</span></span>|[<span data-ttu-id="8359b-124">printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="8359b-124">printOperationStatus</span></span>](printoperationstatus.md)|<span data-ttu-id="8359b-125">O status da operação de registro.</span><span class="sxs-lookup"><span data-stu-id="8359b-125">The status of the registration operation.</span></span> <span data-ttu-id="8359b-126">Contém o andamento da operação e se ela foi concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="8359b-126">Contains the operation's progress and whether it completed successfully.</span></span> <span data-ttu-id="8359b-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8359b-127">Read-only.</span></span>|
|<span data-ttu-id="8359b-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8359b-128">createdDateTime</span></span>|<span data-ttu-id="8359b-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8359b-129">DateTimeOffset</span></span>|<span data-ttu-id="8359b-130">O DateTimeOffset quando a operação foi criada.</span><span class="sxs-lookup"><span data-stu-id="8359b-130">The DateTimeOffset when the operation was created.</span></span> <span data-ttu-id="8359b-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8359b-131">Read-only.</span></span>|
|<span data-ttu-id="8359b-132">certificado</span><span class="sxs-lookup"><span data-stu-id="8359b-132">certificate</span></span>|<span data-ttu-id="8359b-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8359b-133">String</span></span>|<span data-ttu-id="8359b-134">O certificado assinado criado durante o processo de registro.</span><span class="sxs-lookup"><span data-stu-id="8359b-134">The signed certificate created during the registration process.</span></span> <span data-ttu-id="8359b-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8359b-135">Read-only.</span></span>|
|<span data-ttu-id="8359b-136">impressora</span><span class="sxs-lookup"><span data-stu-id="8359b-136">printer</span></span>|[<span data-ttu-id="8359b-137">impressora</span><span class="sxs-lookup"><span data-stu-id="8359b-137">printer</span></span>](printer.md)|<span data-ttu-id="8359b-138">A entidade de impressora criada.</span><span class="sxs-lookup"><span data-stu-id="8359b-138">The created printer entity.</span></span> <span data-ttu-id="8359b-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8359b-139">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8359b-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8359b-140">JSON representation</span></span>

<span data-ttu-id="8359b-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8359b-141">The following is a JSON representation of the resource.</span></span>

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

