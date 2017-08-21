# <a name="list-contacts"></a><span data-ttu-id="24e73-101">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="24e73-101">List contacts</span></span>

<span data-ttu-id="24e73-102">Obtenha uma coleção de contatos da pasta de contatos padrão do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="24e73-102">Get a contact collection from the default Contacts folder of the signed-in user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="24e73-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="24e73-103">Prerequisites</span></span>
<span data-ttu-id="24e73-104">Um dos seguintes **escopos** é necessário para executar esta API: *Contacts.Read; Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="24e73-104">One of the following scopes is required to execute this API: Contacts.Read; Contacts.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="24e73-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24e73-105">HTTP request</span></span>

<span data-ttu-id="24e73-106">Para obter todos os contatos na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="24e73-106">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="24e73-107">Para obter os contatos em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="24e73-107">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="24e73-108">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24e73-108">Optional query parameters</span></span>
<span data-ttu-id="24e73-109">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="24e73-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="24e73-110">Por exemplo, você pode usar o parâmetro de consulta `$filter` para filtrar os contatos com base no domínio dos endereços de email deles:</span><span class="sxs-lookup"><span data-stu-id="24e73-110">For example, you can use the `$filter` query parameter to filter contacts based on the domain of their email addresses:</span></span>

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a><span data-ttu-id="24e73-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24e73-111">Request headers</span></span>
| <span data-ttu-id="24e73-112">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24e73-112">Header</span></span>       | <span data-ttu-id="24e73-113">Valor</span><span class="sxs-lookup"><span data-stu-id="24e73-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="24e73-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="24e73-114">Authorization</span></span>  | <span data-ttu-id="24e73-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24e73-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="24e73-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24e73-117">Content-Type</span></span>   | <span data-ttu-id="24e73-118">application/json</span><span class="sxs-lookup"><span data-stu-id="24e73-118">application/json</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="24e73-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24e73-119">Request body</span></span>
<span data-ttu-id="24e73-120">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24e73-120">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24e73-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="24e73-121">Response</span></span>

<span data-ttu-id="24e73-122">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24e73-122">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="24e73-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24e73-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24e73-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24e73-124">Request</span></span>
<span data-ttu-id="24e73-125">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24e73-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="24e73-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="24e73-126">Response</span></span>
<span data-ttu-id="24e73-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24e73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
