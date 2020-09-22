---
title: tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c39762290577c6279a4ecb52bd832ac9c961dbdb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009195"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="b8bb5-103">tipo de recurso settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="b8bb5-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="b8bb5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8bb5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8bb5-105">Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.</span><span class="sxs-lookup"><span data-stu-id="b8bb5-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="b8bb5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8bb5-106">Properties</span></span>

| <span data-ttu-id="b8bb5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8bb5-107">Property</span></span> | <span data-ttu-id="b8bb5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8bb5-108">Type</span></span> | <span data-ttu-id="b8bb5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8bb5-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b8bb5-110">defaultValue</span><span class="sxs-lookup"><span data-stu-id="b8bb5-110">defaultValue</span></span>|<span data-ttu-id="b8bb5-111">String</span><span class="sxs-lookup"><span data-stu-id="b8bb5-111">String</span></span>| <span data-ttu-id="b8bb5-112">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="b8bb5-112">Default value for the setting.</span></span> |
|<span data-ttu-id="b8bb5-113">description</span><span class="sxs-lookup"><span data-stu-id="b8bb5-113">description</span></span>|<span data-ttu-id="b8bb5-114">String</span><span class="sxs-lookup"><span data-stu-id="b8bb5-114">String</span></span>| <span data-ttu-id="b8bb5-115">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="b8bb5-115">Description of the setting.</span></span> |
|<span data-ttu-id="b8bb5-116">nome</span><span class="sxs-lookup"><span data-stu-id="b8bb5-116">name</span></span>|<span data-ttu-id="b8bb5-117">String</span><span class="sxs-lookup"><span data-stu-id="b8bb5-117">String</span></span>| <span data-ttu-id="b8bb5-118">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="b8bb5-118">Name of the setting.</span></span> |
|<span data-ttu-id="b8bb5-119">tipo</span><span class="sxs-lookup"><span data-stu-id="b8bb5-119">type</span></span>|<span data-ttu-id="b8bb5-120">String</span><span class="sxs-lookup"><span data-stu-id="b8bb5-120">String</span></span>| <span data-ttu-id="b8bb5-121">Tipo da configuração.</span><span class="sxs-lookup"><span data-stu-id="b8bb5-121">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="b8bb5-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8bb5-122">JSON representation</span></span>

<span data-ttu-id="b8bb5-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8bb5-123">Here is a JSON representation of the resource.</span></span>

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

