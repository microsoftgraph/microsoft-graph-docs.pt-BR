---
title: tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a2046017dec6439c6db35169de15eb6bb49413b1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806734"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="563e9-103">tipo de recurso settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="563e9-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="563e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="563e9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="563e9-105">Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.</span><span class="sxs-lookup"><span data-stu-id="563e9-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="563e9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="563e9-106">Properties</span></span>

| <span data-ttu-id="563e9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="563e9-107">Property</span></span> | <span data-ttu-id="563e9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="563e9-108">Type</span></span> | <span data-ttu-id="563e9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="563e9-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="563e9-110">defaultValue</span><span class="sxs-lookup"><span data-stu-id="563e9-110">defaultValue</span></span>|<span data-ttu-id="563e9-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="563e9-111">String</span></span>| <span data-ttu-id="563e9-112">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="563e9-112">Default value for the setting.</span></span> |
|<span data-ttu-id="563e9-113">description</span><span class="sxs-lookup"><span data-stu-id="563e9-113">description</span></span>|<span data-ttu-id="563e9-114">String</span><span class="sxs-lookup"><span data-stu-id="563e9-114">String</span></span>| <span data-ttu-id="563e9-115">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="563e9-115">Description of the setting.</span></span> |
|<span data-ttu-id="563e9-116">nome</span><span class="sxs-lookup"><span data-stu-id="563e9-116">name</span></span>|<span data-ttu-id="563e9-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="563e9-117">String</span></span>| <span data-ttu-id="563e9-118">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="563e9-118">Name of the setting.</span></span> |
|<span data-ttu-id="563e9-119">type</span><span class="sxs-lookup"><span data-stu-id="563e9-119">type</span></span>|<span data-ttu-id="563e9-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="563e9-120">String</span></span>| <span data-ttu-id="563e9-121">Tipo da configuração.</span><span class="sxs-lookup"><span data-stu-id="563e9-121">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="563e9-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="563e9-122">JSON representation</span></span>

<span data-ttu-id="563e9-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="563e9-123">Here is a JSON representation of the resource.</span></span>

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
