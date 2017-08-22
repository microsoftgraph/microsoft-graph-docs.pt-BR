# <a name="get-contactfolder"></a><span data-ttu-id="1c6da-101">Obter contactFolder</span><span class="sxs-lookup"><span data-stu-id="1c6da-101">Get contactFolder</span></span>

<span data-ttu-id="1c6da-102">Obtém uma pasta de contatos usando a ID respectiva.</span><span class="sxs-lookup"><span data-stu-id="1c6da-102">Get a contact folder by using the contact folder ID.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c6da-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c6da-103">Prerequisites</span></span>
<span data-ttu-id="1c6da-104">Um dos seguintes **escopos** é necessário para executar esta API: *Contacts.ReadWrite; Contacts.Read*</span><span class="sxs-lookup"><span data-stu-id="1c6da-104">One of the following **scopes** is required to execute this API: *Contacts.ReadWrite; Contacts.Read*</span></span>
## <a name="http-request"></a><span data-ttu-id="1c6da-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c6da-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1c6da-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c6da-106">Optional query parameters</span></span>
<span data-ttu-id="1c6da-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c6da-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1c6da-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c6da-108">Request headers</span></span>
| <span data-ttu-id="1c6da-109">Nome</span><span class="sxs-lookup"><span data-stu-id="1c6da-109">Name</span></span>       | <span data-ttu-id="1c6da-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c6da-110">Type</span></span> | <span data-ttu-id="1c6da-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c6da-111">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1c6da-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c6da-112">Authorization</span></span>  | <span data-ttu-id="1c6da-113">string</span><span class="sxs-lookup"><span data-stu-id="1c6da-113">string</span></span>  | <span data-ttu-id="1c6da-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c6da-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c6da-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c6da-116">Request body</span></span>
<span data-ttu-id="1c6da-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c6da-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c6da-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c6da-118">Response</span></span>

<span data-ttu-id="1c6da-119">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [contactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c6da-119">If successful, this method returns a `200 OK` response code and [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c6da-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c6da-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c6da-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c6da-121">Request</span></span>
<span data-ttu-id="1c6da-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c6da-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="1c6da-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c6da-123">Response</span></span>
<span data-ttu-id="1c6da-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c6da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "displayName": "Finance",
  "id": "AAMkAGI2TKI5AAA=",
  "parentFolderId": "AAMkAGI2AAEOAAA="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
