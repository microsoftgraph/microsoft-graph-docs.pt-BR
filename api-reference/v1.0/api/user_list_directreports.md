# <a name="list-directreports"></a><span data-ttu-id="4c7b4-101">Listar directReports</span><span class="sxs-lookup"><span data-stu-id="4c7b4-101">List directReports</span></span>

<span data-ttu-id="4c7b4-p101">Obtenha relatórios diretos do usuário. Retorna os usuários e contatos para quem este usuário está atribuído como gerente.</span><span class="sxs-lookup"><span data-stu-id="4c7b4-p101">Get user's direct reports. Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="4c7b4-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c7b4-104">Permissions</span></span>
<span data-ttu-id="4c7b4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4c7b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4c7b4-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c7b4-107">Permission type</span></span>      | <span data-ttu-id="4c7b4-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c7b4-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4c7b4-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c7b4-109">Delegated (work or school account)</span></span> | <span data-ttu-id="4c7b4-110">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4c7b4-110">One of the following scopes is required to execute this API: User.Read; User.ReadWrite; User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="4c7b4-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c7b4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c7b4-112">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c7b4-112">User.Read, User.ReadWrite</span></span>    | 
|<span data-ttu-id="4c7b4-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c7b4-113">Application</span></span> | <span data-ttu-id="4c7b4-114">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c7b4-114">One of the following scopes is required to execute this API: User.Read.All; User.ReadWrite.All; Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4c7b4-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c7b4-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4c7b4-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4c7b4-116">Optional query parameters</span></span>
<span data-ttu-id="4c7b4-117">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4c7b4-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4c7b4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c7b4-118">Request headers</span></span>
| <span data-ttu-id="4c7b4-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c7b4-119">Header</span></span>       | <span data-ttu-id="4c7b4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4c7b4-120">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="4c7b4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c7b4-121">Authorization</span></span>  | <span data-ttu-id="4c7b4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c7b4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4c7b4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c7b4-124">Content-Type</span></span>   | <span data-ttu-id="4c7b4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c7b4-125">application/json</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="4c7b4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c7b4-126">Request body</span></span>
<span data-ttu-id="4c7b4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c7b4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c7b4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c7b4-128">Response</span></span>

<span data-ttu-id="4c7b4-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c7b4-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c7b4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c7b4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c7b4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c7b4-131">Request</span></span>
<span data-ttu-id="4c7b4-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c7b4-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/directReports
```
##### <a name="response"></a><span data-ttu-id="4c7b4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c7b4-133">Response</span></span>
<span data-ttu-id="4c7b4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c7b4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->