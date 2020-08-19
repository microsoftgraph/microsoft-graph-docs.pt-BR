---
title: tipo de recurso de diagnóstico
description: Informações sobre um erro ou aviso para uma operação do OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: b6cad8680b00b935dbaac817d53d930b5046e265
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809107"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="da3d5-103">tipo de recurso de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="da3d5-103">diagnostic resource type</span></span>

<span data-ttu-id="da3d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da3d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da3d5-105">Informações sobre um erro ou aviso para uma operação do OneNote.</span><span class="sxs-lookup"><span data-stu-id="da3d5-105">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da3d5-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da3d5-106">JSON representation</span></span>

<span data-ttu-id="da3d5-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="da3d5-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="da3d5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da3d5-108">Properties</span></span>
| <span data-ttu-id="da3d5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da3d5-109">Property</span></span>     | <span data-ttu-id="da3d5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="da3d5-110">Type</span></span>   |<span data-ttu-id="da3d5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="da3d5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da3d5-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="da3d5-112">message</span></span>|<span data-ttu-id="da3d5-113">String</span><span class="sxs-lookup"><span data-stu-id="da3d5-113">String</span></span>|<span data-ttu-id="da3d5-114">A mensagem que descreve a condição que disparou o erro ou aviso.</span><span class="sxs-lookup"><span data-stu-id="da3d5-114">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="da3d5-115">url</span><span class="sxs-lookup"><span data-stu-id="da3d5-115">url</span></span>|<span data-ttu-id="da3d5-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da3d5-116">String</span></span>|<span data-ttu-id="da3d5-117">O link para a documentação para esse problema.</span><span class="sxs-lookup"><span data-stu-id="da3d5-117">The link to the documentation for this issue.</span></span>|

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
