---
title: Tipo de recurso roleAssignment
description: O recurso de Atribuição de Função. Atribuições de função unem uma definição de função a membros e escopos. Pode haver uma ou mais atribuições de função por função. Aplica-se às funções internas e personalizadas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: af1feaf16cbff0f915982a78a623647803efcd2f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751192"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="cf023-106">Tipo de recurso roleAssignment</span><span class="sxs-lookup"><span data-stu-id="cf023-106">roleAssignment resource type</span></span>

<span data-ttu-id="cf023-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf023-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf023-108">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf023-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf023-109">O recurso de Atribuição de Função.</span><span class="sxs-lookup"><span data-stu-id="cf023-109">The Role Assignment resource.</span></span> <span data-ttu-id="cf023-110">Atribuições de função unem uma definição de função a membros e escopos.</span><span class="sxs-lookup"><span data-stu-id="cf023-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="cf023-111">Pode haver uma ou mais atribuições de função por função.</span><span class="sxs-lookup"><span data-stu-id="cf023-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="cf023-112">Aplica-se às funções internas e personalizadas</span><span class="sxs-lookup"><span data-stu-id="cf023-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="cf023-113">Methods</span><span class="sxs-lookup"><span data-stu-id="cf023-113">Methods</span></span>
|<span data-ttu-id="cf023-114">Método</span><span class="sxs-lookup"><span data-stu-id="cf023-114">Method</span></span>|<span data-ttu-id="cf023-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cf023-115">Return Type</span></span>|<span data-ttu-id="cf023-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf023-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cf023-117">Listar roleAssignments</span><span class="sxs-lookup"><span data-stu-id="cf023-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="cf023-118">Conjunto [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cf023-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="cf023-119">Listar propriedades e relações de objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cf023-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="cf023-120">Obter roleAssignment</span><span class="sxs-lookup"><span data-stu-id="cf023-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="cf023-121">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="cf023-121">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="cf023-122">Ler propriedades e relações de objetos de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cf023-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="cf023-123">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="cf023-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="cf023-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="cf023-124">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="cf023-125">Criar um novo objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cf023-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="cf023-126">Excluir roleAssignment</span><span class="sxs-lookup"><span data-stu-id="cf023-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="cf023-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cf023-127">None</span></span>|<span data-ttu-id="cf023-128">Excluir [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cf023-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="cf023-129">Atualizar roleAssignment</span><span class="sxs-lookup"><span data-stu-id="cf023-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="cf023-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="cf023-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="cf023-131">Atualizar as propriedades de um objeto de [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cf023-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cf023-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf023-132">Properties</span></span>
|<span data-ttu-id="cf023-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf023-133">Property</span></span>|<span data-ttu-id="cf023-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf023-134">Type</span></span>|<span data-ttu-id="cf023-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf023-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf023-136">id</span><span class="sxs-lookup"><span data-stu-id="cf023-136">id</span></span>|<span data-ttu-id="cf023-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf023-137">String</span></span>|<span data-ttu-id="cf023-138">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cf023-138">Key of the entity.</span></span> <span data-ttu-id="cf023-139">É somente leitura e gerada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="cf023-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="cf023-140">displayName</span><span class="sxs-lookup"><span data-stu-id="cf023-140">displayName</span></span>|<span data-ttu-id="cf023-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf023-141">String</span></span>|<span data-ttu-id="cf023-142">O nome de exibição ou nome amigável da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="cf023-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="cf023-143">descrição</span><span class="sxs-lookup"><span data-stu-id="cf023-143">description</span></span>|<span data-ttu-id="cf023-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf023-144">String</span></span>|<span data-ttu-id="cf023-145">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="cf023-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="cf023-146">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="cf023-146">resourceScopes</span></span>|<span data-ttu-id="cf023-147">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf023-147">String collection</span></span>|<span data-ttu-id="cf023-148">Lista de IDs de grupos de segurança de membros de escopo da função.</span><span class="sxs-lookup"><span data-stu-id="cf023-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="cf023-149">Estas são as IDs do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cf023-149">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf023-150">Relações</span><span class="sxs-lookup"><span data-stu-id="cf023-150">Relationships</span></span>
|<span data-ttu-id="cf023-151">Relação</span><span class="sxs-lookup"><span data-stu-id="cf023-151">Relationship</span></span>|<span data-ttu-id="cf023-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf023-152">Type</span></span>|<span data-ttu-id="cf023-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf023-153">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf023-154">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="cf023-154">roleDefinition</span></span>|[<span data-ttu-id="cf023-155">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="cf023-155">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="cf023-156">A definição de função da qual essa atribuição faz parte.</span><span class="sxs-lookup"><span data-stu-id="cf023-156">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf023-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf023-157">JSON Representation</span></span>
<span data-ttu-id="cf023-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf023-158">Here is a JSON representation of the resource.</span></span>
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




