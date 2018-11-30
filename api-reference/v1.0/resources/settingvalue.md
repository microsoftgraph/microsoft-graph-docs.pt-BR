---
title: Tipo de recurso settingValue
description: Uma configuração representada por um par de nome/valor.
ms.openlocfilehash: b47c5c746117390cfd59db71d832928e482403b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007509"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="37f0a-103">Tipo de recurso settingValue</span><span class="sxs-lookup"><span data-stu-id="37f0a-103">settingValue resource type</span></span>

<span data-ttu-id="37f0a-104">Uma configuração representada por um par de nome/valor.</span><span class="sxs-lookup"><span data-stu-id="37f0a-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="37f0a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37f0a-105">Properties</span></span>

| <span data-ttu-id="37f0a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37f0a-106">Property</span></span> | <span data-ttu-id="37f0a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="37f0a-107">Type</span></span> | <span data-ttu-id="37f0a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="37f0a-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="37f0a-109">name</span><span class="sxs-lookup"><span data-stu-id="37f0a-109">name</span></span>|<span data-ttu-id="37f0a-110">String</span><span class="sxs-lookup"><span data-stu-id="37f0a-110">String</span></span>| <span data-ttu-id="37f0a-111">Nome da configuração (como definido pelo [groupSettingTemplate](groupsettingtemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="37f0a-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="37f0a-112">valor</span><span class="sxs-lookup"><span data-stu-id="37f0a-112">value</span></span>|<span data-ttu-id="37f0a-113">String</span><span class="sxs-lookup"><span data-stu-id="37f0a-113">String</span></span>| <span data-ttu-id="37f0a-114">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="37f0a-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="37f0a-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37f0a-115">JSON representation</span></span>

<span data-ttu-id="37f0a-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37f0a-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->