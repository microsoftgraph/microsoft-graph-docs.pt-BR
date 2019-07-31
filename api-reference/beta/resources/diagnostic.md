---
title: tipo de recurso de diagnóstico
description: Informações sobre um erro ou aviso para uma operação do OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4ac591640e647a1caa5230bd8e7e8c64ad2314af
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973138"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="58c92-103">tipo de recurso de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="58c92-103">diagnostic resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58c92-104">Informações sobre um erro ou aviso para uma operação do OneNote.</span><span class="sxs-lookup"><span data-stu-id="58c92-104">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="58c92-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58c92-105">JSON representation</span></span>

<span data-ttu-id="58c92-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="58c92-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="58c92-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58c92-107">Properties</span></span>
| <span data-ttu-id="58c92-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58c92-108">Property</span></span>     | <span data-ttu-id="58c92-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="58c92-109">Type</span></span>   |<span data-ttu-id="58c92-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="58c92-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58c92-111">mensagem</span><span class="sxs-lookup"><span data-stu-id="58c92-111">message</span></span>|<span data-ttu-id="58c92-112">String</span><span class="sxs-lookup"><span data-stu-id="58c92-112">String</span></span>|<span data-ttu-id="58c92-113">A mensagem que descreve a condição que disparou o erro ou aviso.</span><span class="sxs-lookup"><span data-stu-id="58c92-113">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="58c92-114">url</span><span class="sxs-lookup"><span data-stu-id="58c92-114">url</span></span>|<span data-ttu-id="58c92-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58c92-115">String</span></span>|<span data-ttu-id="58c92-116">O link para a documentação para esse problema.</span><span class="sxs-lookup"><span data-stu-id="58c92-116">The link to the documentation for this issue.</span></span>|

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
