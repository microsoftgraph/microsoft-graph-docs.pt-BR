---
title: tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: dkershaw10
ms.openlocfilehash: 024007ef05edbb4c3e2e9f8cc901d654734a39ab
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806265"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="5d7cb-103">tipo de recurso settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="5d7cb-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="5d7cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d7cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d7cb-105">Representa uma definição de configuração de modelo individual, incluindo o valor padrão para a configuração, se a configuração não for instanciada.</span><span class="sxs-lookup"><span data-stu-id="5d7cb-105">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="5d7cb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d7cb-106">Properties</span></span>
| <span data-ttu-id="5d7cb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d7cb-107">Property</span></span>     | <span data-ttu-id="5d7cb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d7cb-108">Type</span></span>   |<span data-ttu-id="5d7cb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d7cb-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d7cb-110">defaultValue</span><span class="sxs-lookup"><span data-stu-id="5d7cb-110">defaultValue</span></span>|<span data-ttu-id="5d7cb-111">string</span><span class="sxs-lookup"><span data-stu-id="5d7cb-111">string</span></span>|<span data-ttu-id="5d7cb-112">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="5d7cb-112">Default value for the setting.</span></span> <span data-ttu-id="5d7cb-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5d7cb-113">Read-only.</span></span>|
|<span data-ttu-id="5d7cb-114">description</span><span class="sxs-lookup"><span data-stu-id="5d7cb-114">description</span></span>|<span data-ttu-id="5d7cb-115">string</span><span class="sxs-lookup"><span data-stu-id="5d7cb-115">string</span></span>|<span data-ttu-id="5d7cb-116">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="5d7cb-116">Description of the setting.</span></span> <span data-ttu-id="5d7cb-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5d7cb-117">Read-only.</span></span>|
|<span data-ttu-id="5d7cb-118">name</span><span class="sxs-lookup"><span data-stu-id="5d7cb-118">name</span></span>|<span data-ttu-id="5d7cb-119">string</span><span class="sxs-lookup"><span data-stu-id="5d7cb-119">string</span></span>|<span data-ttu-id="5d7cb-120">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="5d7cb-120">Name of the setting.</span></span> <span data-ttu-id="5d7cb-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5d7cb-121">Read-only.</span></span>|
|<span data-ttu-id="5d7cb-122">type</span><span class="sxs-lookup"><span data-stu-id="5d7cb-122">type</span></span>|<span data-ttu-id="5d7cb-123">string</span><span class="sxs-lookup"><span data-stu-id="5d7cb-123">string</span></span>|<span data-ttu-id="5d7cb-124">Tipo da configuração.</span><span class="sxs-lookup"><span data-stu-id="5d7cb-124">Type of the setting.</span></span> <span data-ttu-id="5d7cb-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5d7cb-125">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5d7cb-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d7cb-126">JSON representation</span></span>

<span data-ttu-id="5d7cb-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5d7cb-127">Here is a JSON representation of the resource.</span></span>

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
