---
title: tipo de recurso educationWordResource
description: 'Uma subclasse de educationResource. Este é um recurso de documento do Word. O arquivo do Word deve ser carregado no **** diretório fileresource associado ao '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0bd326ea45130da7e7eadb7eb1d21ae3a6c31cce
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972282"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="46e3e-105">tipo de recurso educationWordResource</span><span class="sxs-lookup"><span data-stu-id="46e3e-105">educationWordResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46e3e-106">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="46e3e-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="46e3e-107">Este é um recurso de documento do Word.</span><span class="sxs-lookup"><span data-stu-id="46e3e-107">This is a Word document resource.</span></span> <span data-ttu-id="46e3e-108">O arquivo do Word deve ser carregado no \*\*\*\* diretório fileresource associado à atribuição ou ao envio.</span><span class="sxs-lookup"><span data-stu-id="46e3e-108">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="46e3e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46e3e-109">Properties</span></span>
| <span data-ttu-id="46e3e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46e3e-110">Property</span></span>     | <span data-ttu-id="46e3e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="46e3e-111">Type</span></span>   |<span data-ttu-id="46e3e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="46e3e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46e3e-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="46e3e-113">fileUrl</span></span>|<span data-ttu-id="46e3e-114">String</span><span class="sxs-lookup"><span data-stu-id="46e3e-114">String</span></span>|<span data-ttu-id="46e3e-115">Local do arquivo no disco.</span><span class="sxs-lookup"><span data-stu-id="46e3e-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46e3e-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46e3e-116">JSON representation</span></span>

<span data-ttu-id="46e3e-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46e3e-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
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
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
