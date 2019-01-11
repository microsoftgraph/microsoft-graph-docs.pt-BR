---
title: Tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instanciada.
localization_priority: Normal
ms.openlocfilehash: 0cb3376177e3a4efcae54a591a083914db6b56d7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828319"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="1eeea-103">Tipo de recurso settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="1eeea-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="1eeea-104">Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instanciada.</span><span class="sxs-lookup"><span data-stu-id="1eeea-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="1eeea-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1eeea-105">Properties</span></span>

| <span data-ttu-id="1eeea-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1eeea-106">Property</span></span> | <span data-ttu-id="1eeea-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1eeea-107">Type</span></span> | <span data-ttu-id="1eeea-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1eeea-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1eeea-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="1eeea-109">defaultValue</span></span>|<span data-ttu-id="1eeea-110">String</span><span class="sxs-lookup"><span data-stu-id="1eeea-110">String</span></span>| <span data-ttu-id="1eeea-111">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="1eeea-111">Default value for the setting.</span></span> |
|<span data-ttu-id="1eeea-112">description</span><span class="sxs-lookup"><span data-stu-id="1eeea-112">description</span></span>|<span data-ttu-id="1eeea-113">String</span><span class="sxs-lookup"><span data-stu-id="1eeea-113">String</span></span>| <span data-ttu-id="1eeea-114">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="1eeea-114">Description of the setting.</span></span> |
|<span data-ttu-id="1eeea-115">nome</span><span class="sxs-lookup"><span data-stu-id="1eeea-115">name</span></span>|<span data-ttu-id="1eeea-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1eeea-116">String</span></span>| <span data-ttu-id="1eeea-117">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="1eeea-117">Name of the setting.</span></span> |
|<span data-ttu-id="1eeea-118">type</span><span class="sxs-lookup"><span data-stu-id="1eeea-118">type</span></span>|<span data-ttu-id="1eeea-119">String</span><span class="sxs-lookup"><span data-stu-id="1eeea-119">String</span></span>| <span data-ttu-id="1eeea-120">Tipo da configuração.</span><span class="sxs-lookup"><span data-stu-id="1eeea-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="1eeea-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1eeea-121">JSON representation</span></span>

<span data-ttu-id="1eeea-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1eeea-122">Here is a JSON representation of the resource.</span></span>

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
