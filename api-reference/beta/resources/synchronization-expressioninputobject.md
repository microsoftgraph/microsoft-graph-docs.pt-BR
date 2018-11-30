---
title: tipo de recurso de expressionInputObject
description: 'Representa um objeto a ser usado como dados de teste de entrada quando a [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação realiza uma avaliação de expressão.'
ms.openlocfilehash: 06b7344f7e6418db0557f2b12dfa7e964b9d5ab7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039996"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="63eed-103">tipo de recurso de expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="63eed-103">expressionInputObject resource type</span></span>

> <span data-ttu-id="63eed-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="63eed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63eed-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="63eed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="63eed-106">Representa um objeto a ser usado como dados de teste de entrada quando a [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação realiza uma avaliação de expressão.</span><span class="sxs-lookup"><span data-stu-id="63eed-106">Represents an object to be used as input test data when the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="63eed-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63eed-107">Properties</span></span>
| <span data-ttu-id="63eed-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63eed-108">Property</span></span>     | <span data-ttu-id="63eed-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="63eed-109">Type</span></span>   |<span data-ttu-id="63eed-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="63eed-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63eed-111">definição</span><span class="sxs-lookup"><span data-stu-id="63eed-111">definition</span></span>|[<span data-ttu-id="63eed-112">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="63eed-112">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="63eed-113">Definição do objeto de teste.</span><span class="sxs-lookup"><span data-stu-id="63eed-113">Definition of the test object.</span></span>|
|<span data-ttu-id="63eed-114">properties</span><span class="sxs-lookup"><span data-stu-id="63eed-114">properties</span></span>|<span data-ttu-id="63eed-115">coleção [stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="63eed-115">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="63eed-116">Valores de propriedade do objeto de teste.</span><span class="sxs-lookup"><span data-stu-id="63eed-116">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63eed-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63eed-117">JSON representation</span></span>

<span data-ttu-id="63eed-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63eed-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->