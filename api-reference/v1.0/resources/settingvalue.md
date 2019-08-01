---
title: tipo de recurso SettingValue
description: Uma configuração representada por um par de nome/valor.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f37a429fd9bb8e8d3cf65aef55d6af5033f4a598
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034353"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="8afc3-103">tipo de recurso SettingValue</span><span class="sxs-lookup"><span data-stu-id="8afc3-103">settingValue resource type</span></span>

<span data-ttu-id="8afc3-104">Uma configuração representada por um par de nome/valor.</span><span class="sxs-lookup"><span data-stu-id="8afc3-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="8afc3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8afc3-105">Properties</span></span>

| <span data-ttu-id="8afc3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8afc3-106">Property</span></span> | <span data-ttu-id="8afc3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8afc3-107">Type</span></span> | <span data-ttu-id="8afc3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8afc3-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8afc3-109">name</span><span class="sxs-lookup"><span data-stu-id="8afc3-109">name</span></span>|<span data-ttu-id="8afc3-110">String</span><span class="sxs-lookup"><span data-stu-id="8afc3-110">String</span></span>| <span data-ttu-id="8afc3-111">Nome da configuração (conforme definido pelo [groupSettingTemplate](groupsettingtemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="8afc3-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="8afc3-112">value</span><span class="sxs-lookup"><span data-stu-id="8afc3-112">value</span></span>|<span data-ttu-id="8afc3-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8afc3-113">String</span></span>| <span data-ttu-id="8afc3-114">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="8afc3-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="8afc3-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8afc3-115">JSON representation</span></span>

<span data-ttu-id="8afc3-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8afc3-116">Here is a JSON representation of the resource.</span></span>

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
