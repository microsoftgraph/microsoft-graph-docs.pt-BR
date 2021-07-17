---
title: Tipo de recurso acl
description: Uma entrada de controle de acesso para um item indexado por um Pesquisa da Microsoft externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 339b5ab51fd604cae2dd42e2ec853ede8d27ef5b
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467573"
---
# <a name="acl-resource-type"></a><span data-ttu-id="fdcc1-103">Tipo de recurso acl</span><span class="sxs-lookup"><span data-stu-id="fdcc1-103">acl resource type</span></span>

<span data-ttu-id="fdcc1-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="fdcc1-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdcc1-105">Uma entrada de controle de acesso para um item indexado por um Pesquisa da Microsoft [externalConnection](externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="fdcc1-105">An access control entry for an item indexed by a Microsoft Search [externalConnection](externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fdcc1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fdcc1-106">Properties</span></span>

| <span data-ttu-id="fdcc1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdcc1-107">Property</span></span>       | <span data-ttu-id="fdcc1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdcc1-108">Type</span></span>   | <span data-ttu-id="fdcc1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdcc1-109">Description</span></span>                                        |
|:---------------|:-------|:---------------------------------------------------|
| <span data-ttu-id="fdcc1-110">accessType</span><span class="sxs-lookup"><span data-stu-id="fdcc1-110">accessType</span></span>     | <span data-ttu-id="fdcc1-111">String</span><span class="sxs-lookup"><span data-stu-id="fdcc1-111">String</span></span> | <span data-ttu-id="fdcc1-112">O acesso concedido à identidade.</span><span class="sxs-lookup"><span data-stu-id="fdcc1-112">The access granted to the identity.</span></span> <span data-ttu-id="fdcc1-113">Os valores possíveis são: `grant` e `deny`.</span><span class="sxs-lookup"><span data-stu-id="fdcc1-113">Possible values are: `grant`, `deny`.</span></span> |
| <span data-ttu-id="fdcc1-114">identitySource</span><span class="sxs-lookup"><span data-stu-id="fdcc1-114">identitySource</span></span> | <span data-ttu-id="fdcc1-115">String</span><span class="sxs-lookup"><span data-stu-id="fdcc1-115">String</span></span> | <span data-ttu-id="fdcc1-116">A origem da identidade.</span><span class="sxs-lookup"><span data-stu-id="fdcc1-116">The source of identity.</span></span> <span data-ttu-id="fdcc1-117">Os valores possíveis são: `azureActiveDirectory` ou `external`.</span><span class="sxs-lookup"><span data-stu-id="fdcc1-117">Possible values are `azureActiveDirectory` or `external`.</span></span>           |
| <span data-ttu-id="fdcc1-118">tipo</span><span class="sxs-lookup"><span data-stu-id="fdcc1-118">type</span></span>           | <span data-ttu-id="fdcc1-119">String</span><span class="sxs-lookup"><span data-stu-id="fdcc1-119">String</span></span> | <span data-ttu-id="fdcc1-120">O tipo de identidade.</span><span class="sxs-lookup"><span data-stu-id="fdcc1-120">The type of identity.</span></span> <span data-ttu-id="fdcc1-121">Os valores possíveis são: `user` , , , se a `group` `everyone` `everyoneExceptGuests` identitySource for `azureActiveDirectory` e apenas se a `group` identitySource for `external` .</span><span class="sxs-lookup"><span data-stu-id="fdcc1-121">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests` if the identitySource is `azureActiveDirectory` and just `group` if the identitySource is `external`.</span></span> |
| <span data-ttu-id="fdcc1-122">value</span><span class="sxs-lookup"><span data-stu-id="fdcc1-122">value</span></span>          | <span data-ttu-id="fdcc1-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fdcc1-123">String</span></span> | <span data-ttu-id="fdcc1-124">O identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="fdcc1-124">The unique identifer of the identity.</span></span> <span data-ttu-id="fdcc1-125">No caso de Azure Active Directory identidades, é definido como o identificador de objeto do usuário, grupo ou locatário para tipos de usuário, grupo e todos `value` (e todosExceptGuests), respectivamente.</span><span class="sxs-lookup"><span data-stu-id="fdcc1-125">In case of Azure Active Directory identities, `value` is set to the object identifier of the user, group or tenant for types user, group and everyone (and everyoneExceptGuests) respectively.</span></span> <span data-ttu-id="fdcc1-126">No caso de grupos `value` externos ser definido como a ID do [externalGroup](externalconnectors-externalgroup.md).</span><span class="sxs-lookup"><span data-stu-id="fdcc1-126">In case of external groups `value` is set to the ID of the [externalGroup](externalconnectors-externalgroup.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fdcc1-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fdcc1-127">JSON representation</span></span>

<span data-ttu-id="fdcc1-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fdcc1-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.acl",
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
