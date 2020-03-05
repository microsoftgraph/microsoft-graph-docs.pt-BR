---
title: tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: cbd53a704e37b6f0cfa15cc875d5de000627b76c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520756"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="333dc-103">tipo de recurso settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="333dc-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="333dc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="333dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="333dc-105">Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.</span><span class="sxs-lookup"><span data-stu-id="333dc-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="333dc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="333dc-106">Properties</span></span>
| <span data-ttu-id="333dc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="333dc-107">Property</span></span>     | <span data-ttu-id="333dc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="333dc-108">Type</span></span>   |<span data-ttu-id="333dc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="333dc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="333dc-110">defaultValue</span><span class="sxs-lookup"><span data-stu-id="333dc-110">defaultValue</span></span>|<span data-ttu-id="333dc-111">string</span><span class="sxs-lookup"><span data-stu-id="333dc-111">string</span></span>|<span data-ttu-id="333dc-112">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="333dc-112">Default value for the setting.</span></span> <span data-ttu-id="333dc-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="333dc-113">Read-only.</span></span>|
|<span data-ttu-id="333dc-114">description</span><span class="sxs-lookup"><span data-stu-id="333dc-114">description</span></span>|<span data-ttu-id="333dc-115">string</span><span class="sxs-lookup"><span data-stu-id="333dc-115">string</span></span>|<span data-ttu-id="333dc-116">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="333dc-116">Description of the setting.</span></span> <span data-ttu-id="333dc-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="333dc-117">Read-only.</span></span>|
|<span data-ttu-id="333dc-118">name</span><span class="sxs-lookup"><span data-stu-id="333dc-118">name</span></span>|<span data-ttu-id="333dc-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="333dc-119">string</span></span>|<span data-ttu-id="333dc-120">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="333dc-120">Name of the setting.</span></span> <span data-ttu-id="333dc-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="333dc-121">Read-only.</span></span>|
|<span data-ttu-id="333dc-122">type</span><span class="sxs-lookup"><span data-stu-id="333dc-122">type</span></span>|<span data-ttu-id="333dc-123">string</span><span class="sxs-lookup"><span data-stu-id="333dc-123">string</span></span>|<span data-ttu-id="333dc-124">Tipo da configuração.</span><span class="sxs-lookup"><span data-stu-id="333dc-124">Type of the setting.</span></span> <span data-ttu-id="333dc-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="333dc-125">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="333dc-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="333dc-126">JSON representation</span></span>

<span data-ttu-id="333dc-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="333dc-127">Here is a JSON representation of the resource.</span></span>

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
