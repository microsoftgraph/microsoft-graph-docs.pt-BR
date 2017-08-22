# <a name="list-childfolders"></a><span data-ttu-id="085c9-101">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="085c9-101">List childFolders</span></span>

<span data-ttu-id="085c9-102">Obtém uma coleção de pastas filho sob a pasta de contatos especificada.</span><span class="sxs-lookup"><span data-stu-id="085c9-102">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="085c9-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="085c9-103">Prerequisites</span></span>
<span data-ttu-id="085c9-104">Um dos seguintes **escopos** é necessário para executar esta API: *Contacts.Read; Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="085c9-104">One of the following scopes is required to execute this API: Contacts.Read; Contacts.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="085c9-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="085c9-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="085c9-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="085c9-106">Optional query parameters</span></span>
<span data-ttu-id="085c9-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="085c9-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="085c9-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="085c9-108">Request headers</span></span>
| <span data-ttu-id="085c9-109">Nome</span><span class="sxs-lookup"><span data-stu-id="085c9-109">Name</span></span>       | <span data-ttu-id="085c9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="085c9-110">Type</span></span> | <span data-ttu-id="085c9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="085c9-111">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="085c9-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="085c9-112">Authorization</span></span>  | <span data-ttu-id="085c9-113">string</span><span class="sxs-lookup"><span data-stu-id="085c9-113">string</span></span>  | <span data-ttu-id="085c9-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="085c9-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="085c9-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="085c9-116">Request body</span></span>
<span data-ttu-id="085c9-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="085c9-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="085c9-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="085c9-118">Response</span></span>

<span data-ttu-id="085c9-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="085c9-119">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="085c9-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="085c9-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="085c9-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="085c9-121">Request</span></span>
<span data-ttu-id="085c9-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="085c9-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="085c9-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="085c9-123">Response</span></span>
<span data-ttu-id="085c9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="085c9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
