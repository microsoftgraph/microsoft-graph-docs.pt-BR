# <a name="create-contact"></a><span data-ttu-id="ff156-101">Criar contato</span><span class="sxs-lookup"><span data-stu-id="ff156-101">Create Contact</span></span>

<span data-ttu-id="ff156-102">Adicione um contato na pasta de contatos raiz ou no ponto de extremidade de `contacts` de outra pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="ff156-102">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="ff156-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff156-103">Permissions</span></span>
<span data-ttu-id="ff156-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ff156-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ff156-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff156-106">Permission type</span></span>      | <span data-ttu-id="ff156-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff156-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="ff156-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff156-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ff156-109">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff156-109">Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="ff156-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff156-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff156-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff156-111">Contacts.ReadWrite</span></span>    | 
|<span data-ttu-id="ff156-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff156-112">Application</span></span> | <span data-ttu-id="ff156-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff156-113">Contacts.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ff156-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff156-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="ff156-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff156-115">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="ff156-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff156-116">Request headers</span></span>
| <span data-ttu-id="ff156-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff156-117">Header</span></span>       | <span data-ttu-id="ff156-118">Valor</span><span class="sxs-lookup"><span data-stu-id="ff156-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ff156-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff156-119">Authorization</span></span>  | <span data-ttu-id="ff156-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff156-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ff156-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ff156-122">Content-Type</span></span>  | <span data-ttu-id="ff156-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff156-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff156-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff156-125">Request body</span></span>
<span data-ttu-id="ff156-126">No corpo da solicitação, forneça uma representação JSON do objeto [Contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="ff156-126">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ff156-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff156-127">Response</span></span>

<span data-ttu-id="ff156-128">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff156-128">If successful, this method returns `201, Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff156-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff156-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff156-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff156-130">Request</span></span>
<span data-ttu-id="ff156-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff156-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="ff156-132">No corpo da solicitação, forneça uma representação JSON do objeto [contact](../resources/contact.md).</span><span class="sxs-lookup"><span data-stu-id="ff156-132">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ff156-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff156-133">Response</span></span>
<span data-ttu-id="ff156-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff156-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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