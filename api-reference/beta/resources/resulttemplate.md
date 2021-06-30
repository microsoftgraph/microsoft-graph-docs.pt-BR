---
title: Tipo de recurso resultTemplate
description: Um dicionário de resultTemplateIds e valores associados, que incluem o nome e o esquema JSON dos modelos de resultado.
localization_priority: Normal
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 402b60efc278e72102d9bba4eb89be2dda38916b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211202"
---
# <a name="resulttemplate-resource-type"></a><span data-ttu-id="c494d-103">Tipo de recurso resultTemplate</span><span class="sxs-lookup"><span data-stu-id="c494d-103">resultTemplate resource type</span></span>

<span data-ttu-id="c494d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c494d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c494d-105">Um dicionário de **resultTemplateIds** e valores associados, que inclui o nome e o esquema JSON dos modelos de resultado.</span><span class="sxs-lookup"><span data-stu-id="c494d-105">A dictionary of **resultTemplateIds** and associated values, which includes the name and JSON schema of the result templates.</span></span>

## <a name="properties"></a><span data-ttu-id="c494d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c494d-106">Properties</span></span>

| <span data-ttu-id="c494d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c494d-107">Property</span></span>     | <span data-ttu-id="c494d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c494d-108">Type</span></span>        | <span data-ttu-id="c494d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c494d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c494d-110">key</span><span class="sxs-lookup"><span data-stu-id="c494d-110">key</span></span>|<span data-ttu-id="c494d-111">String</span><span class="sxs-lookup"><span data-stu-id="c494d-111">String</span></span>|<span data-ttu-id="c494d-112">ID de um modelo de resultado.</span><span class="sxs-lookup"><span data-stu-id="c494d-112">ID of a result template.</span></span> <span data-ttu-id="c494d-113">Ele deve mapear para **um resultTemplateId** no [searchHit](searchhit.md).</span><span class="sxs-lookup"><span data-stu-id="c494d-113">It must map to a **resultTemplateId** in the [searchHit](searchhit.md).</span></span>|
|<span data-ttu-id="c494d-114">displayName</span><span class="sxs-lookup"><span data-stu-id="c494d-114">displayName</span></span>|<span data-ttu-id="c494d-115">String</span><span class="sxs-lookup"><span data-stu-id="c494d-115">String</span></span>|<span data-ttu-id="c494d-116">Nome do modelo de resultado.</span><span class="sxs-lookup"><span data-stu-id="c494d-116">Name of the result template.</span></span>|
|<span data-ttu-id="c494d-117">corpo</span><span class="sxs-lookup"><span data-stu-id="c494d-117">body</span></span>|<span data-ttu-id="c494d-118">Json</span><span class="sxs-lookup"><span data-stu-id="c494d-118">Json</span></span>|<span data-ttu-id="c494d-119">Esquema JSON do modelo de resultado.</span><span class="sxs-lookup"><span data-stu-id="c494d-119">JSON schema of the result template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c494d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c494d-120">JSON representation</span></span>

<span data-ttu-id="c494d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c494d-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultTemplate",
  "baseType": null
}-->


```json
{
  "resultTemplateId": {
                    "displayName": "String",
                    "body": "Json schema"
                }
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resultTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


