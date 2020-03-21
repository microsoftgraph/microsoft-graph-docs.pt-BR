---
title: tipo de recurso printerShare
description: Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: a44cac259e9be653ca0e7b21c81b6c72224268b1
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895482"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="47827-103">tipo de recurso printerShare</span><span class="sxs-lookup"><span data-stu-id="47827-103">printerShare resource type</span></span>

<span data-ttu-id="47827-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47827-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47827-105">Representa uma impressora que pretende ser detectável por usuários e por aplicativos de impressão.</span><span class="sxs-lookup"><span data-stu-id="47827-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="47827-106">Methods</span><span class="sxs-lookup"><span data-stu-id="47827-106">Methods</span></span>

| <span data-ttu-id="47827-107">Método</span><span class="sxs-lookup"><span data-stu-id="47827-107">Method</span></span>       | <span data-ttu-id="47827-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="47827-108">Return Type</span></span> | <span data-ttu-id="47827-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="47827-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="47827-110">Listar printerShares</span><span class="sxs-lookup"><span data-stu-id="47827-110">List printerShares</span></span>](../api/print-list-printershares.md) | <span data-ttu-id="47827-111">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="47827-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="47827-112">Obtenha uma lista de compartilhamentos de impressora no locatário.</span><span class="sxs-lookup"><span data-stu-id="47827-112">Get a list of printer shares in the tenant.</span></span> |
| [<span data-ttu-id="47827-113">Obter printerShare</span><span class="sxs-lookup"><span data-stu-id="47827-113">Get printerShare</span></span>](../api/printershare-get.md) | [<span data-ttu-id="47827-114">printerShare</span><span class="sxs-lookup"><span data-stu-id="47827-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="47827-115">Ler propriedades e relações de um objeto printerShare.</span><span class="sxs-lookup"><span data-stu-id="47827-115">Read properties and relationships of a printerShare object.</span></span> |
| [<span data-ttu-id="47827-116">Update</span><span class="sxs-lookup"><span data-stu-id="47827-116">Update</span></span>](../api/printershare-update.md) | [<span data-ttu-id="47827-117">printerShare</span><span class="sxs-lookup"><span data-stu-id="47827-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="47827-118">Atualizar um objeto printerShare.</span><span class="sxs-lookup"><span data-stu-id="47827-118">Update a printerShare object.</span></span> |
| [<span data-ttu-id="47827-119">Delete</span><span class="sxs-lookup"><span data-stu-id="47827-119">Delete</span></span>](../api/printershare-delete.md) | <span data-ttu-id="47827-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47827-120">None</span></span> | <span data-ttu-id="47827-121">Descompartilhar uma impressora.</span><span class="sxs-lookup"><span data-stu-id="47827-121">Unshare a printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="47827-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47827-122">Properties</span></span>
| <span data-ttu-id="47827-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47827-123">Property</span></span>     | <span data-ttu-id="47827-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="47827-124">Type</span></span>        | <span data-ttu-id="47827-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="47827-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="47827-126">id</span><span class="sxs-lookup"><span data-stu-id="47827-126">id</span></span>|<span data-ttu-id="47827-127">String</span><span class="sxs-lookup"><span data-stu-id="47827-127">String</span></span>| <span data-ttu-id="47827-128">O identificador do printerShare.</span><span class="sxs-lookup"><span data-stu-id="47827-128">The printerShare's identifier.</span></span> <span data-ttu-id="47827-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="47827-129">Read-only.</span></span>|
|<span data-ttu-id="47827-130">name</span><span class="sxs-lookup"><span data-stu-id="47827-130">name</span></span>|<span data-ttu-id="47827-131">String</span><span class="sxs-lookup"><span data-stu-id="47827-131">String</span></span>|<span data-ttu-id="47827-132">O nome do compartilhamento de impressora que os clientes de impressão devem exibir.</span><span class="sxs-lookup"><span data-stu-id="47827-132">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="47827-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47827-133">createdDateTime</span></span>|<span data-ttu-id="47827-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47827-134">DateTimeOffset</span></span>|<span data-ttu-id="47827-135">O DateTimeOffset quando o compartilhamento da impressora foi criado.</span><span class="sxs-lookup"><span data-stu-id="47827-135">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="47827-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="47827-136">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47827-137">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="47827-137">Relationships</span></span>
| <span data-ttu-id="47827-138">Relação</span><span class="sxs-lookup"><span data-stu-id="47827-138">Relationship</span></span> | <span data-ttu-id="47827-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="47827-139">Type</span></span>        | <span data-ttu-id="47827-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="47827-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="47827-141">impressora</span><span class="sxs-lookup"><span data-stu-id="47827-141">printer</span></span>|[<span data-ttu-id="47827-142">impressora</span><span class="sxs-lookup"><span data-stu-id="47827-142">printer</span></span>](printer.md)|<span data-ttu-id="47827-143">A impressora à qual esse compartilhamento de impressora está relacionado.</span><span class="sxs-lookup"><span data-stu-id="47827-143">The printer that this printer share is related to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="47827-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47827-144">JSON representation</span></span>

<span data-ttu-id="47827-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47827-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerShare",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerShare resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->