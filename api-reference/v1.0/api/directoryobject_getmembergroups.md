# <a name="get-member-groups"></a><span data-ttu-id="46bce-101">Obter grupos de membros</span><span class="sxs-lookup"><span data-stu-id="46bce-101">Get member groups</span></span>

<span data-ttu-id="46bce-p101">Retorna todos os grupos dos quais o usuário, grupo ou objeto de diretório especificado é membro. Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="46bce-p101">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="46bce-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="46bce-104">Permissions</span></span>
<span data-ttu-id="46bce-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="46bce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="46bce-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46bce-107">Permission type</span></span>      | <span data-ttu-id="46bce-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46bce-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46bce-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46bce-109">Delegated (work or school account)</span></span> | <span data-ttu-id="46bce-110">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="46bce-110">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="46bce-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46bce-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46bce-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46bce-112">Not supported.</span></span>    |
|<span data-ttu-id="46bce-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46bce-113">Application</span></span> | <span data-ttu-id="46bce-114">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="46bce-114">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46bce-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46bce-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="46bce-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46bce-116">Request headers</span></span>
| <span data-ttu-id="46bce-117">Nome</span><span class="sxs-lookup"><span data-stu-id="46bce-117">Name</span></span>       | <span data-ttu-id="46bce-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="46bce-118">Type</span></span> | <span data-ttu-id="46bce-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="46bce-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46bce-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="46bce-120">Authorization</span></span>  | <span data-ttu-id="46bce-121">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="46bce-121">string</span></span>  | <span data-ttu-id="46bce-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46bce-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46bce-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46bce-124">Content-Type</span></span>   | <span data-ttu-id="46bce-125">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="46bce-125">string</span></span>  | <span data-ttu-id="46bce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46bce-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="46bce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46bce-127">Request body</span></span>
<span data-ttu-id="46bce-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46bce-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="46bce-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="46bce-129">Parameter</span></span>    | <span data-ttu-id="46bce-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="46bce-130">Type</span></span>   |<span data-ttu-id="46bce-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="46bce-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46bce-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="46bce-132">securityEnabledOnly</span></span>|<span data-ttu-id="46bce-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="46bce-133">Boolean</span></span>| <span data-ttu-id="46bce-p104">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="46bce-p104">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="46bce-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="46bce-136">Response</span></span>

<span data-ttu-id="46bce-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46bce-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46bce-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46bce-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="46bce-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46bce-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="46bce-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="46bce-140">Response</span></span>
<span data-ttu-id="46bce-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46bce-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
