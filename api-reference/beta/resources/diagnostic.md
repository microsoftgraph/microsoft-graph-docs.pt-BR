---
title: tipo de recurso de diagnóstico
description: Informações sobre um erro ou aviso para uma operação do OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: e3a28c1078dbd72b3246de31ce98a50a317bcff7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049825"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="92358-103">tipo de recurso de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="92358-103">diagnostic resource type</span></span>

<span data-ttu-id="92358-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92358-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92358-105">Informações sobre um erro ou aviso para uma operação do OneNote.</span><span class="sxs-lookup"><span data-stu-id="92358-105">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="92358-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92358-106">JSON representation</span></span>

<span data-ttu-id="92358-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="92358-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a><span data-ttu-id="92358-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92358-108">Properties</span></span>
| <span data-ttu-id="92358-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92358-109">Property</span></span>     | <span data-ttu-id="92358-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="92358-110">Type</span></span>   |<span data-ttu-id="92358-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="92358-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92358-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="92358-112">message</span></span>|<span data-ttu-id="92358-113">String</span><span class="sxs-lookup"><span data-stu-id="92358-113">String</span></span>|<span data-ttu-id="92358-114">A mensagem que descreve a condição que disparou o erro ou aviso.</span><span class="sxs-lookup"><span data-stu-id="92358-114">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="92358-115">url</span><span class="sxs-lookup"><span data-stu-id="92358-115">url</span></span>|<span data-ttu-id="92358-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92358-116">String</span></span>|<span data-ttu-id="92358-117">O link para a documentação para esse problema.</span><span class="sxs-lookup"><span data-stu-id="92358-117">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


