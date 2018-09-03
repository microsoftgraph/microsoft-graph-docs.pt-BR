# <a name="check-member-groups"></a><span data-ttu-id="855ee-101">Verificar grupos de membros</span><span class="sxs-lookup"><span data-stu-id="855ee-101">Check member groups</span></span>

<span data-ttu-id="855ee-p101">Verifica se há associação em uma lista de grupos especificada e retorna dessa lista os grupos dos quais o usuário, grupo ou objeto de diretório especificado é membro. Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="855ee-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="855ee-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="855ee-104">Permissions</span></span>
<span data-ttu-id="855ee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="855ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="855ee-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="855ee-107">Permission type</span></span>      | <span data-ttu-id="855ee-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="855ee-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="855ee-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="855ee-109">Delegated (work or school account)</span></span> | <span data-ttu-id="855ee-110">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="855ee-110">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="855ee-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="855ee-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="855ee-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="855ee-112">Not supported.</span></span>    |
|<span data-ttu-id="855ee-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="855ee-113">Application</span></span> | <span data-ttu-id="855ee-114">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="855ee-114">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="855ee-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="855ee-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="855ee-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="855ee-116">Request headers</span></span>
| <span data-ttu-id="855ee-117">Nome</span><span class="sxs-lookup"><span data-stu-id="855ee-117">Name</span></span>       | <span data-ttu-id="855ee-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="855ee-118">Type</span></span> | <span data-ttu-id="855ee-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="855ee-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="855ee-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="855ee-120">Authorization</span></span>  | <span data-ttu-id="855ee-121">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="855ee-121">string</span></span>  | <span data-ttu-id="855ee-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="855ee-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="855ee-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="855ee-124">Content-Type</span></span>  | <span data-ttu-id="855ee-125">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="855ee-125">string</span></span> | <span data-ttu-id="855ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="855ee-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="855ee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="855ee-127">Request body</span></span>
<span data-ttu-id="855ee-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="855ee-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="855ee-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="855ee-129">Parameter</span></span>    | <span data-ttu-id="855ee-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="855ee-130">Type</span></span>   |<span data-ttu-id="855ee-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="855ee-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="855ee-132">groupIds</span><span class="sxs-lookup"><span data-stu-id="855ee-132">groupIds</span></span>|<span data-ttu-id="855ee-133">Conjunto de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="855ee-133">String collection</span></span>|<span data-ttu-id="855ee-p104">Uma coleção que contém as IDs de objetos dos grupos em que se deve verificar a associação. Até 20 grupos podem ser especificados.</span><span class="sxs-lookup"><span data-stu-id="855ee-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="855ee-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="855ee-136">Response</span></span>

<span data-ttu-id="855ee-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="855ee-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="855ee-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="855ee-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="855ee-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="855ee-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{id}/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="855ee-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="855ee-140">Response</span></span>
<span data-ttu-id="855ee-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="855ee-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
