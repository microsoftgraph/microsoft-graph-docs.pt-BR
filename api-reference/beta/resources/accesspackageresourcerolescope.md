---
title: Tipo de recurso accessPackageResourceRoleScope
description: Um escopo de função de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso e a uma função nesse recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f899203fd58174fdb2d7935da3de4105576338d2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443199"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="1dc8d-103">Tipo de recurso accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="1dc8d-103">accessPackageResourceRoleScope resource type</span></span>

<span data-ttu-id="1dc8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dc8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dc8d-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)um escopo de função de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso e uma função nesse recurso para esse escopo.</span><span class="sxs-lookup"><span data-stu-id="1dc8d-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource for that scope.</span></span>  <span data-ttu-id="1dc8d-106">Um pacote de acesso terá escopos de função de recurso de pacote de acesso para os recursos em seu catálogo que são relevantes para esse pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="1dc8d-106">An access package will have access package resource role scopes for the resources in its catalog which are relevant to that access package.</span></span>  <span data-ttu-id="1dc8d-107">Quando um assunto recebe uma atribuição de pacote de acesso, o assunto será provisionado com a função nesse escopo de cada escopo de função de recurso do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="1dc8d-107">When a subject receives an access package assignment, the subject will be provisioned with the role in that scope of each access package resource role scope.</span></span>

## <a name="methods"></a><span data-ttu-id="1dc8d-108">Methods</span><span class="sxs-lookup"><span data-stu-id="1dc8d-108">Methods</span></span>

| <span data-ttu-id="1dc8d-109">Método</span><span class="sxs-lookup"><span data-stu-id="1dc8d-109">Method</span></span>       | <span data-ttu-id="1dc8d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1dc8d-110">Return Type</span></span> | <span data-ttu-id="1dc8d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dc8d-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1dc8d-112">Listar accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="1dc8d-112">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="1dc8d-113">[Coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="1dc8d-113">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="1dc8d-114">Recupere uma lista de **objetos accessPackageResourceRoleScope** para um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="1dc8d-114">Retrieve a list of **accessPackageResourceRoleScope** objects for an access package.</span></span> |
| [<span data-ttu-id="1dc8d-115">Criar accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="1dc8d-115">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | <span data-ttu-id="1dc8d-116">Crie um novo **objeto accessPackageResourceRoleScope** para um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="1dc8d-116">Create a new **accessPackageResourceRoleScope** object for an access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="1dc8d-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1dc8d-117">Properties</span></span>

| <span data-ttu-id="1dc8d-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1dc8d-118">Property</span></span>     | <span data-ttu-id="1dc8d-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dc8d-119">Type</span></span>        | <span data-ttu-id="1dc8d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dc8d-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1dc8d-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="1dc8d-121">createdBy</span></span>|<span data-ttu-id="1dc8d-122">String</span><span class="sxs-lookup"><span data-stu-id="1dc8d-122">String</span></span>|<span data-ttu-id="1dc8d-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dc8d-123">Read-only.</span></span>|
|<span data-ttu-id="1dc8d-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1dc8d-124">createdDateTime</span></span>|<span data-ttu-id="1dc8d-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dc8d-125">DateTimeOffset</span></span>|<span data-ttu-id="1dc8d-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1dc8d-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1dc8d-128">id</span><span class="sxs-lookup"><span data-stu-id="1dc8d-128">id</span></span>|<span data-ttu-id="1dc8d-129">String</span><span class="sxs-lookup"><span data-stu-id="1dc8d-129">String</span></span>| <span data-ttu-id="1dc8d-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dc8d-130">Read-only.</span></span>|
|<span data-ttu-id="1dc8d-131">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="1dc8d-131">modifiedBy</span></span>|<span data-ttu-id="1dc8d-132">String</span><span class="sxs-lookup"><span data-stu-id="1dc8d-132">String</span></span>|<span data-ttu-id="1dc8d-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dc8d-133">Read-only.</span></span>|
|<span data-ttu-id="1dc8d-134">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dc8d-134">modifiedDateTime</span></span>|<span data-ttu-id="1dc8d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dc8d-135">DateTimeOffset</span></span>|<span data-ttu-id="1dc8d-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1dc8d-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="1dc8d-138">Relações</span><span class="sxs-lookup"><span data-stu-id="1dc8d-138">Relationships</span></span>

| <span data-ttu-id="1dc8d-139">Relação</span><span class="sxs-lookup"><span data-stu-id="1dc8d-139">Relationship</span></span> | <span data-ttu-id="1dc8d-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="1dc8d-140">Type</span></span>        | <span data-ttu-id="1dc8d-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dc8d-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1dc8d-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="1dc8d-142">accessPackageResourceRole</span></span>|[<span data-ttu-id="1dc8d-143">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="1dc8d-143">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="1dc8d-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1dc8d-144">Read-only.</span></span> <span data-ttu-id="1dc8d-145">Anulável.</span><span class="sxs-lookup"><span data-stu-id="1dc8d-145">Nullable.</span></span>|
|<span data-ttu-id="1dc8d-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="1dc8d-146">accessPackageResourceScope</span></span>|[<span data-ttu-id="1dc8d-147">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="1dc8d-147">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="1dc8d-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="1dc8d-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1dc8d-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1dc8d-150">JSON representation</span></span>

<span data-ttu-id="1dc8d-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1dc8d-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "keyProperty": "id"
}-->

```json
{
   "createdBy":"String",
   "createdDateTime":"String (timestamp)",
   "id":"String (identifier)",
   "modifiedBy":"String",
   "modifiedDateTime":"String (timestamp)",
   "accessPackageResourceRole":{
      "id":"String (identifier)",
      "displayName":"String",
      "originSystem":"String",
      "originId":"String"
   },
   "accessPackageResourceScope":{
      "id":"String (identifier)",
      "displayName":"String",
      "description":"String",
      "originId":"String (identifier)",
      "originSystem":"String"
   }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRoleScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


