---
title: tipo de recurso unifiedRoleAssignment
description: Uma atribuição de função é o vínculo entre uma definição de função e uma entidade de segurança em um escopo específico para o propósito de conceder acesso.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c51c3cd7c706cf154db8c1de21c04aaa098c3efb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519614"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="2c8b4-103">tipo de recurso unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2c8b4-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="2c8b4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2c8b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c8b4-105">Um unifiedRoleAssignment é usado para conceder acesso aos recursos.</span><span class="sxs-lookup"><span data-stu-id="2c8b4-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="2c8b4-106">Ele representa uma definição de função atribuída a uma entidade de segurança (normalmente um usuário) em um determinado escopo.</span><span class="sxs-lookup"><span data-stu-id="2c8b4-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

## <a name="methods"></a><span data-ttu-id="2c8b4-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2c8b4-107">Methods</span></span>

| <span data-ttu-id="2c8b4-108">Método</span><span class="sxs-lookup"><span data-stu-id="2c8b4-108">Method</span></span>       | <span data-ttu-id="2c8b4-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2c8b4-109">Return Type</span></span> | <span data-ttu-id="2c8b4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c8b4-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2c8b4-111">Obter unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2c8b4-111">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="2c8b4-112">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2c8b4-112">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="2c8b4-113">Leia as propriedades e os relacionamentos do objeto unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="2c8b4-113">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="2c8b4-114">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2c8b4-114">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="2c8b4-115">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2c8b4-115">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="2c8b4-116">Crie um novo unifiedRoleAssignment postando na coleção roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="2c8b4-116">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="2c8b4-117">Delete</span><span class="sxs-lookup"><span data-stu-id="2c8b4-117">Delete</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="2c8b4-118">None</span><span class="sxs-lookup"><span data-stu-id="2c8b4-118">None</span></span> | <span data-ttu-id="2c8b4-119">Exclua o objeto unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="2c8b4-119">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2c8b4-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c8b4-120">Properties</span></span>

| <span data-ttu-id="2c8b4-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c8b4-121">Property</span></span>     | <span data-ttu-id="2c8b4-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c8b4-122">Type</span></span>        | <span data-ttu-id="2c8b4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c8b4-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2c8b4-124">id</span><span class="sxs-lookup"><span data-stu-id="2c8b4-124">id</span></span>|<span data-ttu-id="2c8b4-125">String</span><span class="sxs-lookup"><span data-stu-id="2c8b4-125">String</span></span>| <span data-ttu-id="2c8b4-126">O identificador exclusivo para o unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="2c8b4-126">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="2c8b4-127">Chave, não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c8b4-127">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="2c8b4-128">principalId</span><span class="sxs-lookup"><span data-stu-id="2c8b4-128">principalId</span></span>|<span data-ttu-id="2c8b4-129">String</span><span class="sxs-lookup"><span data-stu-id="2c8b4-129">String</span></span>| <span data-ttu-id="2c8b4-130">ObjectID da entidade de segurança para a qual a atribuição é concedida.</span><span class="sxs-lookup"><span data-stu-id="2c8b4-130">Objectid of the principal to which the assignment is granted.</span></span> |
|<span data-ttu-id="2c8b4-131">resourceScope</span><span class="sxs-lookup"><span data-stu-id="2c8b4-131">resourceScope</span></span>|<span data-ttu-id="2c8b4-132">String</span><span class="sxs-lookup"><span data-stu-id="2c8b4-132">String</span></span>| <span data-ttu-id="2c8b4-133">O escopo no qual o unifiedRoleAssignment se aplica.</span><span class="sxs-lookup"><span data-stu-id="2c8b4-133">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="2c8b4-134">Isso é "/" para todo o serviço.</span><span class="sxs-lookup"><span data-stu-id="2c8b4-134">This is "/" for service-wide.</span></span> |
|<span data-ttu-id="2c8b4-135">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="2c8b4-135">roleDefinitionId</span></span>|<span data-ttu-id="2c8b4-136">String</span><span class="sxs-lookup"><span data-stu-id="2c8b4-136">String</span></span>| <span data-ttu-id="2c8b4-137">O unifiedRoleDefinition para o qual a atribuição é.</span><span class="sxs-lookup"><span data-stu-id="2c8b4-137">The unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="2c8b4-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c8b4-138">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2c8b4-139">Relações</span><span class="sxs-lookup"><span data-stu-id="2c8b4-139">Relationships</span></span>

<span data-ttu-id="2c8b4-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c8b4-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c8b4-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c8b4-141">JSON representation</span></span>

<span data-ttu-id="2c8b4-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c8b4-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "principalId": "String",
  "resourceScope": "String",
  "roleDefinitionId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
