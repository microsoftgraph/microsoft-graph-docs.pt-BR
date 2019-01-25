---
title: Tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instanciada.
localization_priority: Normal
ms.openlocfilehash: 80b640419eb2084888dcd6887ece54b4fd4bdf3c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528008"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="eca40-103">Tipo de recurso settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="eca40-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eca40-104">Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instanciada.</span><span class="sxs-lookup"><span data-stu-id="eca40-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="eca40-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eca40-105">Properties</span></span>
| <span data-ttu-id="eca40-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eca40-106">Property</span></span>     | <span data-ttu-id="eca40-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="eca40-107">Type</span></span>   |<span data-ttu-id="eca40-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="eca40-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eca40-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="eca40-109">defaultValue</span></span>|<span data-ttu-id="eca40-110">string</span><span class="sxs-lookup"><span data-stu-id="eca40-110">string</span></span>|<span data-ttu-id="eca40-111">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="eca40-111">Default value for the setting.</span></span> <span data-ttu-id="eca40-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eca40-112">Read-only.</span></span>|
|<span data-ttu-id="eca40-113">description</span><span class="sxs-lookup"><span data-stu-id="eca40-113">description</span></span>|<span data-ttu-id="eca40-114">string</span><span class="sxs-lookup"><span data-stu-id="eca40-114">string</span></span>|<span data-ttu-id="eca40-115">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="eca40-115">Description of the setting.</span></span> <span data-ttu-id="eca40-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eca40-116">Read-only.</span></span>|
|<span data-ttu-id="eca40-117">name</span><span class="sxs-lookup"><span data-stu-id="eca40-117">name</span></span>|<span data-ttu-id="eca40-118">string</span><span class="sxs-lookup"><span data-stu-id="eca40-118">string</span></span>|<span data-ttu-id="eca40-119">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="eca40-119">Name of the setting.</span></span> <span data-ttu-id="eca40-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eca40-120">Read-only.</span></span>|
|<span data-ttu-id="eca40-121">type</span><span class="sxs-lookup"><span data-stu-id="eca40-121">type</span></span>|<span data-ttu-id="eca40-122">string</span><span class="sxs-lookup"><span data-stu-id="eca40-122">string</span></span>|<span data-ttu-id="eca40-123">Tipo da configuração.</span><span class="sxs-lookup"><span data-stu-id="eca40-123">Type of the setting.</span></span> <span data-ttu-id="eca40-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eca40-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eca40-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eca40-125">JSON representation</span></span>

<span data-ttu-id="eca40-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eca40-126">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/settingtemplatevalue.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
