---
title: configuraçãoSplateValue tipo de recurso
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instantânea.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e53a8f07f325b023deea32e01fe217feeb35f49d
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547047"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="0f56a-103">configuraçãoSplateValue tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="0f56a-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="0f56a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f56a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f56a-105">Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instantânea.</span><span class="sxs-lookup"><span data-stu-id="0f56a-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="0f56a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f56a-106">Properties</span></span>

| <span data-ttu-id="0f56a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f56a-107">Property</span></span> | <span data-ttu-id="0f56a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f56a-108">Type</span></span> | <span data-ttu-id="0f56a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f56a-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0f56a-110">defaultValue</span><span class="sxs-lookup"><span data-stu-id="0f56a-110">defaultValue</span></span>|<span data-ttu-id="0f56a-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f56a-111">String</span></span>| <span data-ttu-id="0f56a-112">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="0f56a-112">Default value for the setting.</span></span> |
|<span data-ttu-id="0f56a-113">descrição</span><span class="sxs-lookup"><span data-stu-id="0f56a-113">description</span></span>|<span data-ttu-id="0f56a-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f56a-114">String</span></span>| <span data-ttu-id="0f56a-115">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="0f56a-115">Description of the setting.</span></span> |
|<span data-ttu-id="0f56a-116">nome</span><span class="sxs-lookup"><span data-stu-id="0f56a-116">name</span></span>|<span data-ttu-id="0f56a-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f56a-117">String</span></span>| <span data-ttu-id="0f56a-118">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="0f56a-118">Name of the setting.</span></span> |
|<span data-ttu-id="0f56a-119">tipo</span><span class="sxs-lookup"><span data-stu-id="0f56a-119">type</span></span>|<span data-ttu-id="0f56a-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f56a-120">String</span></span>| <span data-ttu-id="0f56a-121">Tipo de configuração.</span><span class="sxs-lookup"><span data-stu-id="0f56a-121">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="0f56a-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f56a-122">JSON representation</span></span>

<span data-ttu-id="0f56a-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f56a-123">Here is a JSON representation of the resource.</span></span>

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

