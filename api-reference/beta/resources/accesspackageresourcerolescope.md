---
title: Tipo de recurso accessPackageResourceRoleScope
description: Um escopo de função de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso e a uma função nesse recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8fa3e0a20646f2acf72d26d31c20bac674e751cd
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720946"
---
# <a name="accesspackageresourcerolescope-resource-type"></a><span data-ttu-id="a4a6c-103">Tipo de recurso accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="a4a6c-103">accessPackageResourceRoleScope resource type</span></span>

<span data-ttu-id="a4a6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4a6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4a6c-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)um escopo de função de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso e uma função nesse recurso para esse escopo.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource role scope is a reference to both a scope within a resource, and a role in that resource for that scope.</span></span>  <span data-ttu-id="a4a6c-106">Um pacote de acesso terá escopos de função de recurso de pacote de acesso para os recursos em seu catálogo que são relevantes para esse pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-106">An access package will have access package resource role scopes for the resources in its catalog which are relevant to that access package.</span></span>  <span data-ttu-id="a4a6c-107">Quando um assunto recebe uma atribuição de pacote de acesso, o assunto será provisionado com a função nesse escopo de cada escopo de função de recurso do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-107">When a subject receives an access package assignment, the subject will be provisioned with the role in that scope of each access package resource role scope.</span></span>

## <a name="methods"></a><span data-ttu-id="a4a6c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a4a6c-108">Methods</span></span>

| <span data-ttu-id="a4a6c-109">Método</span><span class="sxs-lookup"><span data-stu-id="a4a6c-109">Method</span></span>       | <span data-ttu-id="a4a6c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a4a6c-110">Return Type</span></span> | <span data-ttu-id="a4a6c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4a6c-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a4a6c-112">Listar accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="a4a6c-112">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="a4a6c-113">[Coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="a4a6c-113">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="a4a6c-114">Recupere uma lista de **objetos accessPackageResourceRoleScope** para um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-114">Retrieve a list of **accessPackageResourceRoleScope** objects for an access package.</span></span> |
| [<span data-ttu-id="a4a6c-115">Criar accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="a4a6c-115">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | <span data-ttu-id="a4a6c-116">Crie um novo **objeto accessPackageResourceRoleScope** para um pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-116">Create a new **accessPackageResourceRoleScope** object for an access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="a4a6c-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4a6c-117">Properties</span></span>

| <span data-ttu-id="a4a6c-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4a6c-118">Property</span></span>     | <span data-ttu-id="a4a6c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4a6c-119">Type</span></span>        | <span data-ttu-id="a4a6c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4a6c-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a4a6c-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="a4a6c-121">createdBy</span></span>|<span data-ttu-id="a4a6c-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4a6c-122">String</span></span>|<span data-ttu-id="a4a6c-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-123">Read-only.</span></span>|
|<span data-ttu-id="a4a6c-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4a6c-124">createdDateTime</span></span>|<span data-ttu-id="a4a6c-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4a6c-125">DateTimeOffset</span></span>|<span data-ttu-id="a4a6c-126">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a4a6c-127">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="a4a6c-127">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="a4a6c-128">id</span><span class="sxs-lookup"><span data-stu-id="a4a6c-128">id</span></span>|<span data-ttu-id="a4a6c-129">String</span><span class="sxs-lookup"><span data-stu-id="a4a6c-129">String</span></span>| <span data-ttu-id="a4a6c-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-130">Read-only.</span></span>|
|<span data-ttu-id="a4a6c-131">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="a4a6c-131">modifiedBy</span></span>|<span data-ttu-id="a4a6c-132">String</span><span class="sxs-lookup"><span data-stu-id="a4a6c-132">String</span></span>|<span data-ttu-id="a4a6c-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-133">Read-only.</span></span>|
|<span data-ttu-id="a4a6c-134">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4a6c-134">modifiedDateTime</span></span>|<span data-ttu-id="a4a6c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4a6c-135">DateTimeOffset</span></span>|<span data-ttu-id="a4a6c-136">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a4a6c-137">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="a4a6c-137">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4a6c-138">Relações</span><span class="sxs-lookup"><span data-stu-id="a4a6c-138">Relationships</span></span>

| <span data-ttu-id="a4a6c-139">Relação</span><span class="sxs-lookup"><span data-stu-id="a4a6c-139">Relationship</span></span> | <span data-ttu-id="a4a6c-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4a6c-140">Type</span></span>        | <span data-ttu-id="a4a6c-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4a6c-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a4a6c-142">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="a4a6c-142">accessPackageResourceRole</span></span>|[<span data-ttu-id="a4a6c-143">accessPackageResourceRole</span><span class="sxs-lookup"><span data-stu-id="a4a6c-143">accessPackageResourceRole</span></span>](accesspackageresourcerole.md)| <span data-ttu-id="a4a6c-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-144">Read-only.</span></span> <span data-ttu-id="a4a6c-145">Anulável.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-145">Nullable.</span></span>|
|<span data-ttu-id="a4a6c-146">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="a4a6c-146">accessPackageResourceScope</span></span>|[<span data-ttu-id="a4a6c-147">accessPackageResourceScope</span><span class="sxs-lookup"><span data-stu-id="a4a6c-147">accessPackageResourceScope</span></span>](accesspackageresourcescope.md)| <span data-ttu-id="a4a6c-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4a6c-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4a6c-150">JSON representation</span></span>

<span data-ttu-id="a4a6c-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-151">The following is a JSON representation of the resource.</span></span>

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


