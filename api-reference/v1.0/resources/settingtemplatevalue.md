---
title: tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f4ac39001e260d7f65b3a593d90976f94acd4693
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034388"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="e5931-103">tipo de recurso settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="e5931-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="e5931-104">Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.</span><span class="sxs-lookup"><span data-stu-id="e5931-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="e5931-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5931-105">Properties</span></span>

| <span data-ttu-id="e5931-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5931-106">Property</span></span> | <span data-ttu-id="e5931-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5931-107">Type</span></span> | <span data-ttu-id="e5931-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5931-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e5931-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="e5931-109">defaultValue</span></span>|<span data-ttu-id="e5931-110">String</span><span class="sxs-lookup"><span data-stu-id="e5931-110">String</span></span>| <span data-ttu-id="e5931-111">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="e5931-111">Default value for the setting.</span></span> |
|<span data-ttu-id="e5931-112">descrição</span><span class="sxs-lookup"><span data-stu-id="e5931-112">description</span></span>|<span data-ttu-id="e5931-113">String</span><span class="sxs-lookup"><span data-stu-id="e5931-113">String</span></span>| <span data-ttu-id="e5931-114">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="e5931-114">Description of the setting.</span></span> |
|<span data-ttu-id="e5931-115">name</span><span class="sxs-lookup"><span data-stu-id="e5931-115">name</span></span>|<span data-ttu-id="e5931-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5931-116">String</span></span>| <span data-ttu-id="e5931-117">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="e5931-117">Name of the setting.</span></span> |
|<span data-ttu-id="e5931-118">type</span><span class="sxs-lookup"><span data-stu-id="e5931-118">type</span></span>|<span data-ttu-id="e5931-119">String</span><span class="sxs-lookup"><span data-stu-id="e5931-119">String</span></span>| <span data-ttu-id="e5931-120">Tipo da configuração.</span><span class="sxs-lookup"><span data-stu-id="e5931-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="e5931-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5931-121">JSON representation</span></span>

<span data-ttu-id="e5931-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5931-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
