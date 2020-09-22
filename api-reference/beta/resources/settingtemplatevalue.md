---
title: tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: dkershaw10
ms.openlocfilehash: b0f9db75d870cc775b22011674e6a460e11d8812
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033528"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="1e910-103">tipo de recurso settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="1e910-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="1e910-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e910-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e910-105">Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.</span><span class="sxs-lookup"><span data-stu-id="1e910-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="1e910-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e910-106">Properties</span></span>
| <span data-ttu-id="1e910-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e910-107">Property</span></span>     | <span data-ttu-id="1e910-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e910-108">Type</span></span>   |<span data-ttu-id="1e910-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e910-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e910-110">defaultValue</span><span class="sxs-lookup"><span data-stu-id="1e910-110">defaultValue</span></span>|<span data-ttu-id="1e910-111">string</span><span class="sxs-lookup"><span data-stu-id="1e910-111">string</span></span>|<span data-ttu-id="1e910-112">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="1e910-112">Default value for the setting.</span></span> <span data-ttu-id="1e910-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e910-113">Read-only.</span></span>|
|<span data-ttu-id="1e910-114">description</span><span class="sxs-lookup"><span data-stu-id="1e910-114">description</span></span>|<span data-ttu-id="1e910-115">string</span><span class="sxs-lookup"><span data-stu-id="1e910-115">string</span></span>|<span data-ttu-id="1e910-116">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="1e910-116">Description of the setting.</span></span> <span data-ttu-id="1e910-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e910-117">Read-only.</span></span>|
|<span data-ttu-id="1e910-118">name</span><span class="sxs-lookup"><span data-stu-id="1e910-118">name</span></span>|<span data-ttu-id="1e910-119">string</span><span class="sxs-lookup"><span data-stu-id="1e910-119">string</span></span>|<span data-ttu-id="1e910-120">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="1e910-120">Name of the setting.</span></span> <span data-ttu-id="1e910-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e910-121">Read-only.</span></span>|
|<span data-ttu-id="1e910-122">type</span><span class="sxs-lookup"><span data-stu-id="1e910-122">type</span></span>|<span data-ttu-id="1e910-123">string</span><span class="sxs-lookup"><span data-stu-id="1e910-123">string</span></span>|<span data-ttu-id="1e910-124">Tipo da configuração.</span><span class="sxs-lookup"><span data-stu-id="1e910-124">Type of the setting.</span></span> <span data-ttu-id="1e910-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e910-125">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e910-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e910-126">JSON representation</span></span>

<span data-ttu-id="1e910-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e910-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "string",
  "description": "string",
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


