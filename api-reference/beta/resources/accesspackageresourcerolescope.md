---
title: Tipo de recurso accessPackageResourceRoleScope
description: Um escopo de função de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso e a uma função nesse recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c1446816f5487a579395f75dba521ba53f136fe
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272118"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="843e0-103">Tipo de recurso accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="843e0-103">accessPackageResourceRoleScope resource type</span></span>

<span data-ttu-id="843e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="843e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="843e0-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)um escopo de função de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso e a uma função nesse recurso para esse escopo.</span><span class="sxs-lookup"><span data-stu-id="843e0-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource for that scope.</span></span>  <span data-ttu-id="843e0-106">Um pacote de acesso terá escopos de função de recurso do pacote de acesso para os recursos em seu catálogo que são relevantes para esse pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="843e0-106">An access package will have access package resource role scopes for the resources in its catalog which are relevant to that access package.</span></span>  <span data-ttu-id="843e0-107">Quando um assunto recebe uma atribuição de pacote de acesso, o assunto será provisionado com a função nesse escopo de cada escopo de função de recurso do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="843e0-107">When a subject receives an access package assignment, the subject will be provisioned with the role in that scope of each access package resource role scope.</span></span>

## <a name="methods"></a><span data-ttu-id="843e0-108">Methods</span><span class="sxs-lookup"><span data-stu-id="843e0-108">Methods</span></span>

| <span data-ttu-id="843e0-109">Método</span><span class="sxs-lookup"><span data-stu-id="843e0-109">Method</span></span>       | <span data-ttu-id="843e0-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="843e0-110">Return Type</span></span> | <span data-ttu-id="843e0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="843e0-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="843e0-112">Listar accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="843e0-112">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="843e0-113">[Coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="843e0-113">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="843e0-114">Recupere uma lista de **objetos accessPackageResourceRoleScope** para um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="843e0-114">Retrieve a list of **accessPackageResourceRoleScope** objects for an access package.</span></span> |
| [<span data-ttu-id="843e0-115">Criar accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="843e0-115">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | <span data-ttu-id="843e0-116">Crie um novo **objeto accessPackageResourceRoleScope** para um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="843e0-116">Create a new **accessPackageResourceRoleScope** object for an access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="843e0-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="843e0-117">Properties</span></span>

| <span data-ttu-id="843e0-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="843e0-118">Property</span></span>     | <span data-ttu-id="843e0-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="843e0-119">Type</span></span>        | <span data-ttu-id="843e0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="843e0-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="843e0-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="843e0-121">createdBy</span></span>|<span data-ttu-id="843e0-122">String</span><span class="sxs-lookup"><span data-stu-id="843e0-122">String</span></span>|<span data-ttu-id="843e0-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="843e0-123">Read-only.</span></span>|
|<span data-ttu-id="843e0-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="843e0-124">createdDateTime</span></span>|<span data-ttu-id="843e0-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="843e0-125">DateTimeOffset</span></span>|<span data-ttu-id="843e0-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="843e0-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="843e0-128">id</span><span class="sxs-lookup"><span data-stu-id="843e0-128">id</span></span>|<span data-ttu-id="843e0-129">String</span><span class="sxs-lookup"><span data-stu-id="843e0-129">String</span></span>| <span data-ttu-id="843e0-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="843e0-130">Read-only.</span></span>|
|<span data-ttu-id="843e0-131">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="843e0-131">modifiedBy</span></span>|<span data-ttu-id="843e0-132">String</span><span class="sxs-lookup"><span data-stu-id="843e0-132">String</span></span>|<span data-ttu-id="843e0-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="843e0-133">Read-only.</span></span>|
|<span data-ttu-id="843e0-134">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="843e0-134">modifiedDateTime</span></span>|<span data-ttu-id="843e0-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="843e0-135">DateTimeOffset</span></span>|<span data-ttu-id="843e0-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="843e0-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="843e0-138">Relações</span><span class="sxs-lookup"><span data-stu-id="843e0-138">Relationships</span></span>

| <span data-ttu-id="843e0-139">Relação</span><span class="sxs-lookup"><span data-stu-id="843e0-139">Relationship</span></span> | <span data-ttu-id="843e0-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="843e0-140">Type</span></span>        | <span data-ttu-id="843e0-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="843e0-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="843e0-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="843e0-142">accessPackageResourceRole</span></span>|[<span data-ttu-id="843e0-143">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="843e0-143">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="843e0-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="843e0-144">Read-only.</span></span> <span data-ttu-id="843e0-145">Anulável.</span><span class="sxs-lookup"><span data-stu-id="843e0-145">Nullable.</span></span>|
|<span data-ttu-id="843e0-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="843e0-146">accessPackageResourceScope</span></span>|[<span data-ttu-id="843e0-147">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="843e0-147">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="843e0-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="843e0-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="843e0-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="843e0-150">JSON representation</span></span>

<span data-ttu-id="843e0-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="843e0-151">The following is a JSON representation of the resource.</span></span>

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


