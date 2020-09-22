---
title: tipo de recurso governanceRuleSetting
description: Representa as regras nas quais as configurações de função são compostas.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: b2a4b70eb7d8af5dde6e3741c3473683ca7e0586
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081633"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="60482-103">tipo de recurso governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="60482-103">governanceRuleSetting resource type</span></span>

<span data-ttu-id="60482-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60482-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60482-105">Representa as regras nas quais as configurações de função são compostas.</span><span class="sxs-lookup"><span data-stu-id="60482-105">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="60482-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60482-106">Properties</span></span>
|<span data-ttu-id="60482-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60482-107">Property</span></span>      | <span data-ttu-id="60482-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="60482-108">Type</span></span>         |<span data-ttu-id="60482-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="60482-109">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="60482-110">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="60482-110">ruleIdentifier</span></span>|<span data-ttu-id="60482-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60482-111">String</span></span>        |<span data-ttu-id="60482-112">A ID da regra.</span><span class="sxs-lookup"><span data-stu-id="60482-112">The id of the rule.</span></span> <span data-ttu-id="60482-113">Por exemplo, ``ExpirationRule`` e ``MfaRule`` .</span><span class="sxs-lookup"><span data-stu-id="60482-113">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="60482-114">configuração</span><span class="sxs-lookup"><span data-stu-id="60482-114">setting</span></span>       |<span data-ttu-id="60482-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60482-115">String</span></span>        |<span data-ttu-id="60482-116">As configurações da regra.</span><span class="sxs-lookup"><span data-stu-id="60482-116">The settings of the rule.</span></span> <span data-ttu-id="60482-117">O valor é uma cadeia de caracteres JSON com uma lista de pares no formato de Parameter_Name: Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="60482-117">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="60482-118">Por exemplo, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="60482-118">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60482-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60482-119">JSON representation</span></span>

<span data-ttu-id="60482-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60482-120">Here is a JSON representation of the resource.</span></span>

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


