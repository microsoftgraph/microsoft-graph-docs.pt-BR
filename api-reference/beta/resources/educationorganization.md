---
title: tipo de recurso de educationOrganization
description: 'Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a1e3f82e2d777b1d32cc445f543e7beed570a8b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949518"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="32e65-103">tipo de recurso de educationOrganization</span><span class="sxs-lookup"><span data-stu-id="32e65-103">educationOrganization resource type</span></span>

> <span data-ttu-id="32e65-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="32e65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32e65-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="32e65-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32e65-106">Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.</span><span class="sxs-lookup"><span data-stu-id="32e65-106">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="32e65-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32e65-107">Properties</span></span>
| <span data-ttu-id="32e65-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32e65-108">Property</span></span>     | <span data-ttu-id="32e65-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="32e65-109">Type</span></span>   |<span data-ttu-id="32e65-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="32e65-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32e65-111">description</span><span class="sxs-lookup"><span data-stu-id="32e65-111">description</span></span>|<span data-ttu-id="32e65-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32e65-112">String</span></span>| <span data-ttu-id="32e65-113">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="32e65-113">Organization description.</span></span>|
|<span data-ttu-id="32e65-114">displayName</span><span class="sxs-lookup"><span data-stu-id="32e65-114">displayName</span></span>|<span data-ttu-id="32e65-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32e65-115">String</span></span>| <span data-ttu-id="32e65-116">Nome de exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="32e65-116">Organization display name.</span></span>|
|<span data-ttu-id="32e65-117">externalSource</span><span class="sxs-lookup"><span data-stu-id="32e65-117">externalSource</span></span>|<span data-ttu-id="32e65-118">string</span><span class="sxs-lookup"><span data-stu-id="32e65-118">string</span></span>| <span data-ttu-id="32e65-119">Fonte local a partir do qual esta organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="32e65-119">Source where this organization was created from.</span></span> <span data-ttu-id="32e65-120">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="32e65-120">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32e65-121">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="32e65-121">Relationships</span></span>
<span data-ttu-id="32e65-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="32e65-122">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="32e65-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32e65-123">JSON representation</span></span>

<span data-ttu-id="32e65-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32e65-124">The following is a JSON representation of the resource.</span></span>

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
