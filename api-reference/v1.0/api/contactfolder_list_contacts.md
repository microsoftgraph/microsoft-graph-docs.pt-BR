# <a name="list-contacts"></a><span data-ttu-id="c4a61-101">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="c4a61-101">List contacts</span></span>

<span data-ttu-id="c4a61-102">Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.</span><span class="sxs-lookup"><span data-stu-id="c4a61-102">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c4a61-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4a61-103">Prerequisites</span></span>
<span data-ttu-id="c4a61-104">Um dos seguintes **escopos** é necessário para executar esta API: *Contacts.Read; Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="c4a61-104">One of the following scopes is required to execute this API: Contacts.Read; Contacts.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="c4a61-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4a61-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c4a61-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c4a61-106">Optional query parameters</span></span>
<span data-ttu-id="c4a61-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c4a61-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c4a61-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a61-108">Request headers</span></span>
| <span data-ttu-id="c4a61-109">Nome</span><span class="sxs-lookup"><span data-stu-id="c4a61-109">Name</span></span>       | <span data-ttu-id="c4a61-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4a61-110">Type</span></span> | <span data-ttu-id="c4a61-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4a61-111">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c4a61-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4a61-112">Authorization</span></span>  | <span data-ttu-id="c4a61-113">string</span><span class="sxs-lookup"><span data-stu-id="c4a61-113">string</span></span>  | <span data-ttu-id="c4a61-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4a61-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4a61-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a61-116">Request body</span></span>
<span data-ttu-id="c4a61-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4a61-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4a61-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4a61-118">Response</span></span>

<span data-ttu-id="c4a61-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4a61-119">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c4a61-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4a61-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4a61-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4a61-121">Request</span></span>
<span data-ttu-id="c4a61-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4a61-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="c4a61-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4a61-123">Response</span></span>
<span data-ttu-id="c4a61-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4a61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
