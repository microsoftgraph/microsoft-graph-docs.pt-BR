---
title: tipo de recurso SettingValue
description: Uma configuração representada por um par de nome/valor.
localization_priority: Normal
ms.openlocfilehash: aa30fd61c1498be08be4d87175d18015c58323ba
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584090"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="ca2e9-103">tipo de recurso SettingValue</span><span class="sxs-lookup"><span data-stu-id="ca2e9-103">settingValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca2e9-104">Uma configuração representada por um par de nome/valor.</span><span class="sxs-lookup"><span data-stu-id="ca2e9-104">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="ca2e9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca2e9-105">Properties</span></span>
| <span data-ttu-id="ca2e9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca2e9-106">Property</span></span>     | <span data-ttu-id="ca2e9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca2e9-107">Type</span></span>   |<span data-ttu-id="ca2e9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca2e9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca2e9-109">name</span><span class="sxs-lookup"><span data-stu-id="ca2e9-109">name</span></span>|<span data-ttu-id="ca2e9-110">string</span><span class="sxs-lookup"><span data-stu-id="ca2e9-110">string</span></span>|<span data-ttu-id="ca2e9-111">Nome da configuração (conforme definido pelo directorySettingTemplate).</span><span class="sxs-lookup"><span data-stu-id="ca2e9-111">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="ca2e9-112">value</span><span class="sxs-lookup"><span data-stu-id="ca2e9-112">value</span></span>|<span data-ttu-id="ca2e9-113">string</span><span class="sxs-lookup"><span data-stu-id="ca2e9-113">string</span></span>|<span data-ttu-id="ca2e9-114">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="ca2e9-114">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca2e9-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca2e9-115">JSON representation</span></span>

<span data-ttu-id="ca2e9-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ca2e9-116">Here is a JSON representation of the resource.</span></span>

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
