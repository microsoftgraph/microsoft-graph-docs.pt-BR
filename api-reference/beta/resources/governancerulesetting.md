---
title: tipo de recurso governanceRuleSetting
description: Representa as regras nas quais as configurações de função são compostas.
localization_priority: Normal
ms.openlocfilehash: 433fc0d3ab3a524b86bbf1fc46dbe5185549473b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333714"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="e686d-103">tipo de recurso governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="e686d-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e686d-104">Representa as regras nas quais as configurações de função são compostas.</span><span class="sxs-lookup"><span data-stu-id="e686d-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="e686d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e686d-105">Properties</span></span>
|<span data-ttu-id="e686d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e686d-106">Property</span></span>      | <span data-ttu-id="e686d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e686d-107">Type</span></span>         |<span data-ttu-id="e686d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e686d-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="e686d-109">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="e686d-109">ruleIdentifier</span></span>|<span data-ttu-id="e686d-110">String</span><span class="sxs-lookup"><span data-stu-id="e686d-110">String</span></span>        |<span data-ttu-id="e686d-111">A ID da regra.</span><span class="sxs-lookup"><span data-stu-id="e686d-111">The id of the rule.</span></span> <span data-ttu-id="e686d-112">Por exemplo, ``ExpirationRule`` e ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="e686d-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="e686d-113">configuração</span><span class="sxs-lookup"><span data-stu-id="e686d-113">setting</span></span>       |<span data-ttu-id="e686d-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e686d-114">String</span></span>        |<span data-ttu-id="e686d-115">As configurações da regra.</span><span class="sxs-lookup"><span data-stu-id="e686d-115">The settings of the rule.</span></span> <span data-ttu-id="e686d-116">O valor é uma cadeia de caracteres JSON com uma lista de pares no formato de Parameter_Name: Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="e686d-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="e686d-117">Por exemplo, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="e686d-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e686d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e686d-118">JSON representation</span></span>

<span data-ttu-id="e686d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e686d-119">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
