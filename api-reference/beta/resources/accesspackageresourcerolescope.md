---
title: tipo de recurso accessPackageResourceRoleScope
description: Um escopo de função de recurso de pacote do Access é uma referência a um escopo dentro de um recurso e uma função nesse recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c96d5a0499ae269c7ce67bae2252c6521d66eb7b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024644"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="62392-103">tipo de recurso accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="62392-103">accessPackageResourceRoleScope resource type</span></span>

<span data-ttu-id="62392-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62392-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62392-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um escopo de função de recurso de pacote de acesso é uma referência a um escopo dentro de um recurso e uma função nesse recurso para esse escopo.</span><span class="sxs-lookup"><span data-stu-id="62392-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource for that scope.</span></span>  <span data-ttu-id="62392-106">Um pacote de acesso terá escopos de função de recurso pacote de acesso para os recursos em seu catálogo que são relevantes para esse pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="62392-106">An access package will have access package resource role scopes for the resources in its catalog which are relevant to that access package.</span></span>  <span data-ttu-id="62392-107">Quando um assunto recebe uma atribuição de pacote do Access, o assunto será provisionado com a função nesse escopo de cada escopo de função de recurso de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="62392-107">When a subject receives an access package assignment, the subject will be provisioned with the role in that scope of each access package resource role scope.</span></span>

## <a name="methods"></a><span data-ttu-id="62392-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="62392-108">Methods</span></span>

| <span data-ttu-id="62392-109">Método</span><span class="sxs-lookup"><span data-stu-id="62392-109">Method</span></span>       | <span data-ttu-id="62392-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="62392-110">Return Type</span></span> | <span data-ttu-id="62392-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="62392-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="62392-112">Listar accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="62392-112">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="62392-113">coleção [accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="62392-113">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="62392-114">Recupere uma lista de objetos **accessPackageResourceRoleScope** para um pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="62392-114">Retrieve a list of **accessPackageResourceRoleScope** objects for an access package.</span></span> |
| [<span data-ttu-id="62392-115">Criar accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="62392-115">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | <span data-ttu-id="62392-116">Criar um novo objeto **accessPackageResourceRoleScope** para um pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="62392-116">Create a new **accessPackageResourceRoleScope** object for an access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="62392-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62392-117">Properties</span></span>

| <span data-ttu-id="62392-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62392-118">Property</span></span>     | <span data-ttu-id="62392-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="62392-119">Type</span></span>        | <span data-ttu-id="62392-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="62392-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="62392-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="62392-121">createdBy</span></span>|<span data-ttu-id="62392-122">String</span><span class="sxs-lookup"><span data-stu-id="62392-122">String</span></span>|<span data-ttu-id="62392-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="62392-123">Read-only.</span></span>|
|<span data-ttu-id="62392-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62392-124">createdDateTime</span></span>|<span data-ttu-id="62392-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62392-125">DateTimeOffset</span></span>|<span data-ttu-id="62392-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="62392-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="62392-128">id</span><span class="sxs-lookup"><span data-stu-id="62392-128">id</span></span>|<span data-ttu-id="62392-129">String</span><span class="sxs-lookup"><span data-stu-id="62392-129">String</span></span>| <span data-ttu-id="62392-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="62392-130">Read-only.</span></span>|
|<span data-ttu-id="62392-131">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="62392-131">modifiedBy</span></span>|<span data-ttu-id="62392-132">String</span><span class="sxs-lookup"><span data-stu-id="62392-132">String</span></span>|<span data-ttu-id="62392-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="62392-133">Read-only.</span></span>|
|<span data-ttu-id="62392-134">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62392-134">modifiedDateTime</span></span>|<span data-ttu-id="62392-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62392-135">DateTimeOffset</span></span>|<span data-ttu-id="62392-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="62392-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="62392-138">Relações</span><span class="sxs-lookup"><span data-stu-id="62392-138">Relationships</span></span>

| <span data-ttu-id="62392-139">Relação</span><span class="sxs-lookup"><span data-stu-id="62392-139">Relationship</span></span> | <span data-ttu-id="62392-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="62392-140">Type</span></span>        | <span data-ttu-id="62392-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="62392-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="62392-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="62392-142">accessPackageResourceRole</span></span>|[<span data-ttu-id="62392-143">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="62392-143">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="62392-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="62392-144">Read-only.</span></span> <span data-ttu-id="62392-145">Anulável.</span><span class="sxs-lookup"><span data-stu-id="62392-145">Nullable.</span></span>|
|<span data-ttu-id="62392-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="62392-146">accessPackageResourceScope</span></span>|[<span data-ttu-id="62392-147">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="62392-147">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="62392-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="62392-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62392-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62392-150">JSON representation</span></span>

<span data-ttu-id="62392-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62392-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "accessPackageResourceRole": {
    "id": "String (identifier)",
     "displayName": "String",
     "originSystem": "String",
     "originId": "String"
  },
  "accessPackageResourceScope": {
     "id": "String (identifier)",
     "displayName": "String",
     "description": "String",
     "originId": "String (identifier)",
     "originSystem": "String"
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


