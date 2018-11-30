---
title: tipo de recurso de governanceRuleSetting
description: Representa as regras que as configurações de função são compostas de.
ms.openlocfilehash: 486b5163c59772c971cfc1d61a98817b7f0c16f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037342"
---
# <a name="governancerulesetting-resource-type"></a><span data-ttu-id="51f36-103">tipo de recurso de governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="51f36-103">governanceRuleSetting resource type</span></span>

> <span data-ttu-id="51f36-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="51f36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51f36-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="51f36-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51f36-106">Representa as regras que as configurações de função são compostas de.</span><span class="sxs-lookup"><span data-stu-id="51f36-106">Represents the rules that the role settings are composed of.</span></span>


## <a name="properties"></a><span data-ttu-id="51f36-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51f36-107">Properties</span></span>
|<span data-ttu-id="51f36-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51f36-108">Property</span></span>      | <span data-ttu-id="51f36-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="51f36-109">Type</span></span>         |<span data-ttu-id="51f36-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="51f36-110">Description</span></span>|
|:-------------|:-------------|:----------|
|<span data-ttu-id="51f36-111">ruleIdentifier</span><span class="sxs-lookup"><span data-stu-id="51f36-111">ruleIdentifier</span></span>|<span data-ttu-id="51f36-112">String</span><span class="sxs-lookup"><span data-stu-id="51f36-112">String</span></span>        |<span data-ttu-id="51f36-113">A id da regra.</span><span class="sxs-lookup"><span data-stu-id="51f36-113">The id of the rule.</span></span> <span data-ttu-id="51f36-114">Por exemplo, ``ExpirationRule`` e ``MfaRule``.</span><span class="sxs-lookup"><span data-stu-id="51f36-114">For example, ``ExpirationRule`` and ``MfaRule``.</span></span>|
|<span data-ttu-id="51f36-115">configuração</span><span class="sxs-lookup"><span data-stu-id="51f36-115">setting</span></span>       |<span data-ttu-id="51f36-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51f36-116">String</span></span>        |<span data-ttu-id="51f36-117">As configurações da regra.</span><span class="sxs-lookup"><span data-stu-id="51f36-117">The settings of the rule.</span></span> <span data-ttu-id="51f36-118">O valor é uma cadeia de caracteres JSON com uma lista de pares no formato de Parameter_Name:Parameter_Value.</span><span class="sxs-lookup"><span data-stu-id="51f36-118">The value is a JSON string with a list of pairs in the format of Parameter_Name:Parameter_Value.</span></span> <span data-ttu-id="51f36-119">Por exemplo, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span><span class="sxs-lookup"><span data-stu-id="51f36-119">For example, `{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51f36-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51f36-120">JSON representation</span></span>

<span data-ttu-id="51f36-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51f36-121">Here is a JSON representation of the resource.</span></span>

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