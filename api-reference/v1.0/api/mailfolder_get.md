# <a name="get-mailfolder"></a><span data-ttu-id="13e95-101">Obter mailFolder</span><span class="sxs-lookup"><span data-stu-id="13e95-101">Get mailFolder</span></span>

<span data-ttu-id="13e95-102">Recupere as propriedades e os relacionamentos do objeto mailfolder.</span><span class="sxs-lookup"><span data-stu-id="13e95-102">Retrieve the properties and relationships of mailfolder object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="13e95-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="13e95-103">Prerequisites</span></span>
<span data-ttu-id="13e95-104">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.Read; Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="13e95-104">One of the following scopes is required to execute this API: Mail.Read; Mail.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="13e95-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13e95-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="13e95-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="13e95-106">Optional query parameters</span></span>
<span data-ttu-id="13e95-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="13e95-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="13e95-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13e95-108">Request headers</span></span>
| <span data-ttu-id="13e95-109">Nome</span><span class="sxs-lookup"><span data-stu-id="13e95-109">Name</span></span>       | <span data-ttu-id="13e95-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="13e95-110">Type</span></span> | <span data-ttu-id="13e95-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="13e95-111">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="13e95-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="13e95-112">Authorization</span></span>  | <span data-ttu-id="13e95-113">string</span><span class="sxs-lookup"><span data-stu-id="13e95-113">string</span></span>  | <span data-ttu-id="13e95-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13e95-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13e95-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13e95-116">Request body</span></span>
<span data-ttu-id="13e95-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13e95-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13e95-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="13e95-118">Response</span></span>

<span data-ttu-id="13e95-119">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13e95-119">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="13e95-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="13e95-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13e95-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13e95-121">Request</span></span>
<span data-ttu-id="13e95-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="13e95-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="13e95-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="13e95-123">Response</span></span>
<span data-ttu-id="13e95-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13e95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
