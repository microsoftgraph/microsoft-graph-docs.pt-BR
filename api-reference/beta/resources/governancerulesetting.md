---
title: tipo de recurso governanceRuleSetting
description: Representa as regras nas quais as configurações de função são compostas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bfc3bb7895a3ec66a32456b48901fc456d3c3b2e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971863"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="4c860-103">tipo de recurso governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="4c860-103">governanceRuleSetting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c860-104">Representa as regras nas quais as configurações de função são compostas.</span><span class="sxs-lookup"><span data-stu-id="4c860-104">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="4c860-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c860-105">Properties</span></span>
|<span data-ttu-id="4c860-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c860-106">Property</span></span>      | <span data-ttu-id="4c860-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c860-107">Type</span></span>         |<span data-ttu-id="4c860-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c860-108">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="4c860-109">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="4c860-109">ruleIdentifier</span></span>|<span data-ttu-id="4c860-110">String</span><span class="sxs-lookup"><span data-stu-id="4c860-110">String</span></span>        |<span data-ttu-id="4c860-111">A ID da regra.</span><span class="sxs-lookup"><span data-stu-id="4c860-111">The id of the rule.</span></span> <span data-ttu-id="4c860-112">Por exemplo, ``ExpirationRule`` e ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="4c860-112">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="4c860-113">configuração</span><span class="sxs-lookup"><span data-stu-id="4c860-113">setting</span></span>       |<span data-ttu-id="4c860-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c860-114">String</span></span>        |<span data-ttu-id="4c860-115">As configurações da regra.</span><span class="sxs-lookup"><span data-stu-id="4c860-115">The settings of the rule.</span></span> <span data-ttu-id="4c860-116">O valor é uma cadeia de caracteres JSON com uma lista de pares no formato de Parameter_Name: Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="4c860-116">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="4c860-117">Por exemplo, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="4c860-117">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c860-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c860-118">JSON representation</span></span>

<span data-ttu-id="4c860-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c860-119">Here is a JSON representation of the resource.</span></span>

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
