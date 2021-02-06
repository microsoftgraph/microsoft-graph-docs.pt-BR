---
title: Tipo de recurso expressionInputObject
description: Representa um objeto a ser usado como dados de teste de entrada quando a ação synchronizationSchema parseExpression executa uma avaliação de expressão.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 161589d9d8b6e3d06ef6afe31df0fde79bf938bb
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132045"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="1289b-103">Tipo de recurso expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="1289b-103">expressionInputObject resource type</span></span>

<span data-ttu-id="1289b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1289b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1289b-105">Representa um objeto a ser usado como dados de teste de entrada quando a [ação parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) executa uma avaliação de expressão.</span><span class="sxs-lookup"><span data-stu-id="1289b-105">Represents an object to be used as input test data when the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="1289b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1289b-106">Properties</span></span>
| <span data-ttu-id="1289b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1289b-107">Property</span></span>     | <span data-ttu-id="1289b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1289b-108">Type</span></span>   |<span data-ttu-id="1289b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1289b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1289b-110">definição</span><span class="sxs-lookup"><span data-stu-id="1289b-110">definition</span></span>|[<span data-ttu-id="1289b-111">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="1289b-111">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="1289b-112">Definição do objeto de teste.</span><span class="sxs-lookup"><span data-stu-id="1289b-112">Definition of the test object.</span></span>|
|<span data-ttu-id="1289b-113">properties</span><span class="sxs-lookup"><span data-stu-id="1289b-113">properties</span></span>|<span data-ttu-id="1289b-114">[Coleção stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="1289b-114">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="1289b-115">Valores de propriedade do objeto de teste.</span><span class="sxs-lookup"><span data-stu-id="1289b-115">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1289b-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1289b-116">JSON representation</span></span>

<span data-ttu-id="1289b-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1289b-117">The following is a JSON representation of the resource.</span></span>

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


