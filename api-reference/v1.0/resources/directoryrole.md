# <a name="directoryrole-resource-type"></a><span data-ttu-id="0b794-101">tipo de recurso directoryRole</span><span class="sxs-lookup"><span data-stu-id="0b794-101">directoryRole resource type</span></span>

<span data-ttu-id="0b794-p101">Representa uma função do diretório do Azure AD. As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*. Para obter mais informações sobre funções de diretório (administrador), confira [Atribuindo funções de administrador no Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST com a ID do [directoryRoleTemplate](directoryroletemplate.md) no qual a função directory se baseia. Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="0b794-p101">Represents an Azure AD directory role. Azure AD directory roles are also known as *administrator roles*. For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0b794-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="0b794-110">Methods</span></span>

| <span data-ttu-id="0b794-111">Método</span><span class="sxs-lookup"><span data-stu-id="0b794-111">Method</span></span>       | <span data-ttu-id="0b794-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0b794-112">Return Type</span></span>  |<span data-ttu-id="0b794-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b794-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0b794-114">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="0b794-114">Get directoryRole</span></span>](../api/directoryrole_get.md) | [<span data-ttu-id="0b794-115">directoryRole</span><span class="sxs-lookup"><span data-stu-id="0b794-115">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="0b794-116">Leia as propriedades e os relacionamentos do objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="0b794-116">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="0b794-117">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="0b794-117">List directoryRoles</span></span>](../api/directoryrole_list.md) | <span data-ttu-id="0b794-118">Coleção [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="0b794-118">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="0b794-119">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="0b794-119">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="0b794-120">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="0b794-120">Add member</span></span>](../api/directoryrole_post_members.md) |[<span data-ttu-id="0b794-121">directoryObject</span><span class="sxs-lookup"><span data-stu-id="0b794-121">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="0b794-122">Adicione um usuário à função de diretório postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="0b794-122">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="0b794-123">Listar membros</span><span class="sxs-lookup"><span data-stu-id="0b794-123">List members</span></span>](../api/directoryrole_list_members.md) |<span data-ttu-id="0b794-124">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="0b794-124">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="0b794-125">Obtenha os usuários que são membros da função directory da propriedade de navegação members.</span><span class="sxs-lookup"><span data-stu-id="0b794-125">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="0b794-126">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="0b794-126">Remove a member</span></span>](../api/directoryrole_delete_member.md) |[<span data-ttu-id="0b794-127">directoryObject</span><span class="sxs-lookup"><span data-stu-id="0b794-127">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="0b794-128">Remova um usuário da função de diretório.</span><span class="sxs-lookup"><span data-stu-id="0b794-128">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="0b794-129">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="0b794-129">Activate directoryRole</span></span>](../api/directoryrole_post_directoryroles.md) |[<span data-ttu-id="0b794-130">directoryRole</span><span class="sxs-lookup"><span data-stu-id="0b794-130">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="0b794-131">Ative uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="0b794-131">Activate a directory role.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b794-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b794-132">Properties</span></span>
| <span data-ttu-id="0b794-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b794-133">Property</span></span>   | <span data-ttu-id="0b794-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b794-134">Type</span></span> | <span data-ttu-id="0b794-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b794-135">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0b794-136">description</span><span class="sxs-lookup"><span data-stu-id="0b794-136">description</span></span>|<span data-ttu-id="0b794-137">String</span><span class="sxs-lookup"><span data-stu-id="0b794-137">String</span></span>|<span data-ttu-id="0b794-p102">A descrição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b794-p102">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="0b794-140">displayName</span><span class="sxs-lookup"><span data-stu-id="0b794-140">displayName</span></span>|<span data-ttu-id="0b794-141">String</span><span class="sxs-lookup"><span data-stu-id="0b794-141">String</span></span>|<span data-ttu-id="0b794-p103">O nome de exibição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b794-p103">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="0b794-144">id</span><span class="sxs-lookup"><span data-stu-id="0b794-144">id</span></span>|<span data-ttu-id="0b794-145">String</span><span class="sxs-lookup"><span data-stu-id="0b794-145">String</span></span>|<span data-ttu-id="0b794-p104">O identificador exclusivo da função de diretório. Herdado de [directoryObject](directoryobject.md). Chave, Não Anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="0b794-p104">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="0b794-149">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="0b794-149">roleTemplateId</span></span>|<span data-ttu-id="0b794-150">String</span><span class="sxs-lookup"><span data-stu-id="0b794-150">String</span></span>| <span data-ttu-id="0b794-p105">A **id** do [directoryRoleTemplate](directoryroletemplate.md) em que esta função se baseia. A propriedade deve ser especificada ao ativar uma função de diretório em um locatário com uma operação POST. Depois que a função directory tiver sido ativada, a propriedade será somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b794-p105">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0b794-154">Relações</span><span class="sxs-lookup"><span data-stu-id="0b794-154">Relationships</span></span>
| <span data-ttu-id="0b794-155">Relação</span><span class="sxs-lookup"><span data-stu-id="0b794-155">Relationship</span></span> | <span data-ttu-id="0b794-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b794-156">Type</span></span> |<span data-ttu-id="0b794-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b794-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b794-158">membros</span><span class="sxs-lookup"><span data-stu-id="0b794-158">members</span></span>|<span data-ttu-id="0b794-159">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="0b794-159">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="0b794-p106">Usuários que são membros desta função de diretório. Métodos HTTP: GET, POST, DELETE. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0b794-p106">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b794-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b794-164">JSON representation</span></span>

<span data-ttu-id="0b794-165">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0b794-165">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
