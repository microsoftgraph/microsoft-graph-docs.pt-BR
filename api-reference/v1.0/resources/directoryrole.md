# <a name="directoryrole-resource-type"></a><span data-ttu-id="2cce9-101">tipo de recurso directoryRole</span><span class="sxs-lookup"><span data-stu-id="2cce9-101">directoryRole resource type</span></span>

<span data-ttu-id="2cce9-102">Representa uma função de diretório do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2cce9-102">Represents an Azure AD directory role.</span></span> <span data-ttu-id="2cce9-103">Funções de diretório do Windows Azure AD também são conhecidos como *funções de administrador*.</span><span class="sxs-lookup"><span data-stu-id="2cce9-103">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="2cce9-104">Para obter mais informações sobre as funções de diretório (administrador), consulte [Atribuindo funções de administrador no Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="2cce9-104">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="2cce9-105">Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder as permissões da função de destino.</span><span class="sxs-lookup"><span data-stu-id="2cce9-105">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="2cce9-106">Para ler uma função de diretório ou atualizar seus membros, ele deve primeiro ser ativado no inquilino.</span><span class="sxs-lookup"><span data-stu-id="2cce9-106">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="2cce9-107">Por padrão, apenas a função do diretório de administradores de empresa é ativada.</span><span class="sxs-lookup"><span data-stu-id="2cce9-107">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="2cce9-108">Para ativar a outras funções de diretório disponíveis que você enviar uma solicitação POST com a ID de [directoryRoleTemplate](directoryroletemplate.md) na qual a função de diretório se baseia.</span><span class="sxs-lookup"><span data-stu-id="2cce9-108">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="2cce9-109">Herda de [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="2cce9-109">Inherits from [directoryObject](directoryobject.md).</span></span>
<span data-ttu-id="2cce9-110">Esse recurso permite:</span><span class="sxs-lookup"><span data-stu-id="2cce9-110">This resource supports:</span></span>

- <span data-ttu-id="2cce9-111">Usar a [consulta delta](../../../concepts/delta_query_overview.md) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryrole_delta.md).</span><span class="sxs-lookup"><span data-stu-id="2cce9-111">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole_delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="2cce9-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="2cce9-112">Methods</span></span>

| <span data-ttu-id="2cce9-113">Método</span><span class="sxs-lookup"><span data-stu-id="2cce9-113">Method</span></span>       | <span data-ttu-id="2cce9-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2cce9-114">Return Type</span></span>  |<span data-ttu-id="2cce9-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cce9-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2cce9-116">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="2cce9-116">Get directoryRole</span></span>](../api/directoryrole_get.md) | [<span data-ttu-id="2cce9-117">directoryRole</span><span class="sxs-lookup"><span data-stu-id="2cce9-117">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="2cce9-118">Leia as propriedades e os relacionamentos do objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="2cce9-118">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="2cce9-119">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="2cce9-119">List directoryRoles</span></span>](../api/directoryrole_list.md) | <span data-ttu-id="2cce9-120">Coleção [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="2cce9-120">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="2cce9-121">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="2cce9-121">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="2cce9-122">Adicionar membro</span><span class="sxs-lookup"><span data-stu-id="2cce9-122">Add member</span></span>](../api/directoryrole_post_members.md) |[<span data-ttu-id="2cce9-123">directoryObject</span><span class="sxs-lookup"><span data-stu-id="2cce9-123">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="2cce9-124">Adicione um usuário à função de diretório postando na propriedade de navegação de membros.</span><span class="sxs-lookup"><span data-stu-id="2cce9-124">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="2cce9-125">Listar membros</span><span class="sxs-lookup"><span data-stu-id="2cce9-125">List members</span></span>](../api/directoryrole_list_members.md) |<span data-ttu-id="2cce9-126">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="2cce9-126">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="2cce9-127">Obtenha os usuários que são membros da função directory da propriedade de navegação members.</span><span class="sxs-lookup"><span data-stu-id="2cce9-127">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="2cce9-128">Remover um membro</span><span class="sxs-lookup"><span data-stu-id="2cce9-128">Remove a member</span></span>](../api/directoryrole_delete_member.md) |[<span data-ttu-id="2cce9-129">directoryObject</span><span class="sxs-lookup"><span data-stu-id="2cce9-129">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="2cce9-130">Remova um usuário da função de diretório.</span><span class="sxs-lookup"><span data-stu-id="2cce9-130">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="2cce9-131">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="2cce9-131">Activate directoryRole</span></span>](../api/directoryrole_post_directoryroles.md) |[<span data-ttu-id="2cce9-132">directoryRole</span><span class="sxs-lookup"><span data-stu-id="2cce9-132">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="2cce9-133">Ative uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="2cce9-133">Activate a directory role.</span></span>|
|[<span data-ttu-id="2cce9-134">delta</span><span class="sxs-lookup"><span data-stu-id="2cce9-134">delta</span></span>](../api/directoryrole_delta.md)|<span data-ttu-id="2cce9-135">Coleção directoryRole</span><span class="sxs-lookup"><span data-stu-id="2cce9-135">directoryRole collection</span></span>| <span data-ttu-id="2cce9-136">Obtenha as alterações incrementais para funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="2cce9-136">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="2cce9-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2cce9-137">Properties</span></span>
| <span data-ttu-id="2cce9-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2cce9-138">Property</span></span>   | <span data-ttu-id="2cce9-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cce9-139">Type</span></span> | <span data-ttu-id="2cce9-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cce9-140">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2cce9-141">description</span><span class="sxs-lookup"><span data-stu-id="2cce9-141">description</span></span>|<span data-ttu-id="2cce9-142">String</span><span class="sxs-lookup"><span data-stu-id="2cce9-142">String</span></span>|<span data-ttu-id="2cce9-p102">A descrição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2cce9-p102">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="2cce9-145">displayName</span><span class="sxs-lookup"><span data-stu-id="2cce9-145">displayName</span></span>|<span data-ttu-id="2cce9-146">String</span><span class="sxs-lookup"><span data-stu-id="2cce9-146">String</span></span>|<span data-ttu-id="2cce9-p103">O nome de exibição da função de diretório. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2cce9-p103">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="2cce9-149">id</span><span class="sxs-lookup"><span data-stu-id="2cce9-149">id</span></span>|<span data-ttu-id="2cce9-150">String</span><span class="sxs-lookup"><span data-stu-id="2cce9-150">String</span></span>|<span data-ttu-id="2cce9-p104">O identificador exclusivo da função de diretório. Herdado de [directoryObject](directoryobject.md). Chave, Não Anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="2cce9-p104">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="2cce9-154">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="2cce9-154">roleTemplateId</span></span>|<span data-ttu-id="2cce9-155">String</span><span class="sxs-lookup"><span data-stu-id="2cce9-155">String</span></span>| <span data-ttu-id="2cce9-p105">A **id** do [directoryRoleTemplate](directoryroletemplate.md) em que esta função se baseia. A propriedade deve ser especificada ao ativar uma função de diretório em um locatário com uma operação POST. Depois que a função directory tiver sido ativada, a propriedade será somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2cce9-p105">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2cce9-159">Relações</span><span class="sxs-lookup"><span data-stu-id="2cce9-159">Relationships</span></span>
| <span data-ttu-id="2cce9-160">Relação</span><span class="sxs-lookup"><span data-stu-id="2cce9-160">Relationship</span></span> | <span data-ttu-id="2cce9-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cce9-161">Type</span></span> |<span data-ttu-id="2cce9-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cce9-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2cce9-163">membros</span><span class="sxs-lookup"><span data-stu-id="2cce9-163">members</span></span>|<span data-ttu-id="2cce9-164">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="2cce9-164">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="2cce9-p106">Usuários que são membros desta função de diretório. Métodos HTTP: GET, POST, DELETE. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2cce9-p106">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2cce9-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2cce9-169">JSON representation</span></span>

<span data-ttu-id="2cce9-170">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2cce9-170">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
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
