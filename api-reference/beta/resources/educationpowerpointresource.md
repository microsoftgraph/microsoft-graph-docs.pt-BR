---
title: tipo de recurso de educationPowerPointResource
description: 'Uma subclasse de educationResource. Esse é um recurso do PowerPoint. O arquivo do PowerPoint que deve ser carregado no diretório **fileResource** associado a '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: b61f210ce0efde36b83632268e12d18d3b96b661
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512196"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="43f6a-105">tipo de recurso de educationPowerPointResource</span><span class="sxs-lookup"><span data-stu-id="43f6a-105">educationPowerPointResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43f6a-106">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="43f6a-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="43f6a-107">Esse é um recurso do PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="43f6a-107">This is a PowerPoint resource.</span></span> <span data-ttu-id="43f6a-108">O arquivo do PowerPoint deve ser carregado no diretório **fileResource** associado a atribuição ou o envio.</span><span class="sxs-lookup"><span data-stu-id="43f6a-108">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="43f6a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43f6a-109">Properties</span></span>
| <span data-ttu-id="43f6a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43f6a-110">Property</span></span>     | <span data-ttu-id="43f6a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="43f6a-111">Type</span></span>   |<span data-ttu-id="43f6a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="43f6a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43f6a-113">FileURL</span><span class="sxs-lookup"><span data-stu-id="43f6a-113">fileUrl</span></span>|<span data-ttu-id="43f6a-114">String</span><span class="sxs-lookup"><span data-stu-id="43f6a-114">String</span></span>|<span data-ttu-id="43f6a-115">Local do arquivo no disco.</span><span class="sxs-lookup"><span data-stu-id="43f6a-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43f6a-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43f6a-116">JSON representation</span></span>

<span data-ttu-id="43f6a-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43f6a-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerPointResource"
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
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerpointresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
