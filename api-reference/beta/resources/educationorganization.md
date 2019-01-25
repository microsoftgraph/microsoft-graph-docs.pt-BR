---
title: tipo de recurso de educationOrganization
description: 'Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 122717952781cd8effe415fb01b07ec9bf71143d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507471"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="60b41-103">tipo de recurso de educationOrganization</span><span class="sxs-lookup"><span data-stu-id="60b41-103">educationOrganization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60b41-104">Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.</span><span class="sxs-lookup"><span data-stu-id="60b41-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="60b41-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60b41-105">Properties</span></span>
| <span data-ttu-id="60b41-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60b41-106">Property</span></span>     | <span data-ttu-id="60b41-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="60b41-107">Type</span></span>   |<span data-ttu-id="60b41-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="60b41-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60b41-109">description</span><span class="sxs-lookup"><span data-stu-id="60b41-109">description</span></span>|<span data-ttu-id="60b41-110">String</span><span class="sxs-lookup"><span data-stu-id="60b41-110">String</span></span>| <span data-ttu-id="60b41-111">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="60b41-111">Organization description.</span></span>|
|<span data-ttu-id="60b41-112">displayName</span><span class="sxs-lookup"><span data-stu-id="60b41-112">displayName</span></span>|<span data-ttu-id="60b41-113">String</span><span class="sxs-lookup"><span data-stu-id="60b41-113">String</span></span>| <span data-ttu-id="60b41-114">Nome de exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="60b41-114">Organization display name.</span></span>|
|<span data-ttu-id="60b41-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="60b41-115">externalSource</span></span>|<span data-ttu-id="60b41-116">string</span><span class="sxs-lookup"><span data-stu-id="60b41-116">string</span></span>| <span data-ttu-id="60b41-117">Fonte local a partir do qual esta organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="60b41-117">Source where this organization was created from.</span></span> <span data-ttu-id="60b41-118">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="60b41-118">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60b41-119">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="60b41-119">Relationships</span></span>
<span data-ttu-id="60b41-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="60b41-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="60b41-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60b41-121">JSON representation</span></span>

<span data-ttu-id="60b41-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60b41-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationorganization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
