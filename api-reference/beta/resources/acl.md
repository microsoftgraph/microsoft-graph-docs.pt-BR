---
title: tipo de recurso ACL
description: Uma entrada de controle de acesso para um item indexado por um externalConnection de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5a26004cf20a5f8c5c032eeade8f657fdf8bd93c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703937"
---
# <a name="acl-resource-type"></a><span data-ttu-id="476d3-103">tipo de recurso ACL</span><span class="sxs-lookup"><span data-stu-id="476d3-103">acl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="476d3-104">Uma entrada de controle de acesso para um item indexado por um [externalConnection](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="476d3-104">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="476d3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="476d3-105">Properties</span></span>

| <span data-ttu-id="476d3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="476d3-106">Property</span></span>       | <span data-ttu-id="476d3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="476d3-107">Type</span></span>   | <span data-ttu-id="476d3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="476d3-108">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="476d3-109">accessType</span><span class="sxs-lookup"><span data-stu-id="476d3-109">accessType</span></span>     | <span data-ttu-id="476d3-110">String</span><span class="sxs-lookup"><span data-stu-id="476d3-110">String</span></span> | <span data-ttu-id="476d3-111">O acesso concedido à identidade.</span><span class="sxs-lookup"><span data-stu-id="476d3-111">The access granted to the identity.</span></span> <span data-ttu-id="476d3-112">Os valores possíveis são: `grant` e `deny`.</span><span class="sxs-lookup"><span data-stu-id="476d3-112">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="476d3-113">identificação da identidade</span><span class="sxs-lookup"><span data-stu-id="476d3-113">identitySource</span></span> | <span data-ttu-id="476d3-114">String</span><span class="sxs-lookup"><span data-stu-id="476d3-114">String</span></span> | <span data-ttu-id="476d3-115">Deve ser definida como `Azure Active Directory`.</span><span class="sxs-lookup"><span data-stu-id="476d3-115">Must be set to `Azure Active Directory`.</span></span>           |
| <span data-ttu-id="476d3-116">type</span><span class="sxs-lookup"><span data-stu-id="476d3-116">type</span></span>           | <span data-ttu-id="476d3-117">String</span><span class="sxs-lookup"><span data-stu-id="476d3-117">String</span></span> | <span data-ttu-id="476d3-118">O tipo de identidade.</span><span class="sxs-lookup"><span data-stu-id="476d3-118">The type of identity.</span></span> <span data-ttu-id="476d3-119">Os valores possíveis são: `user`, `group`, `everyone`, `everyoneExceptGuests`.</span><span class="sxs-lookup"><span data-stu-id="476d3-119">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests`.</span></span> |
| <span data-ttu-id="476d3-120">value</span><span class="sxs-lookup"><span data-stu-id="476d3-120">value</span></span>          | <span data-ttu-id="476d3-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="476d3-121">String</span></span> | <span data-ttu-id="476d3-122">O identificador do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="476d3-122">The Azure Active Directory identifer.</span></span> <span data-ttu-id="476d3-123">Se `type` for `user` ou `group`, `value` será definido como o identificador de objeto para o usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="476d3-123">If `type` is `user` or `group`, `value` is set to the object identifier for the user or group.</span></span> <span data-ttu-id="476d3-124">Se `type` for `everyone` ou `everyoneExceptGuests`, `value` será definido como o identificador de locatário para o locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="476d3-124">If `type` is `everyone` or `everyoneExceptGuests`, `value` is set to the tenant identifier for the Azure Active Directory tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="476d3-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="476d3-125">JSON representation</span></span>

<span data-ttu-id="476d3-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="476d3-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.acl",
  "baseType": null
}-->

```json
{
  "accessType": "String",
  "identitySource": "String",
  "type": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "acl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
