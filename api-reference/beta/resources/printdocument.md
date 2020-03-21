---
title: tipo de recurso de documento de documentos
description: Representa um documento que está sendo impresso.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 2a981fbdf7e1126783ae97d93c20e3ec08b1f2f0
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895505"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="67295-103">tipo de recurso de documento de documentos</span><span class="sxs-lookup"><span data-stu-id="67295-103">printDocument resource type</span></span>

<span data-ttu-id="67295-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67295-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67295-105">Representa um documento que está sendo impresso.</span><span class="sxs-lookup"><span data-stu-id="67295-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="67295-106">Methods</span><span class="sxs-lookup"><span data-stu-id="67295-106">Methods</span></span>

| <span data-ttu-id="67295-107">Método</span><span class="sxs-lookup"><span data-stu-id="67295-107">Method</span></span>       | <span data-ttu-id="67295-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="67295-108">Return Type</span></span> | <span data-ttu-id="67295-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="67295-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="67295-110">uploadData</span><span class="sxs-lookup"><span data-stu-id="67295-110">uploadData</span></span>](../api/printdocument-uploaddata.md) | <span data-ttu-id="67295-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="67295-111">None</span></span> | <span data-ttu-id="67295-112">Carregar um único segmento binário do **documento**.</span><span class="sxs-lookup"><span data-stu-id="67295-112">Upload a single binary segment of the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="67295-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67295-113">Properties</span></span>
| <span data-ttu-id="67295-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67295-114">Property</span></span>     | <span data-ttu-id="67295-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="67295-115">Type</span></span>        | <span data-ttu-id="67295-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="67295-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="67295-117">id</span><span class="sxs-lookup"><span data-stu-id="67295-117">id</span></span>|<span data-ttu-id="67295-118">String</span><span class="sxs-lookup"><span data-stu-id="67295-118">String</span></span>|<span data-ttu-id="67295-119">O identificador do documento.</span><span class="sxs-lookup"><span data-stu-id="67295-119">The document's identifier.</span></span> <span data-ttu-id="67295-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67295-120">Read-only.</span></span>|
|<span data-ttu-id="67295-121">name</span><span class="sxs-lookup"><span data-stu-id="67295-121">name</span></span>|<span data-ttu-id="67295-122">String</span><span class="sxs-lookup"><span data-stu-id="67295-122">String</span></span>|<span data-ttu-id="67295-123">O nome do documento.</span><span class="sxs-lookup"><span data-stu-id="67295-123">The document's name.</span></span> <span data-ttu-id="67295-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67295-124">Read-only.</span></span>|
|<span data-ttu-id="67295-125">mimeType</span><span class="sxs-lookup"><span data-stu-id="67295-125">mimeType</span></span>|<span data-ttu-id="67295-126">String</span><span class="sxs-lookup"><span data-stu-id="67295-126">String</span></span>|<span data-ttu-id="67295-127">O tipo MIME do documento.</span><span class="sxs-lookup"><span data-stu-id="67295-127">The document's MIME type.</span></span> <span data-ttu-id="67295-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67295-128">Read-only.</span></span>|
|<span data-ttu-id="67295-129">sizeInBytes</span><span class="sxs-lookup"><span data-stu-id="67295-129">sizeInBytes</span></span>|<span data-ttu-id="67295-130">Int64</span><span class="sxs-lookup"><span data-stu-id="67295-130">Int64</span></span>|<span data-ttu-id="67295-131">O tamanho do documento em bytes.</span><span class="sxs-lookup"><span data-stu-id="67295-131">The document's size in bytes.</span></span> <span data-ttu-id="67295-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67295-132">Read-only.</span></span>|
|<span data-ttu-id="67295-133">documentConfiguration</span><span class="sxs-lookup"><span data-stu-id="67295-133">documentConfiguration</span></span>|[<span data-ttu-id="67295-134">printerDocumentConfiguration</span><span class="sxs-lookup"><span data-stu-id="67295-134">printerDocumentConfiguration</span></span>](printerdocumentconfiguration.md) |<span data-ttu-id="67295-135">Um grupo de configurações que uma impressora deve usar para imprimir um documento.</span><span class="sxs-lookup"><span data-stu-id="67295-135">A group of settings that a printer should use to print a document.</span></span> <span data-ttu-id="67295-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67295-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67295-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67295-137">JSON representation</span></span>

<span data-ttu-id="67295-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67295-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printDocument"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "mimeType": "String",
  "sizeInBytes": 12345,
  "documentConfiguration": {
    "pageRanges": [ {"@odata.type": "microsoft.graph.printPageRange"} ],
    "printQuality": "String",
    "printResolutionInDpi": 123456,
    "feedDirection": "String",
    "orientation": "String",
    "duplexConfiguration": "String",
    "copies": 123456,
    "colorConfiguration": "String",
  }
}

```
