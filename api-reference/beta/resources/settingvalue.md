---
title: Tipo de recurso settingValue
description: Uma configuração representada por um par nome/valor.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: dkershaw10
ms.openlocfilehash: d1be40f6ad2046895c1a14f3395185662ae0ff62
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133375"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="727e7-103">Tipo de recurso settingValue</span><span class="sxs-lookup"><span data-stu-id="727e7-103">settingValue resource type</span></span>

<span data-ttu-id="727e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="727e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="727e7-105">Uma configuração representada por um par nome/valor.</span><span class="sxs-lookup"><span data-stu-id="727e7-105">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="727e7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="727e7-106">Properties</span></span>
| <span data-ttu-id="727e7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="727e7-107">Property</span></span>     | <span data-ttu-id="727e7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="727e7-108">Type</span></span>   |<span data-ttu-id="727e7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="727e7-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="727e7-110">nome</span><span class="sxs-lookup"><span data-stu-id="727e7-110">name</span></span>|<span data-ttu-id="727e7-111">string</span><span class="sxs-lookup"><span data-stu-id="727e7-111">string</span></span>|<span data-ttu-id="727e7-112">Nome da configuração (conforme definido pelo directorySettingTemplate).</span><span class="sxs-lookup"><span data-stu-id="727e7-112">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="727e7-113">value</span><span class="sxs-lookup"><span data-stu-id="727e7-113">value</span></span>|<span data-ttu-id="727e7-114">string</span><span class="sxs-lookup"><span data-stu-id="727e7-114">string</span></span>|<span data-ttu-id="727e7-115">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="727e7-115">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="727e7-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="727e7-116">JSON representation</span></span>

<span data-ttu-id="727e7-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="727e7-117">Here is a JSON representation of the resource.</span></span>

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


