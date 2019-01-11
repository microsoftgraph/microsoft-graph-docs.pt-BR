---
title: tipo de recurso de expressionInputObject
description: 'Representa um objeto a ser usado como dados de teste de entrada quando a [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação realiza uma avaliação de expressão.'
localization_priority: Normal
ms.openlocfilehash: acf0fa5125d863224de6df76d46109b9888f8ddf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820108"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="aeefd-103">tipo de recurso de expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="aeefd-103">expressionInputObject resource type</span></span>

> <span data-ttu-id="aeefd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="aeefd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aeefd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aeefd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aeefd-106">Representa um objeto a ser usado como dados de teste de entrada quando a [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação realiza uma avaliação de expressão.</span><span class="sxs-lookup"><span data-stu-id="aeefd-106">Represents an object to be used as input test data when the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="aeefd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aeefd-107">Properties</span></span>
| <span data-ttu-id="aeefd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aeefd-108">Property</span></span>     | <span data-ttu-id="aeefd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="aeefd-109">Type</span></span>   |<span data-ttu-id="aeefd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="aeefd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aeefd-111">definição</span><span class="sxs-lookup"><span data-stu-id="aeefd-111">definition</span></span>|[<span data-ttu-id="aeefd-112">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="aeefd-112">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="aeefd-113">Definição do objeto de teste.</span><span class="sxs-lookup"><span data-stu-id="aeefd-113">Definition of the test object.</span></span>|
|<span data-ttu-id="aeefd-114">properties</span><span class="sxs-lookup"><span data-stu-id="aeefd-114">properties</span></span>|<span data-ttu-id="aeefd-115">coleção [stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="aeefd-115">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="aeefd-116">Valores de propriedade do objeto de teste.</span><span class="sxs-lookup"><span data-stu-id="aeefd-116">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aeefd-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aeefd-117">JSON representation</span></span>

<span data-ttu-id="aeefd-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aeefd-118">The following is a JSON representation of the resource.</span></span>

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
