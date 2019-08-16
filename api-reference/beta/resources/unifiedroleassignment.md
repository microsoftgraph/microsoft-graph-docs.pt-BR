---
title: tipo de recurso unifiedRoleAssignment
description: Uma atribuição de função é o vínculo entre uma definição de função e uma entidade de segurança em um escopo específico para o propósito de conceder acesso.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cfc0c00add243b98c852a00f0a4ab990c3ca5173
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437787"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="ff52e-103">tipo de recurso unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ff52e-103">unifiedRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff52e-104">Um unifiedRoleAssignment é usado para conceder acesso aos recursos.</span><span class="sxs-lookup"><span data-stu-id="ff52e-104">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="ff52e-105">Ele representa uma definição de função atribuída a uma entidade de segurança (normalmente um usuário) em um determinado escopo.</span><span class="sxs-lookup"><span data-stu-id="ff52e-105">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

## <a name="methods"></a><span data-ttu-id="ff52e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ff52e-106">Methods</span></span>

| <span data-ttu-id="ff52e-107">Método</span><span class="sxs-lookup"><span data-stu-id="ff52e-107">Method</span></span>       | <span data-ttu-id="ff52e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ff52e-108">Return Type</span></span> | <span data-ttu-id="ff52e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff52e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ff52e-110">Obter unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ff52e-110">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="ff52e-111">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ff52e-111">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="ff52e-112">Leia as propriedades e os relacionamentos do objeto unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="ff52e-112">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="ff52e-113">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ff52e-113">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="ff52e-114">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ff52e-114">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="ff52e-115">Crie um novo unifiedRoleAssignment postando na coleção roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="ff52e-115">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="ff52e-116">Delete</span><span class="sxs-lookup"><span data-stu-id="ff52e-116">Delete</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="ff52e-117">None</span><span class="sxs-lookup"><span data-stu-id="ff52e-117">None</span></span> | <span data-ttu-id="ff52e-118">Exclua o objeto unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="ff52e-118">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ff52e-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff52e-119">Properties</span></span>

| <span data-ttu-id="ff52e-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff52e-120">Property</span></span>     | <span data-ttu-id="ff52e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff52e-121">Type</span></span>        | <span data-ttu-id="ff52e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff52e-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff52e-123">id</span><span class="sxs-lookup"><span data-stu-id="ff52e-123">id</span></span>|<span data-ttu-id="ff52e-124">String</span><span class="sxs-lookup"><span data-stu-id="ff52e-124">String</span></span>| <span data-ttu-id="ff52e-125">O identificador exclusivo para o unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="ff52e-125">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="ff52e-126">Chave, não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff52e-126">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="ff52e-127">principalId</span><span class="sxs-lookup"><span data-stu-id="ff52e-127">principalId</span></span>|<span data-ttu-id="ff52e-128">String</span><span class="sxs-lookup"><span data-stu-id="ff52e-128">String</span></span>| <span data-ttu-id="ff52e-129">ObjectID da entidade de segurança para a qual a atribuição é concedida.</span><span class="sxs-lookup"><span data-stu-id="ff52e-129">Objectid of the principal to which the assignment is granted.</span></span> |
|<span data-ttu-id="ff52e-130">resourceScope</span><span class="sxs-lookup"><span data-stu-id="ff52e-130">resourceScope</span></span>|<span data-ttu-id="ff52e-131">String</span><span class="sxs-lookup"><span data-stu-id="ff52e-131">String</span></span>| <span data-ttu-id="ff52e-132">O escopo no qual o unifiedRoleAssignment se aplica.</span><span class="sxs-lookup"><span data-stu-id="ff52e-132">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="ff52e-133">Isso é "/" para todo o serviço.</span><span class="sxs-lookup"><span data-stu-id="ff52e-133">This is "/" for service-wide.</span></span> |
|<span data-ttu-id="ff52e-134">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ff52e-134">roleDefinitionId</span></span>|<span data-ttu-id="ff52e-135">String</span><span class="sxs-lookup"><span data-stu-id="ff52e-135">String</span></span>| <span data-ttu-id="ff52e-136">O unifiedRoleDefinition para o qual a atribuição é.</span><span class="sxs-lookup"><span data-stu-id="ff52e-136">The unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="ff52e-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff52e-137">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ff52e-138">Relações</span><span class="sxs-lookup"><span data-stu-id="ff52e-138">Relationships</span></span>

<span data-ttu-id="ff52e-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff52e-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff52e-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff52e-140">JSON representation</span></span>

<span data-ttu-id="ff52e-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff52e-141">The following is a JSON representation of the resource.</span></span>

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
