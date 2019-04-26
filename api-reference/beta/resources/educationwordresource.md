---
title: tipo de recurso educationWordResource
description: 'Uma subclasse de educationResource. Este é um recurso de documento do Word. O arquivo do Word deve ser carregado no **** diretório fileresource associado ao '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9bd9af22c141991efd85fc240a002b5c7a0eac3b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340190"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="589ac-105">tipo de recurso educationWordResource</span><span class="sxs-lookup"><span data-stu-id="589ac-105">educationWordResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="589ac-106">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="589ac-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="589ac-107">Este é um recurso de documento do Word.</span><span class="sxs-lookup"><span data-stu-id="589ac-107">This is a Word document resource.</span></span> <span data-ttu-id="589ac-108">O arquivo do Word deve ser carregado no \*\*\*\* diretório fileresource associado à atribuição ou ao envio.</span><span class="sxs-lookup"><span data-stu-id="589ac-108">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="589ac-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="589ac-109">Properties</span></span>
| <span data-ttu-id="589ac-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="589ac-110">Property</span></span>     | <span data-ttu-id="589ac-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="589ac-111">Type</span></span>   |<span data-ttu-id="589ac-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="589ac-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="589ac-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="589ac-113">fileUrl</span></span>|<span data-ttu-id="589ac-114">String</span><span class="sxs-lookup"><span data-stu-id="589ac-114">String</span></span>|<span data-ttu-id="589ac-115">Local do arquivo no disco.</span><span class="sxs-lookup"><span data-stu-id="589ac-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="589ac-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="589ac-116">JSON representation</span></span>

<span data-ttu-id="589ac-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="589ac-117">The following is a JSON representation of the resource.</span></span>

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
