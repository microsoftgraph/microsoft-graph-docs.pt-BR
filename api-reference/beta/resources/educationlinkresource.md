---
title: tipo de recurso de educationLinkResource
description: Uma subclasse de educationResource. Este recurso é um vínculo e não tem quaisquer dados adicionais associado a ela.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8cdcb47c02481f2f43ee71f46c24e2b8d8f5ba2a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918046"
---
# <a name="educationlinkresource-resource-type"></a><span data-ttu-id="4ce33-104">tipo de recurso de educationLinkResource</span><span class="sxs-lookup"><span data-stu-id="4ce33-104">educationLinkResource resource type</span></span>

> <span data-ttu-id="4ce33-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4ce33-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ce33-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4ce33-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4ce33-107">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="4ce33-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="4ce33-108">Este recurso é um vínculo e não tem quaisquer dados adicionais associado a ela.</span><span class="sxs-lookup"><span data-stu-id="4ce33-108">This resource is a link and does not have any additional data associated with it.</span></span>


## <a name="properties"></a><span data-ttu-id="4ce33-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ce33-109">Properties</span></span>
| <span data-ttu-id="4ce33-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ce33-110">Property</span></span>     | <span data-ttu-id="4ce33-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ce33-111">Type</span></span>   |<span data-ttu-id="4ce33-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ce33-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ce33-113">vínculo</span><span class="sxs-lookup"><span data-stu-id="4ce33-113">link</span></span>|<span data-ttu-id="4ce33-114">String</span><span class="sxs-lookup"><span data-stu-id="4ce33-114">String</span></span>|<span data-ttu-id="4ce33-115">URL para o recurso.</span><span class="sxs-lookup"><span data-stu-id="4ce33-115">URL to the resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ce33-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ce33-116">JSON representation</span></span>

<span data-ttu-id="4ce33-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ce33-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationLinkResource"
}-->

```json
{
  "link": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
