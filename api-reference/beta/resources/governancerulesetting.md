---
title: Tipo de recurso governanceRuleSetting
description: Representa as regras das que as configurações de função são compostas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: b55ddfea8f46f9d064b4a032a804c2c5f4847d1a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132689"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="22ffb-103">Tipo de recurso governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="22ffb-103">governanceRuleSetting resource type</span></span>

<span data-ttu-id="22ffb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22ffb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22ffb-105">Representa as regras das que as configurações de função são compostas.</span><span class="sxs-lookup"><span data-stu-id="22ffb-105">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="22ffb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22ffb-106">Properties</span></span>
|<span data-ttu-id="22ffb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22ffb-107">Property</span></span>      | <span data-ttu-id="22ffb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="22ffb-108">Type</span></span>         |<span data-ttu-id="22ffb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="22ffb-109">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="22ffb-110">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="22ffb-110">ruleIdentifier</span></span>|<span data-ttu-id="22ffb-111">String</span><span class="sxs-lookup"><span data-stu-id="22ffb-111">String</span></span>        |<span data-ttu-id="22ffb-112">A id da regra.</span><span class="sxs-lookup"><span data-stu-id="22ffb-112">The id of the rule.</span></span> <span data-ttu-id="22ffb-113">Por exemplo, ``ExpirationRule`` e ``MfaRule`` .</span><span class="sxs-lookup"><span data-stu-id="22ffb-113">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="22ffb-114">configuração</span><span class="sxs-lookup"><span data-stu-id="22ffb-114">setting</span></span>       |<span data-ttu-id="22ffb-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22ffb-115">String</span></span>        |<span data-ttu-id="22ffb-116">As configurações da regra.</span><span class="sxs-lookup"><span data-stu-id="22ffb-116">The settings of the rule.</span></span> <span data-ttu-id="22ffb-117">O valor é uma cadeia de caracteres JSON com uma lista de pares no formato Parameter_Name:Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="22ffb-117">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="22ffb-118">Por exemplo, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="22ffb-118">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22ffb-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22ffb-119">JSON representation</span></span>

<span data-ttu-id="22ffb-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22ffb-120">Here is a JSON representation of the resource.</span></span>

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


