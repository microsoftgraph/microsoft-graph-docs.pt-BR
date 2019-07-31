---
title: tipo de recurso educationPowerPointResource
description: 'Uma subclasse de educationResource. Este é um recurso do PowerPoint. O arquivo do PowerPoint deve ser carregado no **** diretório fileresource associado ao '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 72ab3435ed30602bbd9b2fadf9a6f4d0879e9198
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972594"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="119f9-105">tipo de recurso educationPowerPointResource</span><span class="sxs-lookup"><span data-stu-id="119f9-105">educationPowerPointResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="119f9-106">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="119f9-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="119f9-107">Este é um recurso do PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="119f9-107">This is a PowerPoint resource.</span></span> <span data-ttu-id="119f9-108">O arquivo do PowerPoint deve ser carregado no \*\*\*\* diretório fileresource associado à atribuição ou ao envio.</span><span class="sxs-lookup"><span data-stu-id="119f9-108">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="119f9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="119f9-109">Properties</span></span>
| <span data-ttu-id="119f9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="119f9-110">Property</span></span>     | <span data-ttu-id="119f9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="119f9-111">Type</span></span>   |<span data-ttu-id="119f9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="119f9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="119f9-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="119f9-113">fileUrl</span></span>|<span data-ttu-id="119f9-114">String</span><span class="sxs-lookup"><span data-stu-id="119f9-114">String</span></span>|<span data-ttu-id="119f9-115">Local do arquivo no disco.</span><span class="sxs-lookup"><span data-stu-id="119f9-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="119f9-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="119f9-116">JSON representation</span></span>

<span data-ttu-id="119f9-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="119f9-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
