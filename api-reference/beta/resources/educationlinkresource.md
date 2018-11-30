---
title: tipo de recurso de educationLinkResource
description: Uma subclasse de educationResource. Este recurso é um vínculo e não tem quaisquer dados adicionais associado a ela.
ms.openlocfilehash: 314bd87998ada178484401b2122f0936f87e51a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038530"
---
# <a name="educationlinkresource-resource-type"></a><span data-ttu-id="f91e0-104">tipo de recurso de educationLinkResource</span><span class="sxs-lookup"><span data-stu-id="f91e0-104">educationLinkResource resource type</span></span>

> <span data-ttu-id="f91e0-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f91e0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f91e0-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f91e0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f91e0-107">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="f91e0-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="f91e0-108">Este recurso é um vínculo e não tem quaisquer dados adicionais associado a ela.</span><span class="sxs-lookup"><span data-stu-id="f91e0-108">This resource is a link and does not have any additional data associated with it.</span></span>


## <a name="properties"></a><span data-ttu-id="f91e0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f91e0-109">Properties</span></span>
| <span data-ttu-id="f91e0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f91e0-110">Property</span></span>     | <span data-ttu-id="f91e0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f91e0-111">Type</span></span>   |<span data-ttu-id="f91e0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f91e0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f91e0-113">vínculo</span><span class="sxs-lookup"><span data-stu-id="f91e0-113">link</span></span>|<span data-ttu-id="f91e0-114">String</span><span class="sxs-lookup"><span data-stu-id="f91e0-114">String</span></span>|<span data-ttu-id="f91e0-115">URL para o recurso.</span><span class="sxs-lookup"><span data-stu-id="f91e0-115">URL to the resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f91e0-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f91e0-116">JSON representation</span></span>

<span data-ttu-id="f91e0-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f91e0-117">The following is a JSON representation of the resource.</span></span>

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