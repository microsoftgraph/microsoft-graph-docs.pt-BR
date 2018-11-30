---
title: Tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instanciada.
ms.openlocfilehash: 00e424e36338855d8ef603d06c7a9ee52a99c621
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006916"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="aea5b-103">Tipo de recurso settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="aea5b-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="aea5b-104">Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instanciada.</span><span class="sxs-lookup"><span data-stu-id="aea5b-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="aea5b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aea5b-105">Properties</span></span>

| <span data-ttu-id="aea5b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aea5b-106">Property</span></span> | <span data-ttu-id="aea5b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="aea5b-107">Type</span></span> | <span data-ttu-id="aea5b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="aea5b-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="aea5b-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="aea5b-109">defaultValue</span></span>|<span data-ttu-id="aea5b-110">String</span><span class="sxs-lookup"><span data-stu-id="aea5b-110">String</span></span>| <span data-ttu-id="aea5b-111">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="aea5b-111">Default value for the setting.</span></span> |
|<span data-ttu-id="aea5b-112">description</span><span class="sxs-lookup"><span data-stu-id="aea5b-112">description</span></span>|<span data-ttu-id="aea5b-113">String</span><span class="sxs-lookup"><span data-stu-id="aea5b-113">String</span></span>| <span data-ttu-id="aea5b-114">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="aea5b-114">Description of the setting.</span></span> |
|<span data-ttu-id="aea5b-115">nome</span><span class="sxs-lookup"><span data-stu-id="aea5b-115">name</span></span>|<span data-ttu-id="aea5b-116">String</span><span class="sxs-lookup"><span data-stu-id="aea5b-116">String</span></span>| <span data-ttu-id="aea5b-117">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="aea5b-117">Name of the setting.</span></span> |
|<span data-ttu-id="aea5b-118">type</span><span class="sxs-lookup"><span data-stu-id="aea5b-118">type</span></span>|<span data-ttu-id="aea5b-119">String</span><span class="sxs-lookup"><span data-stu-id="aea5b-119">String</span></span>| <span data-ttu-id="aea5b-120">Tipo da configuração.</span><span class="sxs-lookup"><span data-stu-id="aea5b-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="aea5b-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aea5b-121">JSON representation</span></span>

<span data-ttu-id="aea5b-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aea5b-122">Here is a JSON representation of the resource.</span></span>

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