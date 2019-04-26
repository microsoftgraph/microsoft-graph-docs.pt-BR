---
title: tipo de recurso SettingValue
description: Uma configuração representada por um par de nome/valor.
localization_priority: Normal
ms.openlocfilehash: dd2cb58c63ff560850bde285a17a06da2399711f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343163"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="fe4d4-103">tipo de recurso SettingValue</span><span class="sxs-lookup"><span data-stu-id="fe4d4-103">settingValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe4d4-104">Uma configuração representada por um par de nome/valor.</span><span class="sxs-lookup"><span data-stu-id="fe4d4-104">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="fe4d4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe4d4-105">Properties</span></span>
| <span data-ttu-id="fe4d4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe4d4-106">Property</span></span>     | <span data-ttu-id="fe4d4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe4d4-107">Type</span></span>   |<span data-ttu-id="fe4d4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe4d4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe4d4-109">name</span><span class="sxs-lookup"><span data-stu-id="fe4d4-109">name</span></span>|<span data-ttu-id="fe4d4-110">string</span><span class="sxs-lookup"><span data-stu-id="fe4d4-110">string</span></span>|<span data-ttu-id="fe4d4-111">Nome da configuração (conforme definido pelo directorySettingTemplate).</span><span class="sxs-lookup"><span data-stu-id="fe4d4-111">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="fe4d4-112">value</span><span class="sxs-lookup"><span data-stu-id="fe4d4-112">value</span></span>|<span data-ttu-id="fe4d4-113">string</span><span class="sxs-lookup"><span data-stu-id="fe4d4-113">string</span></span>|<span data-ttu-id="fe4d4-114">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="fe4d4-114">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe4d4-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe4d4-115">JSON representation</span></span>

<span data-ttu-id="fe4d4-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe4d4-116">Here is a JSON representation of the resource.</span></span>

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
