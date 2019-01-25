---
title: Tipo de recurso settingValue
description: Uma configuração representada por um par de nome/valor.
localization_priority: Normal
ms.openlocfilehash: aa30fd61c1498be08be4d87175d18015c58323ba
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527735"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="b5f24-103">Tipo de recurso settingValue</span><span class="sxs-lookup"><span data-stu-id="b5f24-103">settingValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5f24-104">Uma configuração representada por um par de nome/valor.</span><span class="sxs-lookup"><span data-stu-id="b5f24-104">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="b5f24-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5f24-105">Properties</span></span>
| <span data-ttu-id="b5f24-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5f24-106">Property</span></span>     | <span data-ttu-id="b5f24-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5f24-107">Type</span></span>   |<span data-ttu-id="b5f24-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5f24-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5f24-109">name</span><span class="sxs-lookup"><span data-stu-id="b5f24-109">name</span></span>|<span data-ttu-id="b5f24-110">string</span><span class="sxs-lookup"><span data-stu-id="b5f24-110">string</span></span>|<span data-ttu-id="b5f24-111">Nome da configuração (conforme definido pelo directorySettingTemplate).</span><span class="sxs-lookup"><span data-stu-id="b5f24-111">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="b5f24-112">valor</span><span class="sxs-lookup"><span data-stu-id="b5f24-112">value</span></span>|<span data-ttu-id="b5f24-113">string</span><span class="sxs-lookup"><span data-stu-id="b5f24-113">string</span></span>|<span data-ttu-id="b5f24-114">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="b5f24-114">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5f24-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5f24-115">JSON representation</span></span>

<span data-ttu-id="b5f24-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b5f24-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/settingvalue.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
