# <a name="get-member-objects"></a><span data-ttu-id="a5ee8-101">Obter objetos de membros</span><span class="sxs-lookup"><span data-stu-id="a5ee8-101">Get member objects</span></span>

 <span data-ttu-id="a5ee8-p101">Retorna todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="a5ee8-p101">Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.</span></span> 
 > <span data-ttu-id="a5ee8-104">Observação: Somente usuários podem ser membros de funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="a5ee8-104">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5ee8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5ee8-105">Permissions</span></span>
<span data-ttu-id="a5ee8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5ee8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a5ee8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5ee8-108">Permission type</span></span>      | <span data-ttu-id="a5ee8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5ee8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5ee8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5ee8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a5ee8-111">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5ee8-111">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="a5ee8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5ee8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5ee8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5ee8-113">Not supported.</span></span>    |
|<span data-ttu-id="a5ee8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5ee8-114">Application</span></span> | <span data-ttu-id="a5ee8-115">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a5ee8-115">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5ee8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5ee8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="a5ee8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ee8-117">Request headers</span></span>
| <span data-ttu-id="a5ee8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a5ee8-118">Name</span></span>       | <span data-ttu-id="a5ee8-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5ee8-119">Type</span></span> | <span data-ttu-id="a5ee8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5ee8-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a5ee8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5ee8-121">Authorization</span></span>  | <span data-ttu-id="a5ee8-122">string</span><span class="sxs-lookup"><span data-stu-id="a5ee8-122">string</span></span>  | <span data-ttu-id="a5ee8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5ee8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a5ee8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5ee8-125">Content-Type</span></span>  | <span data-ttu-id="a5ee8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5ee8-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5ee8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ee8-127">Request body</span></span>
<span data-ttu-id="a5ee8-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5ee8-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a5ee8-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a5ee8-129">Parameter</span></span>    | <span data-ttu-id="a5ee8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5ee8-130">Type</span></span>   |<span data-ttu-id="a5ee8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5ee8-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5ee8-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a5ee8-132">securityEnabledOnly</span></span>|<span data-ttu-id="a5ee8-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5ee8-133">Boolean</span></span>| <span data-ttu-id="a5ee8-p104">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="a5ee8-p104">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="a5ee8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5ee8-136">Response</span></span>

<span data-ttu-id="a5ee8-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5ee8-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5ee8-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5ee8-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a5ee8-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ee8-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="a5ee8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5ee8-140">Response</span></span>
<span data-ttu-id="a5ee8-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5ee8-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
