---
title: Tipo de recurso phone
description: Representa um número de telefone.
localization_priority: Normal
ms.openlocfilehash: 7397349e1fee1164d3bcde8ebc785edd9402fe75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874176"
---
# <a name="phone-resource-type"></a><span data-ttu-id="cf0a6-103">Tipo de recurso phone</span><span class="sxs-lookup"><span data-stu-id="cf0a6-103">phone resource type</span></span>

> <span data-ttu-id="cf0a6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cf0a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf0a6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cf0a6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cf0a6-106">Representa um número de telefone.</span><span class="sxs-lookup"><span data-stu-id="cf0a6-106">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="cf0a6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf0a6-107">Properties</span></span>
| <span data-ttu-id="cf0a6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf0a6-108">Property</span></span>     | <span data-ttu-id="cf0a6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf0a6-109">Type</span></span>   |<span data-ttu-id="cf0a6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf0a6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf0a6-111">number</span><span class="sxs-lookup"><span data-stu-id="cf0a6-111">number</span></span>|<span data-ttu-id="cf0a6-112">string</span><span class="sxs-lookup"><span data-stu-id="cf0a6-112">string</span></span>|<span data-ttu-id="cf0a6-113">O número de telefone.</span><span class="sxs-lookup"><span data-stu-id="cf0a6-113">The phone number.</span></span>|
|<span data-ttu-id="cf0a6-114">type</span><span class="sxs-lookup"><span data-stu-id="cf0a6-114">type</span></span>|<span data-ttu-id="cf0a6-115">String</span><span class="sxs-lookup"><span data-stu-id="cf0a6-115">String</span></span>|<span data-ttu-id="cf0a6-p102">O tipo de número de telefone. Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="cf0a6-p102">The type of phone number. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf0a6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf0a6-118">JSON representation</span></span>

<span data-ttu-id="cf0a6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf0a6-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
