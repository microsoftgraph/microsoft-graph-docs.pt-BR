---
title: Tipo de recurso roleAssignment
description: O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32527fad8db54f865f054f04400897e51638e5c2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554034"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="06f15-106">Tipo de recurso roleAssignment</span><span class="sxs-lookup"><span data-stu-id="06f15-106">roleAssignment resource type</span></span>

> <span data-ttu-id="06f15-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06f15-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06f15-108">O recurso de Atribuição de Função.</span><span class="sxs-lookup"><span data-stu-id="06f15-108">The Role Assignment resource.</span></span> <span data-ttu-id="06f15-109">Atribuições de função unem uma definição de função a membros e escopos.</span><span class="sxs-lookup"><span data-stu-id="06f15-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="06f15-110">Pode haver uma ou mais atribuições de função por função.</span><span class="sxs-lookup"><span data-stu-id="06f15-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="06f15-111">Aplica-se às funções internas e personalizadas</span><span class="sxs-lookup"><span data-stu-id="06f15-111">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="06f15-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="06f15-112">Methods</span></span>
|<span data-ttu-id="06f15-113">Método</span><span class="sxs-lookup"><span data-stu-id="06f15-113">Method</span></span>|<span data-ttu-id="06f15-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="06f15-114">Return Type</span></span>|<span data-ttu-id="06f15-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="06f15-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="06f15-116">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="06f15-116">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="06f15-117">Conjunto [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="06f15-117">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="06f15-118">Listar propriedades e relações de objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="06f15-118">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="06f15-119">Obter roleAssignment</span><span class="sxs-lookup"><span data-stu-id="06f15-119">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="06f15-120">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="06f15-120">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="06f15-121">Ler propriedades e relações de objetos de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="06f15-121">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="06f15-122">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="06f15-122">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="06f15-123">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="06f15-123">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="06f15-124">Criar um novo objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="06f15-124">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="06f15-125">Excluir roleAssignment</span><span class="sxs-lookup"><span data-stu-id="06f15-125">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="06f15-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="06f15-126">None</span></span>|<span data-ttu-id="06f15-127">Excluir [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="06f15-127">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="06f15-128">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="06f15-128">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="06f15-129">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="06f15-129">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="06f15-130">Atualizar as propriedades de um objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="06f15-130">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="06f15-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06f15-131">Properties</span></span>
|<span data-ttu-id="06f15-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06f15-132">Property</span></span>|<span data-ttu-id="06f15-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="06f15-133">Type</span></span>|<span data-ttu-id="06f15-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="06f15-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06f15-135">id</span><span class="sxs-lookup"><span data-stu-id="06f15-135">id</span></span>|<span data-ttu-id="06f15-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06f15-136">String</span></span>|<span data-ttu-id="06f15-137">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06f15-137">Key of the entity.</span></span> <span data-ttu-id="06f15-138">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="06f15-138">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="06f15-139">displayName</span><span class="sxs-lookup"><span data-stu-id="06f15-139">displayName</span></span>|<span data-ttu-id="06f15-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06f15-140">String</span></span>|<span data-ttu-id="06f15-141">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="06f15-141">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="06f15-142">description</span><span class="sxs-lookup"><span data-stu-id="06f15-142">description</span></span>|<span data-ttu-id="06f15-143">String</span><span class="sxs-lookup"><span data-stu-id="06f15-143">String</span></span>|<span data-ttu-id="06f15-144">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="06f15-144">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="06f15-145">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="06f15-145">resourceScopes</span></span>|<span data-ttu-id="06f15-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="06f15-146">String collection</span></span>|<span data-ttu-id="06f15-147">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="06f15-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="06f15-148">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="06f15-148">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06f15-149">Relações</span><span class="sxs-lookup"><span data-stu-id="06f15-149">Relationships</span></span>
|<span data-ttu-id="06f15-150">Relação</span><span class="sxs-lookup"><span data-stu-id="06f15-150">Relationship</span></span>|<span data-ttu-id="06f15-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="06f15-151">Type</span></span>|<span data-ttu-id="06f15-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="06f15-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06f15-153">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="06f15-153">roleDefinition</span></span>|[<span data-ttu-id="06f15-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="06f15-154">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="06f15-155">A definição de função da qual essa atribuição faz parte.</span><span class="sxs-lookup"><span data-stu-id="06f15-155">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06f15-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06f15-156">JSON Representation</span></span>
<span data-ttu-id="06f15-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="06f15-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ]
}
```



