---
title: tipo de recurso de governanceRuleSetting
description: Representa as regras que as configurações de função são compostas de.
localization_priority: Normal
ms.openlocfilehash: 7554c96daec70a95cde5ab0c3faedfba74764cff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894254"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="65452-103">tipo de recurso de governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="65452-103">governanceRuleSetting resource type</span></span>

> <span data-ttu-id="65452-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="65452-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65452-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="65452-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65452-106">Representa as regras que as configurações de função são compostas de.</span><span class="sxs-lookup"><span data-stu-id="65452-106">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="65452-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65452-107">Properties</span></span>
|<span data-ttu-id="65452-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65452-108">Property</span></span>      | <span data-ttu-id="65452-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="65452-109">Type</span></span>         |<span data-ttu-id="65452-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="65452-110">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="65452-111">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="65452-111">ruleIdentifier</span></span>|<span data-ttu-id="65452-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65452-112">String</span></span>        |<span data-ttu-id="65452-113">A id da regra.</span><span class="sxs-lookup"><span data-stu-id="65452-113">The id of the rule.</span></span> <span data-ttu-id="65452-114">Por exemplo, ``ExpirationRule`` e ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="65452-114">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="65452-115">configuração</span><span class="sxs-lookup"><span data-stu-id="65452-115">setting</span></span>       |<span data-ttu-id="65452-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65452-116">String</span></span>        |<span data-ttu-id="65452-117">As configurações da regra.</span><span class="sxs-lookup"><span data-stu-id="65452-117">The settings of the rule.</span></span> <span data-ttu-id="65452-118">O valor é uma cadeia de caracteres JSON com uma lista de pares no formato de Parameter_Name:Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="65452-118">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="65452-119">Por exemplo, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="65452-119">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65452-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65452-120">JSON representation</span></span>

<span data-ttu-id="65452-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65452-121">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
