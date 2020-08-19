---
title: tipo de recurso SettingValue
description: Uma configuração representada por um par de nome/valor.
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 211609f81bf2ff8123783660b50e1bdd06cb3d56
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808120"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="1bd7b-103">tipo de recurso SettingValue</span><span class="sxs-lookup"><span data-stu-id="1bd7b-103">settingValue resource type</span></span>

<span data-ttu-id="1bd7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bd7b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1bd7b-105">Uma configuração representada por um par de nome/valor.</span><span class="sxs-lookup"><span data-stu-id="1bd7b-105">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="1bd7b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1bd7b-106">Properties</span></span>

| <span data-ttu-id="1bd7b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bd7b-107">Property</span></span> | <span data-ttu-id="1bd7b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bd7b-108">Type</span></span> | <span data-ttu-id="1bd7b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bd7b-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1bd7b-110">nome</span><span class="sxs-lookup"><span data-stu-id="1bd7b-110">name</span></span>|<span data-ttu-id="1bd7b-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bd7b-111">String</span></span>| <span data-ttu-id="1bd7b-112">Nome da configuração (conforme definido pelo [groupSettingTemplate](groupsettingtemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="1bd7b-112">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="1bd7b-113">value</span><span class="sxs-lookup"><span data-stu-id="1bd7b-113">value</span></span>|<span data-ttu-id="1bd7b-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bd7b-114">String</span></span>| <span data-ttu-id="1bd7b-115">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="1bd7b-115">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="1bd7b-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1bd7b-116">JSON representation</span></span>

<span data-ttu-id="1bd7b-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1bd7b-117">Here is a JSON representation of the resource.</span></span>

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
