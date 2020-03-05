---
title: tipo de recurso ACL
description: Uma entrada de controle de acesso para um item indexado por um externalConnection de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a957feaffe36e76a36958ef7855376bcfe58484e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508447"
---
# <a name="acl-resource-type"></a><span data-ttu-id="1643e-103">tipo de recurso ACL</span><span class="sxs-lookup"><span data-stu-id="1643e-103">acl resource type</span></span>

<span data-ttu-id="1643e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1643e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1643e-105">Uma entrada de controle de acesso para um item indexado por um [externalConnection](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1643e-105">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="1643e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1643e-106">Properties</span></span>

| <span data-ttu-id="1643e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1643e-107">Property</span></span>       | <span data-ttu-id="1643e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1643e-108">Type</span></span>   | <span data-ttu-id="1643e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1643e-109">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="1643e-110">accessType</span><span class="sxs-lookup"><span data-stu-id="1643e-110">accessType</span></span>     | <span data-ttu-id="1643e-111">String</span><span class="sxs-lookup"><span data-stu-id="1643e-111">String</span></span> | <span data-ttu-id="1643e-112">O acesso concedido à identidade.</span><span class="sxs-lookup"><span data-stu-id="1643e-112">The access granted to the identity.</span></span> <span data-ttu-id="1643e-113">Os valores possíveis são: `grant` e `deny`.</span><span class="sxs-lookup"><span data-stu-id="1643e-113">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="1643e-114">identificação da identidade</span><span class="sxs-lookup"><span data-stu-id="1643e-114">identitySource</span></span> | <span data-ttu-id="1643e-115">String</span><span class="sxs-lookup"><span data-stu-id="1643e-115">String</span></span> | <span data-ttu-id="1643e-116">Tem que ser definida como `Azure Active Directory`.</span><span class="sxs-lookup"><span data-stu-id="1643e-116">Must be set to `Azure Active Directory`.</span></span>           |
| <span data-ttu-id="1643e-117">type</span><span class="sxs-lookup"><span data-stu-id="1643e-117">type</span></span>           | <span data-ttu-id="1643e-118">String</span><span class="sxs-lookup"><span data-stu-id="1643e-118">String</span></span> | <span data-ttu-id="1643e-119">O tipo de identidade.</span><span class="sxs-lookup"><span data-stu-id="1643e-119">The type of identity.</span></span> <span data-ttu-id="1643e-120">Os valores possíveis são: `user`, `group`, `everyone`, `everyoneExceptGuests`.</span><span class="sxs-lookup"><span data-stu-id="1643e-120">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests`.</span></span> |
| <span data-ttu-id="1643e-121">value</span><span class="sxs-lookup"><span data-stu-id="1643e-121">value</span></span>          | <span data-ttu-id="1643e-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1643e-122">String</span></span> | <span data-ttu-id="1643e-123">O identificador do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1643e-123">The Azure Active Directory identifer.</span></span> <span data-ttu-id="1643e-124">Se `type` for `user` ou `group`, `value` será definido como o identificador de objeto para o usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="1643e-124">If `type` is `user` or `group`, `value` is set to the object identifier for the user or group.</span></span> <span data-ttu-id="1643e-125">Se `type` for `everyone` ou `everyoneExceptGuests`, `value` será definido como o identificador de locatário para o locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1643e-125">If `type` is `everyone` or `everyoneExceptGuests`, `value` is set to the tenant identifier for the Azure Active Directory tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1643e-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1643e-126">JSON representation</span></span>

<span data-ttu-id="1643e-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1643e-127">The following is a JSON representation of the resource.</span></span>

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
