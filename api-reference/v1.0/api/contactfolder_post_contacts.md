# <a name="create-contact"></a><span data-ttu-id="df974-101">Criar contato</span><span class="sxs-lookup"><span data-stu-id="df974-101">Create Contact</span></span>

<span data-ttu-id="df974-102">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="df974-102">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df974-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df974-103">Prerequisites</span></span>
<span data-ttu-id="df974-104">Um dos seguintes **escopos** é necessário para executar esta API: *Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="df974-104">One of the following **scopes** is required to execute this API: *Contacts.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="df974-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df974-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="df974-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df974-106">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="df974-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df974-107">Request headers</span></span>
| <span data-ttu-id="df974-108">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df974-108">Header</span></span>       | <span data-ttu-id="df974-109">Valor</span><span class="sxs-lookup"><span data-stu-id="df974-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df974-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="df974-110">Authorization</span></span>  | <span data-ttu-id="df974-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df974-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="df974-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df974-113">Content-Type</span></span>  | <span data-ttu-id="df974-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df974-p102">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df974-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df974-116">Request body</span></span>
<span data-ttu-id="df974-117">No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="df974-117">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="df974-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="df974-118">Response</span></span>

<span data-ttu-id="df974-119">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df974-119">If successful, this method returns `201, Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df974-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df974-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df974-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df974-121">Request</span></span>
<span data-ttu-id="df974-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df974-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
<span data-ttu-id="df974-123">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="df974-123">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="df974-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="df974-124">Response</span></span>
<span data-ttu-id="df974-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df974-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->