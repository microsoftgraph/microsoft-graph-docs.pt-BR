# <a name="list-contactfolders"></a><span data-ttu-id="9438b-101">Listar contactFolders</span><span class="sxs-lookup"><span data-stu-id="9438b-101">List contactFolders</span></span>

<span data-ttu-id="9438b-102">Obtenha a coleção de pasta de contatos na pasta de contatos padrão do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="9438b-102">Get the contact folder collection in the default Contacts folder of the signed-in user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9438b-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9438b-103">Prerequisites</span></span>
<span data-ttu-id="9438b-104">Um dos seguintes **escopos** é necessário para executar esta API: *Contacts.Read; Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="9438b-104">One of the following scopes is required to execute this API: Contacts.Read; Contacts.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="9438b-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9438b-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9438b-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9438b-106">Optional query parameters</span></span>
<span data-ttu-id="9438b-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9438b-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9438b-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9438b-108">Request headers</span></span>
| <span data-ttu-id="9438b-109">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9438b-109">Header</span></span>       | <span data-ttu-id="9438b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="9438b-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9438b-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="9438b-111">Authorization</span></span>  | <span data-ttu-id="9438b-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9438b-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9438b-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9438b-114">Content-Type</span></span>   | <span data-ttu-id="9438b-115">application/json</span><span class="sxs-lookup"><span data-stu-id="9438b-115">application/json</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="9438b-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9438b-116">Request body</span></span>
<span data-ttu-id="9438b-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9438b-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9438b-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="9438b-118">Response</span></span>

<span data-ttu-id="9438b-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9438b-119">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9438b-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9438b-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9438b-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9438b-121">Request</span></span>
<span data-ttu-id="9438b-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9438b-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders
```
##### <a name="response"></a><span data-ttu-id="9438b-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="9438b-123">Response</span></span>
<span data-ttu-id="9438b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9438b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
