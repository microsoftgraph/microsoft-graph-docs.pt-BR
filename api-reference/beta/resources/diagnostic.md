---
title: tipo de recurso de diagnóstico
description: Informações sobre um erro ou aviso para uma operação do OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f0d5e6a938c454ca2efeda0dd7628c15269d6311
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507237"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="6ecfc-103">tipo de recurso de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="6ecfc-103">diagnostic resource type</span></span>

<span data-ttu-id="6ecfc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6ecfc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ecfc-105">Informações sobre um erro ou aviso para uma operação do OneNote.</span><span class="sxs-lookup"><span data-stu-id="6ecfc-105">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ecfc-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ecfc-106">JSON representation</span></span>

<span data-ttu-id="6ecfc-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6ecfc-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="6ecfc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ecfc-108">Properties</span></span>
| <span data-ttu-id="6ecfc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ecfc-109">Property</span></span>     | <span data-ttu-id="6ecfc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ecfc-110">Type</span></span>   |<span data-ttu-id="6ecfc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ecfc-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ecfc-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="6ecfc-112">message</span></span>|<span data-ttu-id="6ecfc-113">String</span><span class="sxs-lookup"><span data-stu-id="6ecfc-113">String</span></span>|<span data-ttu-id="6ecfc-114">A mensagem que descreve a condição que disparou o erro ou aviso.</span><span class="sxs-lookup"><span data-stu-id="6ecfc-114">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="6ecfc-115">url</span><span class="sxs-lookup"><span data-stu-id="6ecfc-115">url</span></span>|<span data-ttu-id="6ecfc-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ecfc-116">String</span></span>|<span data-ttu-id="6ecfc-117">O link para a documentação para esse problema.</span><span class="sxs-lookup"><span data-stu-id="6ecfc-117">The link to the documentation for this issue.</span></span>|

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
