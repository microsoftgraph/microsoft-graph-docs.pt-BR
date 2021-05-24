---
title: tipo de recurso settingValue
description: Uma configuração representada por um par de nomes/valores.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 171b08d4542af6900dcb6549527e956c4395c947
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547040"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="c6672-103">tipo de recurso settingValue</span><span class="sxs-lookup"><span data-stu-id="c6672-103">settingValue resource type</span></span>

<span data-ttu-id="c6672-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6672-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6672-105">Uma configuração representada por um par de nomes/valores.</span><span class="sxs-lookup"><span data-stu-id="c6672-105">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="c6672-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6672-106">Properties</span></span>

| <span data-ttu-id="c6672-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6672-107">Property</span></span> | <span data-ttu-id="c6672-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6672-108">Type</span></span> | <span data-ttu-id="c6672-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6672-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c6672-110">nome</span><span class="sxs-lookup"><span data-stu-id="c6672-110">name</span></span>|<span data-ttu-id="c6672-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6672-111">String</span></span>| <span data-ttu-id="c6672-112">Nome da configuração (conforme definido pelo [groupSettingTemplate](groupsettingtemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="c6672-112">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="c6672-113">value</span><span class="sxs-lookup"><span data-stu-id="c6672-113">value</span></span>|<span data-ttu-id="c6672-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6672-114">String</span></span>| <span data-ttu-id="c6672-115">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="c6672-115">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="c6672-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6672-116">JSON representation</span></span>

<span data-ttu-id="c6672-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6672-117">Here is a JSON representation of the resource.</span></span>

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

