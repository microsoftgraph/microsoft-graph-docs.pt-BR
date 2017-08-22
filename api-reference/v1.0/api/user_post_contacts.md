# <a name="create-contact"></a><span data-ttu-id="38d57-101">Criar contato</span><span class="sxs-lookup"><span data-stu-id="38d57-101">Create Contact</span></span>

<span data-ttu-id="38d57-102">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de contatos de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="38d57-102">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38d57-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38d57-103">Prerequisites</span></span>
<span data-ttu-id="38d57-104">Um dos seguintes **escopos** é necessário para executar esta API: *Contacts.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="38d57-104">One of the following **scopes** is required to execute this API: *Contacts.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="38d57-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38d57-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts
POST /me/contactFolders/{contactFolderId}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{contactFolderId}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="38d57-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38d57-106">Request headers</span></span>
| <span data-ttu-id="38d57-107">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38d57-107">Header</span></span>       | <span data-ttu-id="38d57-108">Valor</span><span class="sxs-lookup"><span data-stu-id="38d57-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="38d57-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="38d57-109">Authorization</span></span>  | <span data-ttu-id="38d57-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38d57-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="38d57-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38d57-112">Content-Type</span></span>  | <span data-ttu-id="38d57-113">application/json</span><span class="sxs-lookup"><span data-stu-id="38d57-113">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="38d57-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38d57-114">Request body</span></span>
<span data-ttu-id="38d57-115">No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="38d57-115">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="38d57-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="38d57-116">Response</span></span>

<span data-ttu-id="38d57-117">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38d57-117">If successful, this method returns `201, Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38d57-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38d57-118">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38d57-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38d57-119">Request</span></span>
<span data-ttu-id="38d57-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38d57-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contact_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contacts
Content-type: application/json

{
  "givenName": "Pavel",
  "surname": "Bansky",
  "emailAddresses": [
    {
      "address": "pavelb@fabrikam.onmicrosoft.com",
      "name": "Pavel Bansky"
    }
  ],
  "businessPhones": [
    "+1 732 555 0102"
  ]
}
```
<span data-ttu-id="38d57-121">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="38d57-121">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="38d57-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="38d57-122">Response</span></span>
<span data-ttu-id="38d57-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38d57-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "createdDateTime": "2015-11-09T02:14:32Z",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z",
   "displayName": "Pavel Bansky"
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
