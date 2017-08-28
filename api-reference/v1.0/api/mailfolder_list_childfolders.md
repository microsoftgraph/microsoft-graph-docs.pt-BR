# <a name="list-childfolders"></a><span data-ttu-id="e962e-101">Listar childFolders</span><span class="sxs-lookup"><span data-stu-id="e962e-101">List childFolders</span></span>

<span data-ttu-id="e962e-p101">Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.</span><span class="sxs-lookup"><span data-stu-id="e962e-p101">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="e962e-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="e962e-104">Permissions</span></span>
<span data-ttu-id="e962e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e962e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e962e-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e962e-107">Permission type</span></span>      | <span data-ttu-id="e962e-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e962e-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="e962e-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e962e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e962e-110">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e962e-110">Mail.Read, Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="e962e-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e962e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e962e-112">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e962e-112">Mail.Read, Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="e962e-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e962e-113">Application</span></span> | <span data-ttu-id="e962e-114">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e962e-114">Mail.Read, Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e962e-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e962e-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e962e-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e962e-116">Optional query parameters</span></span>
<span data-ttu-id="e962e-117">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e962e-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e962e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e962e-118">Request headers</span></span>
| <span data-ttu-id="e962e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e962e-119">Name</span></span>       | <span data-ttu-id="e962e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e962e-120">Type</span></span> | <span data-ttu-id="e962e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e962e-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e962e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e962e-122">Authorization</span></span>  | <span data-ttu-id="e962e-123">string</span><span class="sxs-lookup"><span data-stu-id="e962e-123">string</span></span>  | <span data-ttu-id="e962e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e962e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e962e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e962e-126">Request body</span></span>
<span data-ttu-id="e962e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e962e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e962e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e962e-128">Response</span></span>

<span data-ttu-id="e962e-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e962e-129">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e962e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e962e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e962e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e962e-131">Request</span></span>
<span data-ttu-id="e962e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e962e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="e962e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e962e-133">Response</span></span>
<span data-ttu-id="e962e-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e962e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
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
