---
title: tipo de recurso de expressionInputObject
description: 'Representa um objeto a ser usado como dados de teste de entrada quando a [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação realiza uma avaliação de expressão.'
localization_priority: Normal
ms.openlocfilehash: 3e631102505408b955404c4badb33b98f314236f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510775"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="30511-103">tipo de recurso de expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="30511-103">expressionInputObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30511-104">Representa um objeto a ser usado como dados de teste de entrada quando a [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação realiza uma avaliação de expressão.</span><span class="sxs-lookup"><span data-stu-id="30511-104">Represents an object to be used as input test data when the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="30511-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="30511-105">Properties</span></span>
| <span data-ttu-id="30511-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30511-106">Property</span></span>     | <span data-ttu-id="30511-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="30511-107">Type</span></span>   |<span data-ttu-id="30511-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="30511-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30511-109">Definição</span><span class="sxs-lookup"><span data-stu-id="30511-109">definition</span></span>|[<span data-ttu-id="30511-110">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="30511-110">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="30511-111">Definição do objeto de teste.</span><span class="sxs-lookup"><span data-stu-id="30511-111">Definition of the test object.</span></span>|
|<span data-ttu-id="30511-112">properties</span><span class="sxs-lookup"><span data-stu-id="30511-112">properties</span></span>|<span data-ttu-id="30511-113">coleção [stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="30511-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="30511-114">Valores de propriedade do objeto de teste.</span><span class="sxs-lookup"><span data-stu-id="30511-114">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30511-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="30511-115">JSON representation</span></span>

<span data-ttu-id="30511-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="30511-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-expressioninputobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
