---
title: tipo de recurso educationExcelResource
description: 'Uma subclasse de educationResource. Esse tipo de recurso representa um documento do Excel.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: be9ea1d08575ad9dc07ac9fe538a597da8db2803
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334416"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="8c30d-104">tipo de recurso educationExcelResource</span><span class="sxs-lookup"><span data-stu-id="8c30d-104">educationExcelResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c30d-105">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="8c30d-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="8c30d-106">Esse tipo de recurso representa um documento do Excel.</span><span class="sxs-lookup"><span data-stu-id="8c30d-106">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="8c30d-107">**Observação:** O arquivo do Excel deve estar na pasta de recursos associada à atribuição ou ao objeto de envio ao qual este recurso pertence.</span><span class="sxs-lookup"><span data-stu-id="8c30d-107">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="8c30d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c30d-108">Properties</span></span>
| <span data-ttu-id="8c30d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c30d-109">Property</span></span>     | <span data-ttu-id="8c30d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c30d-110">Type</span></span>   |<span data-ttu-id="8c30d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c30d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c30d-112">fileUrl</span><span class="sxs-lookup"><span data-stu-id="8c30d-112">fileUrl</span></span>|<span data-ttu-id="8c30d-113">String</span><span class="sxs-lookup"><span data-stu-id="8c30d-113">String</span></span>|<span data-ttu-id="8c30d-114">Ponteiro para o objeto de arquivo do Excel.</span><span class="sxs-lookup"><span data-stu-id="8c30d-114">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c30d-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c30d-115">JSON representation</span></span>

<span data-ttu-id="8c30d-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c30d-116">The following is a JSON representation of the resource.</span></span>

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
