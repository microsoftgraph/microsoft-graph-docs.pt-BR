---
title: Tipo de recurso unifiedRolePermission
description: Uma permissão de função de diretório é uma coleção de ações e condições de recursos permitidos.
localization_priority: Normal
author: sureshja
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6fc799fec39eaa209ac8e74b02743cf84e76a51a
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316474"
---
# <a name="unifiedrolepermission-resource-type"></a><span data-ttu-id="13e3e-103">Tipo de recurso unifiedRolePermission</span><span class="sxs-lookup"><span data-stu-id="13e3e-103">unifiedRolePermission resource type</span></span>

<span data-ttu-id="13e3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13e3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13e3e-105">Representa uma coleção de ações de recursos permitidas e as condições que devem ser atendidas para que a ação seja efetiva.</span><span class="sxs-lookup"><span data-stu-id="13e3e-105">Represents a collection of allowed resource actions and the conditions that must be met for the action to be effective.</span></span> <span data-ttu-id="13e3e-106">Ações de recurso são tarefas que podem ser executadas em um recurso.</span><span class="sxs-lookup"><span data-stu-id="13e3e-106">Resource actions are tasks that can be performed on a resource.</span></span> <span data-ttu-id="13e3e-107">Por exemplo, o recurso de aplicativo oferece suporte para criar, atualizar, excluir e redefinir ações de recurso de senha.</span><span class="sxs-lookup"><span data-stu-id="13e3e-107">For example, the application resource supports create, update, delete, and reset password resource actions.</span></span>

## <a name="properties"></a><span data-ttu-id="13e3e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13e3e-108">Properties</span></span>

| <span data-ttu-id="13e3e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13e3e-109">Property</span></span>     | <span data-ttu-id="13e3e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="13e3e-110">Type</span></span>        | <span data-ttu-id="13e3e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="13e3e-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13e3e-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="13e3e-112">allowedResourceActions</span></span>|<span data-ttu-id="13e3e-113">String collection</span><span class="sxs-lookup"><span data-stu-id="13e3e-113">String collection</span></span>| <span data-ttu-id="13e3e-114">Conjunto de tarefas que podem ser executadas em um recurso.</span><span class="sxs-lookup"><span data-stu-id="13e3e-114">Set of tasks that can be performed on a resource.</span></span> |
|<span data-ttu-id="13e3e-115">condition</span><span class="sxs-lookup"><span data-stu-id="13e3e-115">condition</span></span>|<span data-ttu-id="13e3e-116">String</span><span class="sxs-lookup"><span data-stu-id="13e3e-116">String</span></span>| <span data-ttu-id="13e3e-117">Restrições opcionais que devem ser atendidas para que a permissão seja efetiva.</span><span class="sxs-lookup"><span data-stu-id="13e3e-117">Optional constraints that must be met for the permission to be effective.</span></span> |

### <a name="allowedresourceactions-property"></a><span data-ttu-id="13e3e-118">Propriedade allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="13e3e-118">allowedResourceActions property</span></span>

<span data-ttu-id="13e3e-119">Veja a seguir o esquema para ações de recurso:</span><span class="sxs-lookup"><span data-stu-id="13e3e-119">The following is the schema for resource actions:</span></span> 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
<span data-ttu-id="13e3e-120">Por exemplo: `microsoft.directory/applications/credentials/update`.</span><span class="sxs-lookup"><span data-stu-id="13e3e-120">For example: `microsoft.directory/applications/credentials/update`.</span></span>  

- <span data-ttu-id="13e3e-121">Namespace - Os serviços que expõem a tarefa.</span><span class="sxs-lookup"><span data-stu-id="13e3e-121">Namespace - The services that exposes the task.</span></span> <span data-ttu-id="13e3e-122">Por exemplo, todas as tarefas Azure Active Directory usar o namespace microsoft.directory.</span><span class="sxs-lookup"><span data-stu-id="13e3e-122">For example, all tasks in Azure Active Directory use the namespace microsoft.directory.</span></span>  
- <span data-ttu-id="13e3e-123">Entidade - Os recursos lógicos ou componentes expostos pelo serviço no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="13e3e-123">Entity - The logical features or components exposed by the service in Microsoft Graph.</span></span> <span data-ttu-id="13e3e-124">Por exemplo, aplicativos, entidades de serviço ou grupos.</span><span class="sxs-lookup"><span data-stu-id="13e3e-124">For example, applications, service principals, or groups.</span></span>
- <span data-ttu-id="13e3e-125">PropertySet - As propriedades ou aspectos específicos da entidade para a qual o acesso está sendo concedido.</span><span class="sxs-lookup"><span data-stu-id="13e3e-125">PropertySet - The specific properties or aspects of the entity for which access is being granted.</span></span> <span data-ttu-id="13e3e-126">Por exemplo, concede a capacidade de ler a URL de resposta, a URL de logout e a propriedade de fluxo implícito no objeto `microsoft.directory/applications/authentication/read` **application** no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="13e3e-126">For example, `microsoft.directory/applications/authentication/read` grants the ability to read the reply URL, logout URL, and implicit flow property on the **application** object in Azure AD.</span></span> <span data-ttu-id="13e3e-127">Veja a seguir os nomes reservados para conjuntos de propriedades comuns:</span><span class="sxs-lookup"><span data-stu-id="13e3e-127">The following are reserved names for common property sets:</span></span>  
  - <span data-ttu-id="13e3e-128">allProperties - Designa todas as propriedades da entidade, incluindo propriedades privilegiadas.</span><span class="sxs-lookup"><span data-stu-id="13e3e-128">allProperties - Designates all properties of the entity, including privileged properties.</span></span> <span data-ttu-id="13e3e-129">Exemplos incluem `microsoft.directory/applications/allProperties/read` `microsoft.directory/applications/allProperties/update` e .</span><span class="sxs-lookup"><span data-stu-id="13e3e-129">Examples include `microsoft.directory/applications/allProperties/read` and `microsoft.directory/applications/allProperties/update`.</span></span>
  - <span data-ttu-id="13e3e-130">basic - designa propriedades comuns de leitura, mas exclui as privilegiadas.</span><span class="sxs-lookup"><span data-stu-id="13e3e-130">basic - Designates common read properties but excludes privileged ones.</span></span> <span data-ttu-id="13e3e-131">Por exemplo, `microsoft.directory/applications/basic/update` inclui a capacidade de atualizar propriedades padrão, como o nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="13e3e-131">For example, `microsoft.directory/applications/basic/update` includes the ability to update standard properties like display name.</span></span>
  - <span data-ttu-id="13e3e-132">standard - designa propriedades de atualização comuns, mas exclui as privilegiadas.</span><span class="sxs-lookup"><span data-stu-id="13e3e-132">standard - Designates common update properties but excludes privileged ones.</span></span> <span data-ttu-id="13e3e-133">Por exemplo, `microsoft.directory/applications/standard/read`.</span><span class="sxs-lookup"><span data-stu-id="13e3e-133">For example, `microsoft.directory/applications/standard/read`.</span></span>
- <span data-ttu-id="13e3e-134">Ações - As operações que estão sendo concedidas.</span><span class="sxs-lookup"><span data-stu-id="13e3e-134">Actions - The operations being granted.</span></span> <span data-ttu-id="13e3e-135">Na maioria das circunstâncias, as permissões devem ser expressas em termos de CRUD ou allTasks.</span><span class="sxs-lookup"><span data-stu-id="13e3e-135">In most circumstances, permissions should be expressed in terms of CRUD or allTasks.</span></span> <span data-ttu-id="13e3e-136">As ações incluem:</span><span class="sxs-lookup"><span data-stu-id="13e3e-136">Actions include:</span></span>
  - <span data-ttu-id="13e3e-137">Criar - A capacidade de criar uma nova instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="13e3e-137">Create - The ability to create a new instance of the entity.</span></span>
  - <span data-ttu-id="13e3e-138">Leitura - A capacidade de ler um determinado conjunto de propriedades (incluindo allProperties).</span><span class="sxs-lookup"><span data-stu-id="13e3e-138">Read - The ability to read a given property set (including allProperties).</span></span>
  - <span data-ttu-id="13e3e-139">Atualização - A capacidade de atualizar um determinado conjunto de propriedades (incluindo allProperties).</span><span class="sxs-lookup"><span data-stu-id="13e3e-139">Update - The ability to update a given property set (including allProperties).</span></span>
  - <span data-ttu-id="13e3e-140">Excluir - A capacidade de excluir uma determinada entidade.</span><span class="sxs-lookup"><span data-stu-id="13e3e-140">Delete - The ability to delete a given entity.</span></span>
  - <span data-ttu-id="13e3e-141">AllTasks - Representa todas as operações CRUD (criar, ler, atualizar e excluir).</span><span class="sxs-lookup"><span data-stu-id="13e3e-141">AllTasks - Represents all CRUD operations (create, read, update, and delete).</span></span> 

### <a name="condition-property"></a><span data-ttu-id="13e3e-142">propriedade condition</span><span class="sxs-lookup"><span data-stu-id="13e3e-142">condition property</span></span>
<span data-ttu-id="13e3e-143">As condições definem restrições que devem ser atendidas.</span><span class="sxs-lookup"><span data-stu-id="13e3e-143">Conditions define constraints that must be met.</span></span> <span data-ttu-id="13e3e-144">Por exemplo, um requisito de que a entidade seja um "proprietário" do destino.</span><span class="sxs-lookup"><span data-stu-id="13e3e-144">For example, a requirement that the principal be an "owner" of the target.</span></span> <span data-ttu-id="13e3e-145">Veja a seguir as condições com suporte:</span><span class="sxs-lookup"><span data-stu-id="13e3e-145">The following are the supported conditions:</span></span>

- <span data-ttu-id="13e3e-146">Self: "$ResourceIsSelf"</span><span class="sxs-lookup"><span data-stu-id="13e3e-146">Self: "$ResourceIsSelf"</span></span>
- <span data-ttu-id="13e3e-147">Proprietário: "$SubjectIsOwner"</span><span class="sxs-lookup"><span data-stu-id="13e3e-147">Owner: "$SubjectIsOwner"</span></span>

<span data-ttu-id="13e3e-148">A seguir, um exemplo de permissão de função com uma condição.</span><span class="sxs-lookup"><span data-stu-id="13e3e-148">The following is an example of a role permission with a condition.</span></span>

```json
"rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/basic/update",
                "microsoft.directory/applications/credentials/update"
            ],
            "condition":  "$SubjectIsOwner"
        }
    ]

```

## <a name="json-representation"></a><span data-ttu-id="13e3e-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13e3e-149">JSON representation</span></span>

<span data-ttu-id="13e3e-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13e3e-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRolePermission",
  "baseType": null
}-->

```json
{
  "allowedResourceActions": ["String"],
  "condition": "String"
}
```
## <a name="see-also"></a><span data-ttu-id="13e3e-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="13e3e-151">See also</span></span>

- <span data-ttu-id="13e3e-152">[Permissões de função de administrador no Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) - Para obter informações sobre permissões para funções de diretório integrados.</span><span class="sxs-lookup"><span data-stu-id="13e3e-152">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles) - For information about permissions for built-in directory roles.</span></span>
- <span data-ttu-id="13e3e-153">[Subtipos de](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) registro de aplicativo e permissões em Azure Active Directory - Para obter informações sobre permissões disponíveis para funções de diretório personalizadas.</span><span class="sxs-lookup"><span data-stu-id="13e3e-153">[Application registration subtypes and permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/roles-custom-available-permissions) -  For information about permissions that are available for custom directory roles.</span></span> 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
