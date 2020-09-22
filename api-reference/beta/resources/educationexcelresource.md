---
title: tipo de recurso educationExcelResource
description: 'Uma subclasse de educationResource. Esse tipo de recurso representa um documento do Excel.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 96fc84227bc7c8e5140ef06ce62ea2d485badab7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095515"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="5ab03-104">tipo de recurso educationExcelResource</span><span class="sxs-lookup"><span data-stu-id="5ab03-104">educationExcelResource resource type</span></span>

<span data-ttu-id="5ab03-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ab03-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ab03-106">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="5ab03-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="5ab03-107">Esse tipo de recurso representa um documento do Excel.</span><span class="sxs-lookup"><span data-stu-id="5ab03-107">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="5ab03-108">**Observação:** O arquivo do Excel deve estar na pasta de recursos associada à atribuição ou ao objeto de envio ao qual este recurso pertence.</span><span class="sxs-lookup"><span data-stu-id="5ab03-108">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="5ab03-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ab03-109">Properties</span></span>
| <span data-ttu-id="5ab03-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ab03-110">Property</span></span>     | <span data-ttu-id="5ab03-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ab03-111">Type</span></span>   |<span data-ttu-id="5ab03-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ab03-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ab03-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="5ab03-113">fileUrl</span></span>|<span data-ttu-id="5ab03-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ab03-114">String</span></span>|<span data-ttu-id="5ab03-115">Ponteiro para o objeto de arquivo do Excel.</span><span class="sxs-lookup"><span data-stu-id="5ab03-115">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ab03-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ab03-116">JSON representation</span></span>

<span data-ttu-id="5ab03-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ab03-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationExcelResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


