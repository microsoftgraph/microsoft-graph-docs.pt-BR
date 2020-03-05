---
title: tipo de recurso SettingValue
description: Uma configuração representada por um par de nome/valor.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 673627d726475708c79445f818f23104f0582ef7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520819"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="0ba97-103">tipo de recurso SettingValue</span><span class="sxs-lookup"><span data-stu-id="0ba97-103">settingValue resource type</span></span>

<span data-ttu-id="0ba97-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0ba97-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ba97-105">Uma configuração representada por um par de nome/valor.</span><span class="sxs-lookup"><span data-stu-id="0ba97-105">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="0ba97-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ba97-106">Properties</span></span>
| <span data-ttu-id="0ba97-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ba97-107">Property</span></span>     | <span data-ttu-id="0ba97-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ba97-108">Type</span></span>   |<span data-ttu-id="0ba97-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ba97-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ba97-110">nome</span><span class="sxs-lookup"><span data-stu-id="0ba97-110">name</span></span>|<span data-ttu-id="0ba97-111">string</span><span class="sxs-lookup"><span data-stu-id="0ba97-111">string</span></span>|<span data-ttu-id="0ba97-112">Nome da configuração (conforme definido pelo directorySettingTemplate).</span><span class="sxs-lookup"><span data-stu-id="0ba97-112">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="0ba97-113">value</span><span class="sxs-lookup"><span data-stu-id="0ba97-113">value</span></span>|<span data-ttu-id="0ba97-114">string</span><span class="sxs-lookup"><span data-stu-id="0ba97-114">string</span></span>|<span data-ttu-id="0ba97-115">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="0ba97-115">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ba97-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ba97-116">JSON representation</span></span>

<span data-ttu-id="0ba97-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ba97-117">Here is a JSON representation of the resource.</span></span>

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
