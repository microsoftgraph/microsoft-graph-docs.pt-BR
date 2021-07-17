---
title: Tipo de recurso acl
description: Uma entrada de controle de acesso para um item indexado por um Pesquisa da Microsoft externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 171b53adc815638546bbdf71411c58d293c05de4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467204"
---
# <a name="acl-resource-type"></a><span data-ttu-id="c8bae-103">Tipo de recurso acl</span><span class="sxs-lookup"><span data-stu-id="c8bae-103">acl resource type</span></span>

<span data-ttu-id="c8bae-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="c8bae-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="c8bae-105">Uma entrada de controle de acesso para um item indexado por um Pesquisa da Microsoft externalConnection.</span><span class="sxs-lookup"><span data-stu-id="c8bae-105">An access control entry for an item indexed by a Microsoft Search externalConnection.</span></span>

## <a name="properties"></a><span data-ttu-id="c8bae-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8bae-106">Properties</span></span>
|<span data-ttu-id="c8bae-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8bae-107">Property</span></span>|<span data-ttu-id="c8bae-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8bae-108">Type</span></span>|<span data-ttu-id="c8bae-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8bae-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8bae-110">accessType</span><span class="sxs-lookup"><span data-stu-id="c8bae-110">accessType</span></span>|<span data-ttu-id="c8bae-111">microsoft.graph.externalConnectors.accessType</span><span class="sxs-lookup"><span data-stu-id="c8bae-111">microsoft.graph.externalConnectors.accessType</span></span>|<span data-ttu-id="c8bae-112">O acesso concedido à identidade.</span><span class="sxs-lookup"><span data-stu-id="c8bae-112">The access granted to the identity.</span></span> <span data-ttu-id="c8bae-113">Os valores possíveis são: `grant`, `deny`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c8bae-113">Possible values are: `grant`, `deny`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c8bae-114">tipo</span><span class="sxs-lookup"><span data-stu-id="c8bae-114">type</span></span>|<span data-ttu-id="c8bae-115">microsoft.graph.externalConnectors.aclType</span><span class="sxs-lookup"><span data-stu-id="c8bae-115">microsoft.graph.externalConnectors.aclType</span></span>|<span data-ttu-id="c8bae-116">O tipo de identidade.</span><span class="sxs-lookup"><span data-stu-id="c8bae-116">The type of identity.</span></span> <span data-ttu-id="c8bae-117">Os possíveis valores são: `user`, `group`, `everyone`, `everyoneExceptGuests`, `externalGroup`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c8bae-117">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests`, `externalGroup`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c8bae-118">value</span><span class="sxs-lookup"><span data-stu-id="c8bae-118">value</span></span>|<span data-ttu-id="c8bae-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8bae-119">String</span></span>|<span data-ttu-id="c8bae-120">O identificador exclusivo da identidade.</span><span class="sxs-lookup"><span data-stu-id="c8bae-120">The unique identifer of the identity.</span></span> <span data-ttu-id="c8bae-121">No caso de Azure Active Directory identidades, é definido como o identificador de objeto do usuário, grupo ou locatário para tipos de usuário, grupo e todos `value` (e todosExceptGuests), respectivamente.</span><span class="sxs-lookup"><span data-stu-id="c8bae-121">In case of Azure Active Directory identities, `value` is set to the object identifier of the user, group or tenant for types user, group and everyone (and everyoneExceptGuests) respectively.</span></span> <span data-ttu-id="c8bae-122">No caso de grupos `value` externos ser definido como a ID do externalGroup</span><span class="sxs-lookup"><span data-stu-id="c8bae-122">In case of external groups `value` is set to the ID of the externalGroup</span></span> |

## <a name="relationships"></a><span data-ttu-id="c8bae-123">Relações</span><span class="sxs-lookup"><span data-stu-id="c8bae-123">Relationships</span></span>
<span data-ttu-id="c8bae-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8bae-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8bae-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8bae-125">JSON representation</span></span>
<span data-ttu-id="c8bae-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8bae-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.acl"
}
-->
``` json
{
  "type": "String",
  "value": "String",
  "accessType": "String"
}
```

