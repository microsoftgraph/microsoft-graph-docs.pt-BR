---
title: tipo de recurso expressionInputObject
description: 'Representa um objeto a ser usado como dados de teste de entrada quando a ação [synchronizationSchema: ParseName](../api/synchronization_synchronizationschema_parseexpression.md) executa uma avaliação de expressão.'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 113c38e540b8c41fb3d3156b27f6f5e1f1df42f2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007946"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="91056-103">tipo de recurso expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="91056-103">expressionInputObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91056-104">Representa um objeto que será usado como dados de teste de entrada [](../api/synchronization-synchronizationschema-parseexpression.md) quando a ação parsetable executar uma avaliação de expressão.</span><span class="sxs-lookup"><span data-stu-id="91056-104">Represents an object to be used as input test data when the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="91056-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91056-105">Properties</span></span>
| <span data-ttu-id="91056-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91056-106">Property</span></span>     | <span data-ttu-id="91056-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="91056-107">Type</span></span>   |<span data-ttu-id="91056-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="91056-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91056-109">definir</span><span class="sxs-lookup"><span data-stu-id="91056-109">definition</span></span>|[<span data-ttu-id="91056-110">ObjectDefinition</span><span class="sxs-lookup"><span data-stu-id="91056-110">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="91056-111">Definição do objeto Test.</span><span class="sxs-lookup"><span data-stu-id="91056-111">Definition of the test object.</span></span>|
|<span data-ttu-id="91056-112">properties</span><span class="sxs-lookup"><span data-stu-id="91056-112">properties</span></span>|<span data-ttu-id="91056-113">coleção [stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="91056-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="91056-114">Valores de Propriedade do objeto Test.</span><span class="sxs-lookup"><span data-stu-id="91056-114">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91056-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91056-115">JSON representation</span></span>

<span data-ttu-id="91056-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91056-116">The following is a JSON representation of the resource.</span></span>

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
