---
title: Tipo de recurso roleAssignment
description: O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b388c043a1903394b1525c10eda7e817f1f1fdf2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441598"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="2b8d9-106">Tipo de recurso roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2b8d9-106">roleAssignment resource type</span></span>

<span data-ttu-id="2b8d9-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b8d9-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b8d9-108">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b8d9-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b8d9-109">O recurso de Atribuição de Função.</span><span class="sxs-lookup"><span data-stu-id="2b8d9-109">The Role Assignment resource.</span></span> <span data-ttu-id="2b8d9-110">Atribuições de função unem uma definição de função a membros e escopos.</span><span class="sxs-lookup"><span data-stu-id="2b8d9-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="2b8d9-111">Pode haver uma ou mais atribuições de função por função.</span><span class="sxs-lookup"><span data-stu-id="2b8d9-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="2b8d9-112">Aplica-se às funções internas e personalizadas</span><span class="sxs-lookup"><span data-stu-id="2b8d9-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="2b8d9-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="2b8d9-113">Methods</span></span>
|<span data-ttu-id="2b8d9-114">Método</span><span class="sxs-lookup"><span data-stu-id="2b8d9-114">Method</span></span>|<span data-ttu-id="2b8d9-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2b8d9-115">Return Type</span></span>|<span data-ttu-id="2b8d9-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b8d9-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2b8d9-117">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="2b8d9-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="2b8d9-118">Conjunto [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2b8d9-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="2b8d9-119">Listar propriedades e relações de objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2b8d9-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="2b8d9-120">Obter roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2b8d9-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="2b8d9-121">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2b8d9-121">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="2b8d9-122">Ler propriedades e relações de objetos de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2b8d9-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="2b8d9-123">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2b8d9-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="2b8d9-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2b8d9-124">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="2b8d9-125">Criar um novo objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2b8d9-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="2b8d9-126">Excluir roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2b8d9-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="2b8d9-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b8d9-127">None</span></span>|<span data-ttu-id="2b8d9-128">Excluir [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2b8d9-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="2b8d9-129">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2b8d9-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="2b8d9-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="2b8d9-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="2b8d9-131">Atualizar as propriedades de um objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2b8d9-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2b8d9-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b8d9-132">Properties</span></span>
|<span data-ttu-id="2b8d9-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b8d9-133">Property</span></span>|<span data-ttu-id="2b8d9-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b8d9-134">Type</span></span>|<span data-ttu-id="2b8d9-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b8d9-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b8d9-136">id</span><span class="sxs-lookup"><span data-stu-id="2b8d9-136">id</span></span>|<span data-ttu-id="2b8d9-137">String</span><span class="sxs-lookup"><span data-stu-id="2b8d9-137">String</span></span>|<span data-ttu-id="2b8d9-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2b8d9-138">Key of the entity.</span></span> <span data-ttu-id="2b8d9-139">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="2b8d9-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="2b8d9-140">displayName</span><span class="sxs-lookup"><span data-stu-id="2b8d9-140">displayName</span></span>|<span data-ttu-id="2b8d9-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b8d9-141">String</span></span>|<span data-ttu-id="2b8d9-142">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="2b8d9-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="2b8d9-143">description</span><span class="sxs-lookup"><span data-stu-id="2b8d9-143">description</span></span>|<span data-ttu-id="2b8d9-144">String</span><span class="sxs-lookup"><span data-stu-id="2b8d9-144">String</span></span>|<span data-ttu-id="2b8d9-145">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="2b8d9-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="2b8d9-146">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="2b8d9-146">resourceScopes</span></span>|<span data-ttu-id="2b8d9-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b8d9-147">String collection</span></span>|<span data-ttu-id="2b8d9-148">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="2b8d9-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="2b8d9-149">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2b8d9-149">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b8d9-150">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="2b8d9-150">Relationships</span></span>
|<span data-ttu-id="2b8d9-151">Relação</span><span class="sxs-lookup"><span data-stu-id="2b8d9-151">Relationship</span></span>|<span data-ttu-id="2b8d9-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b8d9-152">Type</span></span>|<span data-ttu-id="2b8d9-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b8d9-153">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b8d9-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="2b8d9-154">roleDefinition</span></span>|[<span data-ttu-id="2b8d9-155">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="2b8d9-155">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="2b8d9-156">A definição de função da qual essa atribuição faz parte.</span><span class="sxs-lookup"><span data-stu-id="2b8d9-156">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b8d9-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b8d9-157">JSON Representation</span></span>
<span data-ttu-id="2b8d9-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b8d9-158">Here is a JSON representation of the resource.</span></span>
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







