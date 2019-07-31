---
title: tipo de recurso SettingValue
description: Uma configuração representada por um par de nome/valor.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d8e652501f8cd96e3e820e61b4ad9d353b61f3fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008471"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="2afec-103">tipo de recurso SettingValue</span><span class="sxs-lookup"><span data-stu-id="2afec-103">settingValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2afec-104">Uma configuração representada por um par de nome/valor.</span><span class="sxs-lookup"><span data-stu-id="2afec-104">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="2afec-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2afec-105">Properties</span></span>
| <span data-ttu-id="2afec-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2afec-106">Property</span></span>     | <span data-ttu-id="2afec-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2afec-107">Type</span></span>   |<span data-ttu-id="2afec-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2afec-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2afec-109">name</span><span class="sxs-lookup"><span data-stu-id="2afec-109">name</span></span>|<span data-ttu-id="2afec-110">string</span><span class="sxs-lookup"><span data-stu-id="2afec-110">string</span></span>|<span data-ttu-id="2afec-111">Nome da configuração (conforme definido pelo directorySettingTemplate).</span><span class="sxs-lookup"><span data-stu-id="2afec-111">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="2afec-112">value</span><span class="sxs-lookup"><span data-stu-id="2afec-112">value</span></span>|<span data-ttu-id="2afec-113">string</span><span class="sxs-lookup"><span data-stu-id="2afec-113">string</span></span>|<span data-ttu-id="2afec-114">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="2afec-114">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2afec-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2afec-115">JSON representation</span></span>

<span data-ttu-id="2afec-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2afec-116">Here is a JSON representation of the resource.</span></span>

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
