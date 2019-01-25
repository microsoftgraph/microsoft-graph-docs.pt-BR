---
title: tipo de recurso de governanceRuleSetting
description: Representa as regras que as configurações de função são compostas de.
localization_priority: Normal
ms.openlocfilehash: bbb44760cf4b7377e5e5cc6dd312c2caee9897fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522235"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="7f595-103">tipo de recurso de governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="7f595-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f595-104">Representa as regras que as configurações de função são compostas de.</span><span class="sxs-lookup"><span data-stu-id="7f595-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="7f595-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f595-105">Properties</span></span>
|<span data-ttu-id="7f595-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f595-106">Property</span></span>      | <span data-ttu-id="7f595-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f595-107">Type</span></span>         |<span data-ttu-id="7f595-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f595-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="7f595-109">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="7f595-109">ruleIdentifier</span></span>|<span data-ttu-id="7f595-110">String</span><span class="sxs-lookup"><span data-stu-id="7f595-110">String</span></span>        |<span data-ttu-id="7f595-111">A id da regra.</span><span class="sxs-lookup"><span data-stu-id="7f595-111">The id of the rule.</span></span> <span data-ttu-id="7f595-112">Por exemplo, ``ExpirationRule`` e ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="7f595-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="7f595-113">configuração</span><span class="sxs-lookup"><span data-stu-id="7f595-113">setting</span></span>       |<span data-ttu-id="7f595-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f595-114">String</span></span>        |<span data-ttu-id="7f595-115">As configurações da regra.</span><span class="sxs-lookup"><span data-stu-id="7f595-115">The settings of the rule.</span></span> <span data-ttu-id="7f595-116">O valor é uma cadeia de caracteres JSON com uma lista de pares no formato de Parameter_Name:Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="7f595-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="7f595-117">Por exemplo, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="7f595-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f595-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f595-118">JSON representation</span></span>

<span data-ttu-id="7f595-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f595-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRuleSetting"
}-->


```json
{
  "ruleIdentifier": "String",
  "setting": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerulesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
