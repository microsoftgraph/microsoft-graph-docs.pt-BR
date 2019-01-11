---
title: Tipo de recurso settingValue
description: Uma configuração representada por um par de nome/valor.
localization_priority: Normal
ms.openlocfilehash: 0ddd6388e14ea3deff99e927541694a97c594195
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815523"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="f127d-103">Tipo de recurso settingValue</span><span class="sxs-lookup"><span data-stu-id="f127d-103">settingValue resource type</span></span>

> <span data-ttu-id="f127d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f127d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f127d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f127d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f127d-106">Uma configuração representada por um par de nome/valor.</span><span class="sxs-lookup"><span data-stu-id="f127d-106">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="f127d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f127d-107">Properties</span></span>
| <span data-ttu-id="f127d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f127d-108">Property</span></span>     | <span data-ttu-id="f127d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f127d-109">Type</span></span>   |<span data-ttu-id="f127d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f127d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f127d-111">name</span><span class="sxs-lookup"><span data-stu-id="f127d-111">name</span></span>|<span data-ttu-id="f127d-112">string</span><span class="sxs-lookup"><span data-stu-id="f127d-112">string</span></span>|<span data-ttu-id="f127d-113">Nome da configuração (conforme definido pelo directorySettingTemplate).</span><span class="sxs-lookup"><span data-stu-id="f127d-113">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="f127d-114">valor</span><span class="sxs-lookup"><span data-stu-id="f127d-114">value</span></span>|<span data-ttu-id="f127d-115">string</span><span class="sxs-lookup"><span data-stu-id="f127d-115">string</span></span>|<span data-ttu-id="f127d-116">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="f127d-116">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f127d-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f127d-117">JSON representation</span></span>

<span data-ttu-id="f127d-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f127d-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
