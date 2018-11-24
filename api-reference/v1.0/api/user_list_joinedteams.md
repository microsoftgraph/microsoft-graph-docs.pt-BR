# <a name="list-joinedteams"></a><span data-ttu-id="c5d7f-101">Lista joinedTeams</span><span class="sxs-lookup"><span data-stu-id="c5d7f-101">List joinedTeams</span></span>



<span data-ttu-id="c5d7f-102">Obtenha as [equipes](../resources/team.md) no Microsoft Teams que o usuário é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="c5d7f-102">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="c5d7f-103">Permissions</span><span class="sxs-lookup"><span data-stu-id="c5d7f-103">Permissions</span></span>
<span data-ttu-id="c5d7f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5d7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c5d7f-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5d7f-106">Permission type</span></span>      | <span data-ttu-id="c5d7f-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5d7f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5d7f-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5d7f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c5d7f-109">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5d7f-109">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="c5d7f-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5d7f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5d7f-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5d7f-111">Not supported.</span></span>    |
|<span data-ttu-id="c5d7f-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5d7f-112">Application</span></span> | <span data-ttu-id="c5d7f-113">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5d7f-113">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="c5d7f-114">Com as permissões de usuário delegado essa operação só funciona para 'me' usuário.</span><span class="sxs-lookup"><span data-stu-id="c5d7f-114">With user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="c5d7f-115">Com as permissões de aplicativo, ele funciona para todos os usuários, especificando a id de usuário específico. ('me' alias não é suportado com permissões de aplicativo)</span><span class="sxs-lookup"><span data-stu-id="c5d7f-115">With application permissions, it works for all users by specifying  the specific user id. ('me' alias is not supported with application permissions)</span></span>

## <a name="http-request"></a><span data-ttu-id="c5d7f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5d7f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5d7f-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c5d7f-117">Optional query parameters</span></span>
<span data-ttu-id="c5d7f-118">Os [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) não são suportados no momento.</span><span class="sxs-lookup"><span data-stu-id="c5d7f-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5d7f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5d7f-119">Request headers</span></span>
| <span data-ttu-id="c5d7f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5d7f-120">Header</span></span>       | <span data-ttu-id="c5d7f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c5d7f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c5d7f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5d7f-122">Authorization</span></span>  | <span data-ttu-id="c5d7f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5d7f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c5d7f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5d7f-125">Accept</span></span>  | <span data-ttu-id="c5d7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5d7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5d7f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5d7f-127">Request body</span></span>
<span data-ttu-id="c5d7f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5d7f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5d7f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5d7f-129">Response</span></span>

<span data-ttu-id="c5d7f-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5d7f-130">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5d7f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5d7f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5d7f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5d7f-132">Request</span></span>
<span data-ttu-id="c5d7f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5d7f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/beta/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="c5d7f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5d7f-134">Response</span></span>
<span data-ttu-id="c5d7f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5d7f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="c5d7f-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="c5d7f-138">See also</span></span>
[<span data-ttu-id="c5d7f-139">Liste todas as equipes</span><span class="sxs-lookup"><span data-stu-id="c5d7f-139">List all teams</span></span>](../../../concepts/teams_list_all_teams.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
