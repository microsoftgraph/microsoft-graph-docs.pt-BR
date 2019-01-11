---
title: Tipo de recurso settingTemplateValue
description: Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instanciada.
localization_priority: Normal
ms.openlocfilehash: e941630ab72363db1c4be40079cf2af9e40ff002
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811862"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="a73c6-103">Tipo de recurso settingTemplateValue</span><span class="sxs-lookup"><span data-stu-id="a73c6-103">settingTemplateValue resource type</span></span>

> <span data-ttu-id="a73c6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a73c6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a73c6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a73c6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a73c6-106">Representa uma definição de configuração de modelo individual, incluindo o valor padrão da configuração, se a configuração não for instanciada.</span><span class="sxs-lookup"><span data-stu-id="a73c6-106">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="a73c6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a73c6-107">Properties</span></span>
| <span data-ttu-id="a73c6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a73c6-108">Property</span></span>     | <span data-ttu-id="a73c6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a73c6-109">Type</span></span>   |<span data-ttu-id="a73c6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a73c6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a73c6-111">defaultValue</span><span class="sxs-lookup"><span data-stu-id="a73c6-111">defaultValue</span></span>|<span data-ttu-id="a73c6-112">string</span><span class="sxs-lookup"><span data-stu-id="a73c6-112">string</span></span>|<span data-ttu-id="a73c6-113">Valor padrão para a configuração.</span><span class="sxs-lookup"><span data-stu-id="a73c6-113">Default value for the setting.</span></span> <span data-ttu-id="a73c6-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a73c6-114">Read-only.</span></span>|
|<span data-ttu-id="a73c6-115">description</span><span class="sxs-lookup"><span data-stu-id="a73c6-115">description</span></span>|<span data-ttu-id="a73c6-116">string</span><span class="sxs-lookup"><span data-stu-id="a73c6-116">string</span></span>|<span data-ttu-id="a73c6-117">Descrição da configuração.</span><span class="sxs-lookup"><span data-stu-id="a73c6-117">Description of the setting.</span></span> <span data-ttu-id="a73c6-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a73c6-118">Read-only.</span></span>|
|<span data-ttu-id="a73c6-119">name</span><span class="sxs-lookup"><span data-stu-id="a73c6-119">name</span></span>|<span data-ttu-id="a73c6-120">string</span><span class="sxs-lookup"><span data-stu-id="a73c6-120">string</span></span>|<span data-ttu-id="a73c6-121">Nome da configuração.</span><span class="sxs-lookup"><span data-stu-id="a73c6-121">Name of the setting.</span></span> <span data-ttu-id="a73c6-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a73c6-122">Read-only.</span></span>|
|<span data-ttu-id="a73c6-123">type</span><span class="sxs-lookup"><span data-stu-id="a73c6-123">type</span></span>|<span data-ttu-id="a73c6-124">string</span><span class="sxs-lookup"><span data-stu-id="a73c6-124">string</span></span>|<span data-ttu-id="a73c6-125">Tipo da configuração.</span><span class="sxs-lookup"><span data-stu-id="a73c6-125">Type of the setting.</span></span> <span data-ttu-id="a73c6-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a73c6-126">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a73c6-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a73c6-127">JSON representation</span></span>

<span data-ttu-id="a73c6-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a73c6-128">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
