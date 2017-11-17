# <a name="list-contactfolders"></a><span data-ttu-id="66308-101">Listar contactFolders</span><span class="sxs-lookup"><span data-stu-id="66308-101">List contactFolders</span></span>

<span data-ttu-id="66308-102">Obtenha a coleção de pasta de contatos na pasta de contatos padrão do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="66308-102">Get the contact folder collection in the default Contacts folder of the signed-in user.</span></span>
## <a name="permissions"></a><span data-ttu-id="66308-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="66308-103">Permissions</span></span>
<span data-ttu-id="66308-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="66308-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="66308-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66308-106">Permission type</span></span>      | <span data-ttu-id="66308-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66308-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66308-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66308-108">Delegated (work or school account)</span></span> | <span data-ttu-id="66308-109">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66308-109">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="66308-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66308-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66308-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66308-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="66308-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66308-112">Application</span></span> | <span data-ttu-id="66308-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66308-113">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="66308-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66308-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="66308-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="66308-115">Optional query parameters</span></span>
<span data-ttu-id="66308-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="66308-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="66308-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66308-117">Request headers</span></span>
| <span data-ttu-id="66308-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="66308-118">Header</span></span>       | <span data-ttu-id="66308-119">Valor</span><span class="sxs-lookup"><span data-stu-id="66308-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="66308-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="66308-120">Authorization</span></span>  | <span data-ttu-id="66308-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66308-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="66308-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66308-123">Content-Type</span></span>   | <span data-ttu-id="66308-124">application/json</span><span class="sxs-lookup"><span data-stu-id="66308-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="66308-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66308-125">Request body</span></span>
<span data-ttu-id="66308-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="66308-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66308-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="66308-127">Response</span></span>

<span data-ttu-id="66308-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [ContactFolder](../resources/contactfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66308-128">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="66308-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66308-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66308-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66308-130">Request</span></span>
<span data-ttu-id="66308-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66308-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders
```
##### <a name="response"></a><span data-ttu-id="66308-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="66308-132">Response</span></span>
<span data-ttu-id="66308-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66308-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
