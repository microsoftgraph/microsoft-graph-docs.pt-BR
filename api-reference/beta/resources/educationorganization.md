---
title: tipo de recurso de educationOrganization
description: 'Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.  '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: c9930a32e52e9380e26c6fa94095b3a7099beb70
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822502"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="22554-103">tipo de recurso de educationOrganization</span><span class="sxs-lookup"><span data-stu-id="22554-103">educationOrganization resource type</span></span>

> <span data-ttu-id="22554-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="22554-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22554-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="22554-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22554-106">Entidade abstrata usada para modelar o comum entre os tipos de organização diferentes dentro do setor de educação.</span><span class="sxs-lookup"><span data-stu-id="22554-106">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="22554-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22554-107">Properties</span></span>
| <span data-ttu-id="22554-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22554-108">Property</span></span>     | <span data-ttu-id="22554-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="22554-109">Type</span></span>   |<span data-ttu-id="22554-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="22554-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22554-111">description</span><span class="sxs-lookup"><span data-stu-id="22554-111">description</span></span>|<span data-ttu-id="22554-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22554-112">String</span></span>| <span data-ttu-id="22554-113">Descrição da organização.</span><span class="sxs-lookup"><span data-stu-id="22554-113">Organization description.</span></span>|
|<span data-ttu-id="22554-114">displayName</span><span class="sxs-lookup"><span data-stu-id="22554-114">displayName</span></span>|<span data-ttu-id="22554-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22554-115">String</span></span>| <span data-ttu-id="22554-116">Nome de exibição da organização.</span><span class="sxs-lookup"><span data-stu-id="22554-116">Organization display name.</span></span>|
|<span data-ttu-id="22554-117">externalSource</span><span class="sxs-lookup"><span data-stu-id="22554-117">externalSource</span></span>|<span data-ttu-id="22554-118">string</span><span class="sxs-lookup"><span data-stu-id="22554-118">string</span></span>| <span data-ttu-id="22554-119">Fonte local a partir do qual esta organização foi criada.</span><span class="sxs-lookup"><span data-stu-id="22554-119">Source where this organization was created from.</span></span> <span data-ttu-id="22554-120">Os valores possíveis são: `sis`, `manual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="22554-120">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22554-121">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="22554-121">Relationships</span></span>
<span data-ttu-id="22554-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="22554-122">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="22554-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22554-123">JSON representation</span></span>

<span data-ttu-id="22554-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22554-124">The following is a JSON representation of the resource.</span></span>

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
