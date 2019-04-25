---
title: tipo de recurso governanceRuleSetting
description: Representa as regras nas quais as configurações de função são compostas.
localization_priority: Normal
ms.openlocfilehash: bbb44760cf4b7377e5e5cc6dd312c2caee9897fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547445"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="e0498-103">tipo de recurso governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="e0498-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0498-104">Representa as regras nas quais as configurações de função são compostas.</span><span class="sxs-lookup"><span data-stu-id="e0498-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="e0498-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e0498-105">Properties</span></span>
|<span data-ttu-id="e0498-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0498-106">Property</span></span>      | <span data-ttu-id="e0498-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0498-107">Type</span></span>         |<span data-ttu-id="e0498-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0498-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="e0498-109">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="e0498-109">ruleIdentifier</span></span>|<span data-ttu-id="e0498-110">String</span><span class="sxs-lookup"><span data-stu-id="e0498-110">String</span></span>        |<span data-ttu-id="e0498-111">A ID da regra.</span><span class="sxs-lookup"><span data-stu-id="e0498-111">The id of the rule.</span></span> <span data-ttu-id="e0498-112">Por exemplo, ``ExpirationRule`` e ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="e0498-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="e0498-113">configuração</span><span class="sxs-lookup"><span data-stu-id="e0498-113">setting</span></span>       |<span data-ttu-id="e0498-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0498-114">String</span></span>        |<span data-ttu-id="e0498-115">As configurações da regra.</span><span class="sxs-lookup"><span data-stu-id="e0498-115">The settings of the rule.</span></span> <span data-ttu-id="e0498-116">O valor é uma cadeia de caracteres JSON com uma lista de pares no formato de Parameter_Name: Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="e0498-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="e0498-117">Por exemplo, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="e0498-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0498-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e0498-118">JSON representation</span></span>

<span data-ttu-id="e0498-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e0498-119">Here is a JSON representation of the resource.</span></span>

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
