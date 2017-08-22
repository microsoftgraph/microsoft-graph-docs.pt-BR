# <a name="get-member-objects"></a><span data-ttu-id="537b0-101">Obter objetos de membros</span><span class="sxs-lookup"><span data-stu-id="537b0-101">Get member objects</span></span>

 <span data-ttu-id="537b0-p101">Retorna todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="537b0-p101">Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.</span></span> 
 > <span data-ttu-id="537b0-104">Observação: Somente usuários podem ser membros de funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="537b0-104">Note: Only users can be members of directory roles.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="537b0-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="537b0-105">Prerequisites</span></span>
<span data-ttu-id="537b0-106">Um dos seguintes **scopes** é necessário para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="537b0-106">One of the following **scopes** are required to execute this API:</span></span>
- <span data-ttu-id="537b0-107">_User.Read.All_ E _Group.Read.All_</span><span class="sxs-lookup"><span data-stu-id="537b0-107">_User.Read.All_ AND _Group.Read.All_</span></span>
- <span data-ttu-id="537b0-108">_Directory.Read.All_</span><span class="sxs-lookup"><span data-stu-id="537b0-108">_Directory.Read.All_</span></span>

> <span data-ttu-id="537b0-109">Observação: escopos de permissão são listados em ordem de privilégio menos necessário.</span><span class="sxs-lookup"><span data-stu-id="537b0-109">Note: Permission scopes are listed in least privilege required order.</span></span>

## <a name="http-request"></a><span data-ttu-id="537b0-110">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="537b0-110">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="537b0-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="537b0-111">Request headers</span></span>
| <span data-ttu-id="537b0-112">Nome</span><span class="sxs-lookup"><span data-stu-id="537b0-112">Name</span></span>       | <span data-ttu-id="537b0-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="537b0-113">Type</span></span> | <span data-ttu-id="537b0-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="537b0-114">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="537b0-115">Autorização</span><span class="sxs-lookup"><span data-stu-id="537b0-115">Authorization</span></span>  | <span data-ttu-id="537b0-116">string</span><span class="sxs-lookup"><span data-stu-id="537b0-116">string</span></span>  | <span data-ttu-id="537b0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="537b0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="537b0-119">Content-Type</span><span class="sxs-lookup"><span data-stu-id="537b0-119">Content-Type</span></span>  | <span data-ttu-id="537b0-120">application/json</span><span class="sxs-lookup"><span data-stu-id="537b0-120">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="537b0-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="537b0-121">Request body</span></span>
<span data-ttu-id="537b0-122">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="537b0-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="537b0-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="537b0-123">Parameter</span></span>    | <span data-ttu-id="537b0-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="537b0-124">Type</span></span>   |<span data-ttu-id="537b0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="537b0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="537b0-126">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="537b0-126">securityEnabledOnly</span></span>|<span data-ttu-id="537b0-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="537b0-127">Boolean</span></span>| <span data-ttu-id="537b0-p103">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="537b0-p103">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="537b0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="537b0-130">Response</span></span>

<span data-ttu-id="537b0-131">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="537b0-131">If successful, this method returns `200, OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="537b0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="537b0-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="537b0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="537b0-133">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="537b0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="537b0-134">Response</span></span>
<span data-ttu-id="537b0-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="537b0-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
