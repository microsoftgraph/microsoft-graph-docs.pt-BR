# <a name="list-contacts"></a><span data-ttu-id="9122f-101">Listar contatos</span><span class="sxs-lookup"><span data-stu-id="9122f-101">List contacts</span></span>

<span data-ttu-id="9122f-102">Obtém uma coleção de contatos da pasta de contatos padrão do usuário conectado (`.../me/contacts`), ou da pasta contato especificada.</span><span class="sxs-lookup"><span data-stu-id="9122f-102">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="9122f-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="9122f-103">Permissions</span></span>
<span data-ttu-id="9122f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9122f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9122f-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9122f-106">Permission type</span></span>      | <span data-ttu-id="9122f-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9122f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9122f-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9122f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9122f-109">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9122f-109">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9122f-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9122f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9122f-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9122f-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9122f-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9122f-112">Application</span></span> | <span data-ttu-id="9122f-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9122f-113">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9122f-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9122f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9122f-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9122f-115">Optional query parameters</span></span>
<span data-ttu-id="9122f-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9122f-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9122f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9122f-117">Request headers</span></span>
| <span data-ttu-id="9122f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9122f-118">Name</span></span>       | <span data-ttu-id="9122f-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9122f-119">Type</span></span> | <span data-ttu-id="9122f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9122f-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9122f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9122f-121">Authorization</span></span>  | <span data-ttu-id="9122f-122">string</span><span class="sxs-lookup"><span data-stu-id="9122f-122">string</span></span>  | <span data-ttu-id="9122f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9122f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9122f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9122f-125">Request body</span></span>
<span data-ttu-id="9122f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9122f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9122f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9122f-127">Response</span></span>

<span data-ttu-id="9122f-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9122f-128">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9122f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9122f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9122f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9122f-130">Request</span></span>
<span data-ttu-id="9122f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9122f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="9122f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9122f-132">Response</span></span>
<span data-ttu-id="9122f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9122f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
