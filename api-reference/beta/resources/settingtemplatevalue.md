---
title: tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9a49dd291bd9cc7baa31d90ba8e247ac984b1906
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965184"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="e6bba-103">tipo de recurso settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="e6bba-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6bba-104">Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.</span><span class="sxs-lookup"><span data-stu-id="e6bba-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="e6bba-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6bba-105">Properties</span></span>
| <span data-ttu-id="e6bba-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6bba-106">Property</span></span>     | <span data-ttu-id="e6bba-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6bba-107">Type</span></span>   |<span data-ttu-id="e6bba-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6bba-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6bba-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="e6bba-109">defaultValue</span></span>|<span data-ttu-id="e6bba-110">string</span><span class="sxs-lookup"><span data-stu-id="e6bba-110">string</span></span>|<span data-ttu-id="e6bba-111">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="e6bba-111">Default value for the setting.</span></span> <span data-ttu-id="e6bba-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6bba-112">Read-only.</span></span>|
|<span data-ttu-id="e6bba-113">description</span><span class="sxs-lookup"><span data-stu-id="e6bba-113">description</span></span>|<span data-ttu-id="e6bba-114">string</span><span class="sxs-lookup"><span data-stu-id="e6bba-114">string</span></span>|<span data-ttu-id="e6bba-115">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="e6bba-115">Description of the setting.</span></span> <span data-ttu-id="e6bba-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6bba-116">Read-only.</span></span>|
|<span data-ttu-id="e6bba-117">name</span><span class="sxs-lookup"><span data-stu-id="e6bba-117">name</span></span>|<span data-ttu-id="e6bba-118">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6bba-118">string</span></span>|<span data-ttu-id="e6bba-119">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="e6bba-119">Name of the setting.</span></span> <span data-ttu-id="e6bba-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6bba-120">Read-only.</span></span>|
|<span data-ttu-id="e6bba-121">type</span><span class="sxs-lookup"><span data-stu-id="e6bba-121">type</span></span>|<span data-ttu-id="e6bba-122">string</span><span class="sxs-lookup"><span data-stu-id="e6bba-122">string</span></span>|<span data-ttu-id="e6bba-123">Tipo da configuração.</span><span class="sxs-lookup"><span data-stu-id="e6bba-123">Type of the setting.</span></span> <span data-ttu-id="e6bba-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6bba-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6bba-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6bba-125">JSON representation</span></span>

<span data-ttu-id="e6bba-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6bba-126">Here is a JSON representation of the resource.</span></span>

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
