---
title: tipo de recurso expressionInputObject
description: Representa um objeto a ser usado como dados de teste de entrada quando a ação synchronizationSchema ParseName executa uma avaliação de expressão.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9727f50b05eb8cdb5319883dd0058a91d9383cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968350"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="b7474-103">tipo de recurso expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="b7474-103">expressionInputObject resource type</span></span>

<span data-ttu-id="b7474-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7474-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7474-105">Representa um objeto que será usado como dados de teste de entrada quando a ação [parsetable](../api/synchronization-synchronizationschema-parseexpression.md) executar uma avaliação de expressão.</span><span class="sxs-lookup"><span data-stu-id="b7474-105">Represents an object to be used as input test data when the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="b7474-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7474-106">Properties</span></span>
| <span data-ttu-id="b7474-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7474-107">Property</span></span>     | <span data-ttu-id="b7474-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7474-108">Type</span></span>   |<span data-ttu-id="b7474-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7474-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7474-110">definir</span><span class="sxs-lookup"><span data-stu-id="b7474-110">definition</span></span>|[<span data-ttu-id="b7474-111">ObjectDefinition</span><span class="sxs-lookup"><span data-stu-id="b7474-111">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="b7474-112">Definição do objeto Test.</span><span class="sxs-lookup"><span data-stu-id="b7474-112">Definition of the test object.</span></span>|
|<span data-ttu-id="b7474-113">properties</span><span class="sxs-lookup"><span data-stu-id="b7474-113">properties</span></span>|<span data-ttu-id="b7474-114">coleção [stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b7474-114">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="b7474-115">Valores de Propriedade do objeto Test.</span><span class="sxs-lookup"><span data-stu-id="b7474-115">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7474-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7474-116">JSON representation</span></span>

<span data-ttu-id="b7474-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7474-117">The following is a JSON representation of the resource.</span></span>

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


