---
title: Tipo de recurso personType
description: Representa o tipo de pessoa.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 270fa800242ae7a25ed0f5959a97b6a70f7cedd3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462456"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="0bcfc-103">Tipo de recurso personType</span><span class="sxs-lookup"><span data-stu-id="0bcfc-103">personType resource type</span></span>

<span data-ttu-id="0bcfc-104">Representa o tipo de pessoa.</span><span class="sxs-lookup"><span data-stu-id="0bcfc-104">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0bcfc-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0bcfc-105">JSON representation</span></span>

<span data-ttu-id="0bcfc-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0bcfc-106">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personType"
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a><span data-ttu-id="0bcfc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0bcfc-107">Properties</span></span>
| <span data-ttu-id="0bcfc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bcfc-108">Property</span></span>     | <span data-ttu-id="0bcfc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bcfc-109">Type</span></span>   |<span data-ttu-id="0bcfc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bcfc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0bcfc-111">classe</span><span class="sxs-lookup"><span data-stu-id="0bcfc-111">class</span></span>|<span data-ttu-id="0bcfc-112">String</span><span class="sxs-lookup"><span data-stu-id="0bcfc-112">String</span></span>|<span data-ttu-id="0bcfc-113">O tipo de fonte de dados, como Pessoa.</span><span class="sxs-lookup"><span data-stu-id="0bcfc-113">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="0bcfc-114">subclasse</span><span class="sxs-lookup"><span data-stu-id="0bcfc-114">subclass</span></span>|<span data-ttu-id="0bcfc-115">String</span><span class="sxs-lookup"><span data-stu-id="0bcfc-115">String</span></span>|<span data-ttu-id="0bcfc-116">O tipo secundário de fonte de dados, como OrganizationUser.</span><span class="sxs-lookup"><span data-stu-id="0bcfc-116">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
