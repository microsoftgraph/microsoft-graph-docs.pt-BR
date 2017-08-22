# <a name="check-member-groups"></a><span data-ttu-id="81ed2-101">Verificar grupos de membros</span><span class="sxs-lookup"><span data-stu-id="81ed2-101">Check member groups</span></span>

<span data-ttu-id="81ed2-p101">Verifica se há associação em uma lista de grupos especificada e retorna dessa lista os grupos dos quais o usuário, grupo ou objeto de diretório especificado é membro. Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="81ed2-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81ed2-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81ed2-104">Prerequisites</span></span>
<span data-ttu-id="81ed2-105">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="81ed2-105">The following **scopes** are required to execute this API:</span></span> 
- <span data-ttu-id="81ed2-106">_User.Read.All_ E _Group.Read.All_</span><span class="sxs-lookup"><span data-stu-id="81ed2-106">_User.Read.All_ AND _Group.Read.All_</span></span>
- <span data-ttu-id="81ed2-107">_Directory.Read.All_</span><span class="sxs-lookup"><span data-stu-id="81ed2-107">_Directory.Read.All_</span></span>

> <span data-ttu-id="81ed2-108">Observação: escopos de permissão são listados em ordem de privilégio menos necessário.</span><span class="sxs-lookup"><span data-stu-id="81ed2-108">Note: Permission scopes are listed in least privilege required order.</span></span>

## <a name="http-request"></a><span data-ttu-id="81ed2-109">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81ed2-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="81ed2-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81ed2-110">Request headers</span></span>
| <span data-ttu-id="81ed2-111">Nome</span><span class="sxs-lookup"><span data-stu-id="81ed2-111">Name</span></span>       | <span data-ttu-id="81ed2-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="81ed2-112">Type</span></span> | <span data-ttu-id="81ed2-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="81ed2-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="81ed2-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="81ed2-114">Authorization</span></span>  | <span data-ttu-id="81ed2-115">string</span><span class="sxs-lookup"><span data-stu-id="81ed2-115">string</span></span>  | <span data-ttu-id="81ed2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81ed2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81ed2-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81ed2-118">Content-Type</span></span>  | <span data-ttu-id="81ed2-119">application/json</span><span class="sxs-lookup"><span data-stu-id="81ed2-119">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="81ed2-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81ed2-120">Request body</span></span>
<span data-ttu-id="81ed2-121">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81ed2-121">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="81ed2-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="81ed2-122">Parameter</span></span>    | <span data-ttu-id="81ed2-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="81ed2-123">Type</span></span>   |<span data-ttu-id="81ed2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="81ed2-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81ed2-125">groupIds</span><span class="sxs-lookup"><span data-stu-id="81ed2-125">groupIds</span></span>|<span data-ttu-id="81ed2-126">String</span><span class="sxs-lookup"><span data-stu-id="81ed2-126">String</span></span>|<span data-ttu-id="81ed2-p103">Uma coleção que contém as IDs de objetos dos grupos em que se deve verificar a associação. Até 20 grupos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="81ed2-p103">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="81ed2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="81ed2-129">Response</span></span>

<span data-ttu-id="81ed2-130">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81ed2-130">If successful, this method returns `200, OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81ed2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81ed2-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="81ed2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81ed2-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="81ed2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="81ed2-133">Response</span></span>
<span data-ttu-id="81ed2-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81ed2-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
