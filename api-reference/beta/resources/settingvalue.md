---
title: tipo de recurso SettingValue
description: Uma configuração representada por um par de nome/valor.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: dkershaw10
ms.openlocfilehash: 1710bd136391a8c7d6d38217cb1635407570086f
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806247"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="7fc9c-103">tipo de recurso SettingValue</span><span class="sxs-lookup"><span data-stu-id="7fc9c-103">settingValue resource type</span></span>

<span data-ttu-id="7fc9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fc9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fc9c-105">Uma configuração representada por um par de nome/valor.</span><span class="sxs-lookup"><span data-stu-id="7fc9c-105">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="7fc9c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7fc9c-106">Properties</span></span>
| <span data-ttu-id="7fc9c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7fc9c-107">Property</span></span>     | <span data-ttu-id="7fc9c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7fc9c-108">Type</span></span>   |<span data-ttu-id="7fc9c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fc9c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7fc9c-110">nome</span><span class="sxs-lookup"><span data-stu-id="7fc9c-110">name</span></span>|<span data-ttu-id="7fc9c-111">string</span><span class="sxs-lookup"><span data-stu-id="7fc9c-111">string</span></span>|<span data-ttu-id="7fc9c-112">Nome da configuração (conforme definido pelo directorySettingTemplate).</span><span class="sxs-lookup"><span data-stu-id="7fc9c-112">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="7fc9c-113">value</span><span class="sxs-lookup"><span data-stu-id="7fc9c-113">value</span></span>|<span data-ttu-id="7fc9c-114">string</span><span class="sxs-lookup"><span data-stu-id="7fc9c-114">string</span></span>|<span data-ttu-id="7fc9c-115">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="7fc9c-115">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7fc9c-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7fc9c-116">JSON representation</span></span>

<span data-ttu-id="7fc9c-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7fc9c-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
