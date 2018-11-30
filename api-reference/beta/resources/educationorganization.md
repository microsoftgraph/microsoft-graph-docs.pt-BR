---
title: tipo de recurso de educationOrganization
description: 'Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.  '
ms.openlocfilehash: 86da4e19f9cc36de7a61ca2c76565a17ec3acac0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036003"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="2bfa8-103">tipo de recurso de educationOrganization</span><span class="sxs-lookup"><span data-stu-id="2bfa8-103">educationOrganization resource type</span></span>

> <span data-ttu-id="2bfa8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2bfa8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2bfa8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2bfa8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2bfa8-106">Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.</span><span class="sxs-lookup"><span data-stu-id="2bfa8-106">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="2bfa8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2bfa8-107">Properties</span></span>
| <span data-ttu-id="2bfa8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2bfa8-108">Property</span></span>     | <span data-ttu-id="2bfa8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2bfa8-109">Type</span></span>   |<span data-ttu-id="2bfa8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bfa8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bfa8-111">description</span><span class="sxs-lookup"><span data-stu-id="2bfa8-111">description</span></span>|<span data-ttu-id="2bfa8-112">String</span><span class="sxs-lookup"><span data-stu-id="2bfa8-112">String</span></span>| <span data-ttu-id="2bfa8-113">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="2bfa8-113">Organization description.</span></span>|
|<span data-ttu-id="2bfa8-114">displayName</span><span class="sxs-lookup"><span data-stu-id="2bfa8-114">displayName</span></span>|<span data-ttu-id="2bfa8-115">String</span><span class="sxs-lookup"><span data-stu-id="2bfa8-115">String</span></span>| <span data-ttu-id="2bfa8-116">Nome de exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="2bfa8-116">Organization display name.</span></span>|
|<span data-ttu-id="2bfa8-117">externalSource</span><span class="sxs-lookup"><span data-stu-id="2bfa8-117">externalSource</span></span>|<span data-ttu-id="2bfa8-118">string</span><span class="sxs-lookup"><span data-stu-id="2bfa8-118">string</span></span>| <span data-ttu-id="2bfa8-119">Fonte local a partir do qual esta organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="2bfa8-119">Source where this organization was created from.</span></span> <span data-ttu-id="2bfa8-120">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="2bfa8-120">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bfa8-121">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="2bfa8-121">Relationships</span></span>
<span data-ttu-id="2bfa8-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2bfa8-122">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2bfa8-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2bfa8-123">JSON representation</span></span>

<span data-ttu-id="2bfa8-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2bfa8-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->