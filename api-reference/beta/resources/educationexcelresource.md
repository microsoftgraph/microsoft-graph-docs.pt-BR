---
title: tipo de recurso educationExcelResource
description: 'Uma subclasse de educationResource. Esse tipo de recurso representa um documento do Excel.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b533d5072ab9a4e880b14b64e96f4791db399e09
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502162"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="8227b-104">tipo de recurso educationExcelResource</span><span class="sxs-lookup"><span data-stu-id="8227b-104">educationExcelResource resource type</span></span>

<span data-ttu-id="8227b-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8227b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8227b-106">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="8227b-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="8227b-107">Esse tipo de recurso representa um documento do Excel.</span><span class="sxs-lookup"><span data-stu-id="8227b-107">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="8227b-108">**Observação:** O arquivo do Excel deve estar na pasta de recursos associada à atribuição ou ao objeto de envio ao qual este recurso pertence.</span><span class="sxs-lookup"><span data-stu-id="8227b-108">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="8227b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8227b-109">Properties</span></span>
| <span data-ttu-id="8227b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8227b-110">Property</span></span>     | <span data-ttu-id="8227b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8227b-111">Type</span></span>   |<span data-ttu-id="8227b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8227b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8227b-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="8227b-113">fileUrl</span></span>|<span data-ttu-id="8227b-114">String</span><span class="sxs-lookup"><span data-stu-id="8227b-114">String</span></span>|<span data-ttu-id="8227b-115">Ponteiro para o objeto de arquivo do Excel.</span><span class="sxs-lookup"><span data-stu-id="8227b-115">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8227b-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8227b-116">JSON representation</span></span>

<span data-ttu-id="8227b-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8227b-117">The following is a JSON representation of the resource.</span></span>

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
