---
title: tipo de recurso SettingValue
description: Uma configuração representada por um par de nome/valor.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ba9b6321ad443d9538d9c539435c62f50149b330
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446888"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="c27d5-103">tipo de recurso SettingValue</span><span class="sxs-lookup"><span data-stu-id="c27d5-103">settingValue resource type</span></span>

<span data-ttu-id="c27d5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c27d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c27d5-105">Uma configuração representada por um par de nome/valor.</span><span class="sxs-lookup"><span data-stu-id="c27d5-105">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="c27d5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c27d5-106">Properties</span></span>

| <span data-ttu-id="c27d5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c27d5-107">Property</span></span> | <span data-ttu-id="c27d5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c27d5-108">Type</span></span> | <span data-ttu-id="c27d5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c27d5-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c27d5-110">nome</span><span class="sxs-lookup"><span data-stu-id="c27d5-110">name</span></span>|<span data-ttu-id="c27d5-111">String</span><span class="sxs-lookup"><span data-stu-id="c27d5-111">String</span></span>| <span data-ttu-id="c27d5-112">Nome da configuração (conforme definido pelo [groupSettingTemplate](groupsettingtemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="c27d5-112">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="c27d5-113">value</span><span class="sxs-lookup"><span data-stu-id="c27d5-113">value</span></span>|<span data-ttu-id="c27d5-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c27d5-114">String</span></span>| <span data-ttu-id="c27d5-115">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="c27d5-115">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="c27d5-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c27d5-116">JSON representation</span></span>

<span data-ttu-id="c27d5-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c27d5-117">Here is a JSON representation of the resource.</span></span>

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
