# <a name="get-mailfolder"></a><span data-ttu-id="1c72b-101">Obter mailFolder</span><span class="sxs-lookup"><span data-stu-id="1c72b-101">Get mailFolder</span></span>

<span data-ttu-id="1c72b-102">Recuperar as propriedades e os relacionamentos do objeto mailfolder.</span><span class="sxs-lookup"><span data-stu-id="1c72b-102">Retrieve the properties and relationships of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c72b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c72b-103">Permissions</span></span>
<span data-ttu-id="1c72b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c72b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c72b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c72b-106">Permission type</span></span>      | <span data-ttu-id="1c72b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c72b-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="1c72b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c72b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1c72b-109">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c72b-109">Mail.Read, Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="1c72b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c72b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c72b-111">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c72b-111">Mail.Read, Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="1c72b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c72b-112">Application</span></span> | <span data-ttu-id="1c72b-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c72b-113">Mail.Read, Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1c72b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c72b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1c72b-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c72b-115">Optional query parameters</span></span>
<span data-ttu-id="1c72b-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c72b-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1c72b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c72b-117">Request headers</span></span>
| <span data-ttu-id="1c72b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1c72b-118">Name</span></span>       | <span data-ttu-id="1c72b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c72b-119">Type</span></span> | <span data-ttu-id="1c72b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c72b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1c72b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c72b-121">Authorization</span></span>  | <span data-ttu-id="1c72b-122">string</span><span class="sxs-lookup"><span data-stu-id="1c72b-122">string</span></span>  | <span data-ttu-id="1c72b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c72b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c72b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c72b-125">Request body</span></span>
<span data-ttu-id="1c72b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c72b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c72b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c72b-127">Response</span></span>

<span data-ttu-id="1c72b-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c72b-128">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c72b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c72b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c72b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c72b-130">Request</span></span>
<span data-ttu-id="1c72b-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c72b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="1c72b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c72b-132">Response</span></span>
<span data-ttu-id="1c72b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c72b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
