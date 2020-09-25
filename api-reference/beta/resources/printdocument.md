---
title: tipo de recurso de documento de documentos
description: Representa um documento que está sendo impresso.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bfe1badffdd675c68678e1f8463d09aee2af1217
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273680"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="50fa3-103">tipo de recurso de documento de documentos</span><span class="sxs-lookup"><span data-stu-id="50fa3-103">printDocument resource type</span></span>

<span data-ttu-id="50fa3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50fa3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50fa3-105">Representa um documento que está sendo impresso.</span><span class="sxs-lookup"><span data-stu-id="50fa3-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="50fa3-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="50fa3-106">Methods</span></span>

| <span data-ttu-id="50fa3-107">Método</span><span class="sxs-lookup"><span data-stu-id="50fa3-107">Method</span></span>       | <span data-ttu-id="50fa3-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="50fa3-108">Return Type</span></span> | <span data-ttu-id="50fa3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="50fa3-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="50fa3-110">uploadData</span><span class="sxs-lookup"><span data-stu-id="50fa3-110">uploadData</span></span>](../api/printdocument-uploaddata.md) | <span data-ttu-id="50fa3-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50fa3-111">None</span></span> | <span data-ttu-id="50fa3-112">Carregar um único segmento binário do **documento**.</span><span class="sxs-lookup"><span data-stu-id="50fa3-112">Upload a single binary segment of the **printDocument**.</span></span> |
| [<span data-ttu-id="50fa3-113">Baixar arquivo binário</span><span class="sxs-lookup"><span data-stu-id="50fa3-113">Download binary file</span></span>](../api/printdocument-get-file.md) | <span data-ttu-id="50fa3-114">URL de download</span><span class="sxs-lookup"><span data-stu-id="50fa3-114">Download Url</span></span> | <span data-ttu-id="50fa3-115">Baixe o arquivo binário associado ao **documento**.</span><span class="sxs-lookup"><span data-stu-id="50fa3-115">Download the binary file associated with the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="50fa3-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50fa3-116">Properties</span></span>
| <span data-ttu-id="50fa3-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50fa3-117">Property</span></span>     | <span data-ttu-id="50fa3-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="50fa3-118">Type</span></span>        | <span data-ttu-id="50fa3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="50fa3-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="50fa3-120">id</span><span class="sxs-lookup"><span data-stu-id="50fa3-120">id</span></span>|<span data-ttu-id="50fa3-121">String</span><span class="sxs-lookup"><span data-stu-id="50fa3-121">String</span></span>|<span data-ttu-id="50fa3-122">O identificador do documento.</span><span class="sxs-lookup"><span data-stu-id="50fa3-122">The document's identifier.</span></span> <span data-ttu-id="50fa3-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50fa3-123">Read-only.</span></span>|
|<span data-ttu-id="50fa3-124">displayName</span><span class="sxs-lookup"><span data-stu-id="50fa3-124">displayName</span></span>|<span data-ttu-id="50fa3-125">String</span><span class="sxs-lookup"><span data-stu-id="50fa3-125">String</span></span>|<span data-ttu-id="50fa3-126">O nome do documento.</span><span class="sxs-lookup"><span data-stu-id="50fa3-126">The document's name.</span></span> <span data-ttu-id="50fa3-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50fa3-127">Read-only.</span></span>|
|<span data-ttu-id="50fa3-128">contentType</span><span class="sxs-lookup"><span data-stu-id="50fa3-128">contentType</span></span>|<span data-ttu-id="50fa3-129">String</span><span class="sxs-lookup"><span data-stu-id="50fa3-129">String</span></span>|<span data-ttu-id="50fa3-130">O tipo de conteúdo do documento (MIME).</span><span class="sxs-lookup"><span data-stu-id="50fa3-130">The document's content (MIME) type.</span></span> <span data-ttu-id="50fa3-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50fa3-131">Read-only.</span></span>|
|<span data-ttu-id="50fa3-132">size</span><span class="sxs-lookup"><span data-stu-id="50fa3-132">size</span></span>|<span data-ttu-id="50fa3-133">Int64</span><span class="sxs-lookup"><span data-stu-id="50fa3-133">Int64</span></span>|<span data-ttu-id="50fa3-134">O tamanho do documento em bytes.</span><span class="sxs-lookup"><span data-stu-id="50fa3-134">The document's size in bytes.</span></span> <span data-ttu-id="50fa3-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50fa3-135">Read-only.</span></span>|
|<span data-ttu-id="50fa3-136">configuration</span><span class="sxs-lookup"><span data-stu-id="50fa3-136">configuration</span></span>|[<span data-ttu-id="50fa3-137">printerDocumentConfiguration</span><span class="sxs-lookup"><span data-stu-id="50fa3-137">printerDocumentConfiguration</span></span>](printerdocumentconfiguration.md) |<span data-ttu-id="50fa3-138">Um grupo de configurações que uma impressora deve usar para imprimir um documento.</span><span class="sxs-lookup"><span data-stu-id="50fa3-138">A group of settings that a printer should use to print a document.</span></span> <span data-ttu-id="50fa3-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50fa3-139">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50fa3-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50fa3-140">JSON representation</span></span>

<span data-ttu-id="50fa3-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50fa3-141">The following is a JSON representation of the resource.</span></span>

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


