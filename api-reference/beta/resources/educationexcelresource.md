---
title: tipo de recurso de educationExcelResource
description: 'Uma subclasse de educationResource. Esse tipo de recurso representa um documento do Excel.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 14d7823f166ca12d202a6561bc9fe7b158ab7476
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522417"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="ef738-104">tipo de recurso de educationExcelResource</span><span class="sxs-lookup"><span data-stu-id="ef738-104">educationExcelResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef738-105">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="ef738-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="ef738-106">Esse tipo de recurso representa um documento do Excel.</span><span class="sxs-lookup"><span data-stu-id="ef738-106">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="ef738-107">**Observação:** O arquivo do Excel deve estar na pasta de recursos associada ao objeto de envio ou atribuição ao qual este recurso pertence.</span><span class="sxs-lookup"><span data-stu-id="ef738-107">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="ef738-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef738-108">Properties</span></span>
| <span data-ttu-id="ef738-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef738-109">Property</span></span>     | <span data-ttu-id="ef738-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef738-110">Type</span></span>   |<span data-ttu-id="ef738-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef738-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef738-112">FileURL</span><span class="sxs-lookup"><span data-stu-id="ef738-112">fileUrl</span></span>|<span data-ttu-id="ef738-113">String</span><span class="sxs-lookup"><span data-stu-id="ef738-113">String</span></span>|<span data-ttu-id="ef738-114">Ponteiro para o objeto de arquivo do Excel.</span><span class="sxs-lookup"><span data-stu-id="ef738-114">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef738-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef738-115">JSON representation</span></span>

<span data-ttu-id="ef738-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef738-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationexcelresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
