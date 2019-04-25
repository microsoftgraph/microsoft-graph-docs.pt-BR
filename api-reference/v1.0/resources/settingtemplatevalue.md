---
title: tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.
localization_priority: Normal
ms.openlocfilehash: 0cb3376177e3a4efcae54a591a083914db6b56d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549689"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="51f13-103">tipo de recurso settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="51f13-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="51f13-104">Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.</span><span class="sxs-lookup"><span data-stu-id="51f13-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="51f13-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51f13-105">Properties</span></span>

| <span data-ttu-id="51f13-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51f13-106">Property</span></span> | <span data-ttu-id="51f13-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="51f13-107">Type</span></span> | <span data-ttu-id="51f13-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="51f13-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="51f13-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="51f13-109">defaultValue</span></span>|<span data-ttu-id="51f13-110">String</span><span class="sxs-lookup"><span data-stu-id="51f13-110">String</span></span>| <span data-ttu-id="51f13-111">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="51f13-111">Default value for the setting.</span></span> |
|<span data-ttu-id="51f13-112">description</span><span class="sxs-lookup"><span data-stu-id="51f13-112">description</span></span>|<span data-ttu-id="51f13-113">String</span><span class="sxs-lookup"><span data-stu-id="51f13-113">String</span></span>| <span data-ttu-id="51f13-114">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="51f13-114">Description of the setting.</span></span> |
|<span data-ttu-id="51f13-115">name</span><span class="sxs-lookup"><span data-stu-id="51f13-115">name</span></span>|<span data-ttu-id="51f13-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51f13-116">String</span></span>| <span data-ttu-id="51f13-117">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="51f13-117">Name of the setting.</span></span> |
|<span data-ttu-id="51f13-118">type</span><span class="sxs-lookup"><span data-stu-id="51f13-118">type</span></span>|<span data-ttu-id="51f13-119">String</span><span class="sxs-lookup"><span data-stu-id="51f13-119">String</span></span>| <span data-ttu-id="51f13-120">Tipo da configuração.</span><span class="sxs-lookup"><span data-stu-id="51f13-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="51f13-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51f13-121">JSON representation</span></span>

<span data-ttu-id="51f13-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51f13-122">Here is a JSON representation of the resource.</span></span>

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
