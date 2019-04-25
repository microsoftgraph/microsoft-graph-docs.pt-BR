---
title: tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.
localization_priority: Normal
ms.openlocfilehash: 80b640419eb2084888dcd6887ece54b4fd4bdf3c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583673"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="3f096-103">tipo de recurso settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="3f096-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f096-104">Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.</span><span class="sxs-lookup"><span data-stu-id="3f096-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="3f096-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f096-105">Properties</span></span>
| <span data-ttu-id="3f096-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f096-106">Property</span></span>     | <span data-ttu-id="3f096-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f096-107">Type</span></span>   |<span data-ttu-id="3f096-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f096-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f096-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="3f096-109">defaultValue</span></span>|<span data-ttu-id="3f096-110">string</span><span class="sxs-lookup"><span data-stu-id="3f096-110">string</span></span>|<span data-ttu-id="3f096-111">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="3f096-111">Default value for the setting.</span></span> <span data-ttu-id="3f096-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3f096-112">Read-only.</span></span>|
|<span data-ttu-id="3f096-113">description</span><span class="sxs-lookup"><span data-stu-id="3f096-113">description</span></span>|<span data-ttu-id="3f096-114">string</span><span class="sxs-lookup"><span data-stu-id="3f096-114">string</span></span>|<span data-ttu-id="3f096-115">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="3f096-115">Description of the setting.</span></span> <span data-ttu-id="3f096-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3f096-116">Read-only.</span></span>|
|<span data-ttu-id="3f096-117">name</span><span class="sxs-lookup"><span data-stu-id="3f096-117">name</span></span>|<span data-ttu-id="3f096-118">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f096-118">string</span></span>|<span data-ttu-id="3f096-119">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="3f096-119">Name of the setting.</span></span> <span data-ttu-id="3f096-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3f096-120">Read-only.</span></span>|
|<span data-ttu-id="3f096-121">type</span><span class="sxs-lookup"><span data-stu-id="3f096-121">type</span></span>|<span data-ttu-id="3f096-122">string</span><span class="sxs-lookup"><span data-stu-id="3f096-122">string</span></span>|<span data-ttu-id="3f096-123">Tipo da configuração.</span><span class="sxs-lookup"><span data-stu-id="3f096-123">Type of the setting.</span></span> <span data-ttu-id="3f096-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3f096-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f096-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f096-125">JSON representation</span></span>

<span data-ttu-id="3f096-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f096-126">Here is a JSON representation of the resource.</span></span>

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
