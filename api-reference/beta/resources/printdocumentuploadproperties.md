---
author: nilakhan
description: Representa informações para upload de documentos de impressão
title: tipo de recurso printDocumentUploadProperties
localization_priority: Normal
doc_type: resourcePageType
ms.prod: universal-print
ms.openlocfilehash: 1249eaae4d62cffe14935587c655ba402237b0ed
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727966"
---
# <a name="printdocumentuploadproperties-resource-type"></a><span data-ttu-id="722a6-103">tipo de recurso printDocumentUploadProperties</span><span class="sxs-lookup"><span data-stu-id="722a6-103">printDocumentUploadProperties resource type</span></span>

<span data-ttu-id="722a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="722a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="722a6-105">Descreve o documento que está sendo carregado</span><span class="sxs-lookup"><span data-stu-id="722a6-105">Describes the document that is being uploaded</span></span>

## <a name="json-representation"></a><span data-ttu-id="722a6-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="722a6-106">JSON representation</span></span>

<span data-ttu-id="722a6-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="722a6-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.printDocumentUploadProperties",
  "baseType": null
}-->

```json
{
  "contentType": "String",
  "documentName": "String",
  "size": "Int64",
}
```

## <a name="properties"></a><span data-ttu-id="722a6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="722a6-108">Properties</span></span>


| <span data-ttu-id="722a6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="722a6-109">Property</span></span>       | <span data-ttu-id="722a6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="722a6-110">Type</span></span>              |<span data-ttu-id="722a6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="722a6-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="722a6-112">contentType</span><span class="sxs-lookup"><span data-stu-id="722a6-112">contentType</span></span> | <span data-ttu-id="722a6-113">String</span><span class="sxs-lookup"><span data-stu-id="722a6-113">String</span></span>    | <span data-ttu-id="722a6-114">O tipo de conteúdo do documento (MIME).</span><span class="sxs-lookup"><span data-stu-id="722a6-114">The document's content (MIME) type.</span></span>
| <span data-ttu-id="722a6-115">documentName</span><span class="sxs-lookup"><span data-stu-id="722a6-115">documentName</span></span> | <span data-ttu-id="722a6-116">String</span><span class="sxs-lookup"><span data-stu-id="722a6-116">String</span></span> | <span data-ttu-id="722a6-117">O nome do documento.</span><span class="sxs-lookup"><span data-stu-id="722a6-117">The document's name.</span></span>
| <span data-ttu-id="722a6-118">size</span><span class="sxs-lookup"><span data-stu-id="722a6-118">size</span></span>          | <span data-ttu-id="722a6-119">Int64</span><span class="sxs-lookup"><span data-stu-id="722a6-119">Int64</span></span>            | <span data-ttu-id="722a6-120">O tamanho do documento em bytes.</span><span class="sxs-lookup"><span data-stu-id="722a6-120">The document's size in bytes.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "printDocumentUploadProperties",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
