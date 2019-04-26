---
title: tipo de recurso SettingValue
description: Uma configuração representada por um par de nome/valor.
localization_priority: Normal
ms.openlocfilehash: 3edf5bdc1fae77702206eae78d53fcf0fdc5b644
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549682"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="25961-103">tipo de recurso SettingValue</span><span class="sxs-lookup"><span data-stu-id="25961-103">settingValue resource type</span></span>

<span data-ttu-id="25961-104">Uma configuração representada por um par de nome/valor.</span><span class="sxs-lookup"><span data-stu-id="25961-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="25961-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25961-105">Properties</span></span>

| <span data-ttu-id="25961-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25961-106">Property</span></span> | <span data-ttu-id="25961-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="25961-107">Type</span></span> | <span data-ttu-id="25961-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="25961-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="25961-109">name</span><span class="sxs-lookup"><span data-stu-id="25961-109">name</span></span>|<span data-ttu-id="25961-110">String</span><span class="sxs-lookup"><span data-stu-id="25961-110">String</span></span>| <span data-ttu-id="25961-111">Nome da configuração (conforme definido pelo [groupSettingTemplate](groupsettingtemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="25961-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="25961-112">value</span><span class="sxs-lookup"><span data-stu-id="25961-112">value</span></span>|<span data-ttu-id="25961-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25961-113">String</span></span>| <span data-ttu-id="25961-114">Valor da configuração.</span><span class="sxs-lookup"><span data-stu-id="25961-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="25961-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25961-115">JSON representation</span></span>

<span data-ttu-id="25961-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25961-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
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
