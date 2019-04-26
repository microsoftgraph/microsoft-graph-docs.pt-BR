---
title: tipo de recurso expressionInputObject
description: 'Representa um objeto a ser usado como dados de teste de entrada quando a ação [synchronizationSchema: ParseName](../api/synchronization_synchronizationschema_parseexpression.md) executa uma avaliação de expressão.'
localization_priority: Normal
ms.openlocfilehash: 90d394639de7050eaed3b696dd8526e144cac03d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345565"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="5ed3b-103">tipo de recurso expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="5ed3b-103">expressionInputObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ed3b-104">Representa um objeto que será usado como dados de teste de entrada [](../api/synchronization-synchronizationschema-parseexpression.md) quando a ação parsetable executar uma avaliação de expressão.</span><span class="sxs-lookup"><span data-stu-id="5ed3b-104">Represents an object to be used as input test data when the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="5ed3b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ed3b-105">Properties</span></span>
| <span data-ttu-id="5ed3b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ed3b-106">Property</span></span>     | <span data-ttu-id="5ed3b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ed3b-107">Type</span></span>   |<span data-ttu-id="5ed3b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ed3b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ed3b-109">definir</span><span class="sxs-lookup"><span data-stu-id="5ed3b-109">definition</span></span>|[<span data-ttu-id="5ed3b-110">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="5ed3b-110">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="5ed3b-111">Definição do objeto Test.</span><span class="sxs-lookup"><span data-stu-id="5ed3b-111">Definition of the test object.</span></span>|
|<span data-ttu-id="5ed3b-112">properties</span><span class="sxs-lookup"><span data-stu-id="5ed3b-112">properties</span></span>|<span data-ttu-id="5ed3b-113">coleção [stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="5ed3b-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="5ed3b-114">Valores de Propriedade do objeto Test.</span><span class="sxs-lookup"><span data-stu-id="5ed3b-114">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ed3b-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ed3b-115">JSON representation</span></span>

<span data-ttu-id="5ed3b-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ed3b-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
