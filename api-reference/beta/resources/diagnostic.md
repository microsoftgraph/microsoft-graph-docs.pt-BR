---
title: tipo de recurso de diagnóstico
description: Informações sobre um erro ou aviso para uma operação do OneNote.
localization_priority: Normal
ms.openlocfilehash: ef495374f84e0df887198b38a5c8488987a59343
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535211"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="7a8f1-103">tipo de recurso de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="7a8f1-103">diagnostic resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a8f1-104">Informações sobre um erro ou aviso para uma operação do OneNote.</span><span class="sxs-lookup"><span data-stu-id="7a8f1-104">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a8f1-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a8f1-105">JSON representation</span></span>

<span data-ttu-id="7a8f1-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7a8f1-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="7a8f1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a8f1-107">Properties</span></span>
| <span data-ttu-id="7a8f1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a8f1-108">Property</span></span>     | <span data-ttu-id="7a8f1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a8f1-109">Type</span></span>   |<span data-ttu-id="7a8f1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a8f1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a8f1-111">mensagem</span><span class="sxs-lookup"><span data-stu-id="7a8f1-111">message</span></span>|<span data-ttu-id="7a8f1-112">String</span><span class="sxs-lookup"><span data-stu-id="7a8f1-112">String</span></span>|<span data-ttu-id="7a8f1-113">A mensagem que descreve a condição que disparou o erro ou aviso.</span><span class="sxs-lookup"><span data-stu-id="7a8f1-113">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="7a8f1-114">url</span><span class="sxs-lookup"><span data-stu-id="7a8f1-114">url</span></span>|<span data-ttu-id="7a8f1-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a8f1-115">String</span></span>|<span data-ttu-id="7a8f1-116">O link para a documentação para esse problema.</span><span class="sxs-lookup"><span data-stu-id="7a8f1-116">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/diagnostic.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
