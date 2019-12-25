---
title: tipo de recurso accessPackageResourceRoleScope
description: Um escopo de função de recurso de pacote do Access é uma referência a um escopo dentro de um recurso e uma função nesse recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4ee4ec63c9c2efb60850ee7915e62dc0e284f8ba
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870957"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="70941-103">tipo de recurso accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="70941-103">accessPackageResourceRoleScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70941-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um escopo de função de recurso de pacote de acesso é uma referência a um escopo dentro de um recurso e uma função nesse recurso para esse escopo.</span><span class="sxs-lookup"><span data-stu-id="70941-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource for that scope.</span></span>  <span data-ttu-id="70941-105">Um pacote de acesso terá escopos de função de recurso pacote de acesso para os recursos em seu catálogo que são relevantes para esse pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="70941-105">An access package will have access package resource role scopes for the resources in its catalog which are relevant to that access package.</span></span>  <span data-ttu-id="70941-106">Quando um assunto recebe uma atribuição de pacote do Access, o assunto será provisionado com a função nesse escopo de cada escopo de função de recurso de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="70941-106">When a subject receives an access package assignment, the subject will be provisioned with the role in that scope of each access package resource role scope.</span></span>

## <a name="methods"></a><span data-ttu-id="70941-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="70941-107">Methods</span></span>

| <span data-ttu-id="70941-108">Método</span><span class="sxs-lookup"><span data-stu-id="70941-108">Method</span></span>       | <span data-ttu-id="70941-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="70941-109">Return Type</span></span> | <span data-ttu-id="70941-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="70941-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="70941-111">Listar accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="70941-111">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="70941-112">coleção [accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="70941-112">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="70941-113">Recupere uma lista de objetos **accessPackageResourceRoleScope** para um pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="70941-113">Retrieve a list of **accessPackageResourceRoleScope** objects for an access package.</span></span> |
| [<span data-ttu-id="70941-114">Criar accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="70941-114">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | <span data-ttu-id="70941-115">Criar um novo objeto **accessPackageResourceRoleScope** para um pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="70941-115">Create a new **accessPackageResourceRoleScope** object for an access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="70941-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70941-116">Properties</span></span>

| <span data-ttu-id="70941-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70941-117">Property</span></span>     | <span data-ttu-id="70941-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="70941-118">Type</span></span>        | <span data-ttu-id="70941-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="70941-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="70941-120">createdBy</span><span class="sxs-lookup"><span data-stu-id="70941-120">createdBy</span></span>|<span data-ttu-id="70941-121">String</span><span class="sxs-lookup"><span data-stu-id="70941-121">String</span></span>|<span data-ttu-id="70941-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70941-122">Read-only.</span></span>|
|<span data-ttu-id="70941-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70941-123">createdDateTime</span></span>|<span data-ttu-id="70941-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70941-124">DateTimeOffset</span></span>|<span data-ttu-id="70941-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="70941-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="70941-127">id</span><span class="sxs-lookup"><span data-stu-id="70941-127">id</span></span>|<span data-ttu-id="70941-128">String</span><span class="sxs-lookup"><span data-stu-id="70941-128">String</span></span>| <span data-ttu-id="70941-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70941-129">Read-only.</span></span>|
|<span data-ttu-id="70941-130">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="70941-130">modifiedBy</span></span>|<span data-ttu-id="70941-131">String</span><span class="sxs-lookup"><span data-stu-id="70941-131">String</span></span>|<span data-ttu-id="70941-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70941-132">Read-only.</span></span>|
|<span data-ttu-id="70941-133">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70941-133">modifiedDateTime</span></span>|<span data-ttu-id="70941-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70941-134">DateTimeOffset</span></span>|<span data-ttu-id="70941-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="70941-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="70941-137">Relações</span><span class="sxs-lookup"><span data-stu-id="70941-137">Relationships</span></span>

| <span data-ttu-id="70941-138">Relação</span><span class="sxs-lookup"><span data-stu-id="70941-138">Relationship</span></span> | <span data-ttu-id="70941-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="70941-139">Type</span></span>        | <span data-ttu-id="70941-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="70941-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="70941-141">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="70941-141">accessPackageResourceRole</span></span>|[<span data-ttu-id="70941-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="70941-142">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="70941-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70941-143">Read-only.</span></span> <span data-ttu-id="70941-144">Anulável.</span><span class="sxs-lookup"><span data-stu-id="70941-144">Nullable.</span></span>|
|<span data-ttu-id="70941-145">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="70941-145">accessPackageResourceScope</span></span>|[<span data-ttu-id="70941-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="70941-146">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="70941-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="70941-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70941-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70941-149">JSON representation</span></span>

<span data-ttu-id="70941-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70941-150">The following is a JSON representation of the resource.</span></span>

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
