---
title: tipo de recurso de documento de documentos
description: Representa um documento que está sendo impresso.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 1e7a1d6a9c131417e4f0ef171ac364e5fe8b106b
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863779"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="65378-103">tipo de recurso de documento de documentos</span><span class="sxs-lookup"><span data-stu-id="65378-103">printDocument resource type</span></span>

<span data-ttu-id="65378-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65378-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65378-105">Representa um documento que está sendo impresso.</span><span class="sxs-lookup"><span data-stu-id="65378-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="65378-106">Methods</span><span class="sxs-lookup"><span data-stu-id="65378-106">Methods</span></span>

| <span data-ttu-id="65378-107">Método</span><span class="sxs-lookup"><span data-stu-id="65378-107">Method</span></span>       | <span data-ttu-id="65378-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="65378-108">Return Type</span></span> | <span data-ttu-id="65378-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="65378-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="65378-110">uploadData</span><span class="sxs-lookup"><span data-stu-id="65378-110">uploadData</span></span>](../api/printdocument-uploaddata.md) | <span data-ttu-id="65378-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65378-111">None</span></span> | <span data-ttu-id="65378-112">Carregar um único segmento binário do **documento**.</span><span class="sxs-lookup"><span data-stu-id="65378-112">Upload a single binary segment of the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="65378-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65378-113">Properties</span></span>
| <span data-ttu-id="65378-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65378-114">Property</span></span>     | <span data-ttu-id="65378-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="65378-115">Type</span></span>        | <span data-ttu-id="65378-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="65378-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="65378-117">id</span><span class="sxs-lookup"><span data-stu-id="65378-117">id</span></span>|<span data-ttu-id="65378-118">String</span><span class="sxs-lookup"><span data-stu-id="65378-118">String</span></span>|<span data-ttu-id="65378-119">O identificador do documento.</span><span class="sxs-lookup"><span data-stu-id="65378-119">The document's identifier.</span></span> <span data-ttu-id="65378-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="65378-120">Read-only.</span></span>|
|<span data-ttu-id="65378-121">displayName</span><span class="sxs-lookup"><span data-stu-id="65378-121">displayName</span></span>|<span data-ttu-id="65378-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65378-122">String</span></span>|<span data-ttu-id="65378-123">O nome do documento.</span><span class="sxs-lookup"><span data-stu-id="65378-123">The document's name.</span></span> <span data-ttu-id="65378-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="65378-124">Read-only.</span></span>|
|<span data-ttu-id="65378-125">contentType</span><span class="sxs-lookup"><span data-stu-id="65378-125">contentType</span></span>|<span data-ttu-id="65378-126">String</span><span class="sxs-lookup"><span data-stu-id="65378-126">String</span></span>|<span data-ttu-id="65378-127">O tipo de conteúdo do documento (MIME).</span><span class="sxs-lookup"><span data-stu-id="65378-127">The document's content (MIME) type.</span></span> <span data-ttu-id="65378-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="65378-128">Read-only.</span></span>|
|<span data-ttu-id="65378-129">size</span><span class="sxs-lookup"><span data-stu-id="65378-129">size</span></span>|<span data-ttu-id="65378-130">Int64</span><span class="sxs-lookup"><span data-stu-id="65378-130">Int64</span></span>|<span data-ttu-id="65378-131">O tamanho do documento em bytes.</span><span class="sxs-lookup"><span data-stu-id="65378-131">The document's size in bytes.</span></span> <span data-ttu-id="65378-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="65378-132">Read-only.</span></span>|
|<span data-ttu-id="65378-133">configuration</span><span class="sxs-lookup"><span data-stu-id="65378-133">configuration</span></span>|[<span data-ttu-id="65378-134">printerDocumentConfiguration</span><span class="sxs-lookup"><span data-stu-id="65378-134">printerDocumentConfiguration</span></span>](printerdocumentconfiguration.md) |<span data-ttu-id="65378-135">Um grupo de configurações que uma impressora deve usar para imprimir um documento.</span><span class="sxs-lookup"><span data-stu-id="65378-135">A group of settings that a printer should use to print a document.</span></span> <span data-ttu-id="65378-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="65378-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65378-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65378-137">JSON representation</span></span>

<span data-ttu-id="65378-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65378-138">The following is a JSON representation of the resource.</span></span>

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
