# <a name="get-member-groups"></a><span data-ttu-id="69209-101">Obter grupos de membros</span><span class="sxs-lookup"><span data-stu-id="69209-101">Get member groups</span></span>

<span data-ttu-id="69209-p101">Retorna todos os grupos dos quais o usuário, grupo ou objeto de diretório especificado é membro. Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="69209-p101">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69209-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69209-104">Prerequisites</span></span>
<span data-ttu-id="69209-105">Um dos seguintes **scopes** é necessário para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="69209-105">One of the following **scopes** are required to execute this API:</span></span> 
- <span data-ttu-id="69209-106">_User.Read.All_ E _Group.Read.All_</span><span class="sxs-lookup"><span data-stu-id="69209-106">_User.Read.All_ AND _Group.Read.All_</span></span>
- <span data-ttu-id="69209-107">_Directory.Read.All_</span><span class="sxs-lookup"><span data-stu-id="69209-107">_Directory.Read.All_</span></span>

> <span data-ttu-id="69209-108">Observação: escopos de permissão são listados em ordem de privilégio menos necessário.</span><span class="sxs-lookup"><span data-stu-id="69209-108">Note: Permission scopes are listed in least privilege required order.</span></span>

## <a name="http-request"></a><span data-ttu-id="69209-109">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69209-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="69209-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69209-110">Request headers</span></span>
| <span data-ttu-id="69209-111">Nome</span><span class="sxs-lookup"><span data-stu-id="69209-111">Name</span></span>       | <span data-ttu-id="69209-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="69209-112">Type</span></span> | <span data-ttu-id="69209-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="69209-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="69209-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="69209-114">Authorization</span></span>  | <span data-ttu-id="69209-115">string</span><span class="sxs-lookup"><span data-stu-id="69209-115">string</span></span>  | <span data-ttu-id="69209-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69209-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69209-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69209-118">Content-Type</span></span>  | <span data-ttu-id="69209-119">application/json</span><span class="sxs-lookup"><span data-stu-id="69209-119">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="69209-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69209-120">Request body</span></span>
<span data-ttu-id="69209-121">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69209-121">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="69209-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="69209-122">Parameter</span></span>    | <span data-ttu-id="69209-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="69209-123">Type</span></span>   |<span data-ttu-id="69209-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="69209-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69209-125">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="69209-125">securityEnabledOnly</span></span>|<span data-ttu-id="69209-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="69209-126">Boolean</span></span>| <span data-ttu-id="69209-p103">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="69209-p103">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="69209-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="69209-129">Response</span></span>

<span data-ttu-id="69209-130">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69209-130">If successful, this method returns `200, OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69209-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69209-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="69209-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69209-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="69209-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="69209-133">Response</span></span>
<span data-ttu-id="69209-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69209-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
