# <a name="list-directoryroletemplates"></a><span data-ttu-id="6d21c-101">Listar directoryRoleTemplates</span><span class="sxs-lookup"><span data-stu-id="6d21c-101">List directoryRoleTemplates</span></span>

<span data-ttu-id="6d21c-102">Recupera uma lista de objetos directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="6d21c-102">Retrieve a list of directoryRoleTemplate objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d21c-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d21c-103">Permissions</span></span>
<span data-ttu-id="6d21c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6d21c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="6d21c-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d21c-106">Permission type</span></span>      | <span data-ttu-id="6d21c-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d21c-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="6d21c-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d21c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6d21c-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6d21c-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="6d21c-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d21c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d21c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d21c-111">Not supported.</span></span>    | 
|<span data-ttu-id="6d21c-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d21c-112">Application</span></span> | <span data-ttu-id="6d21c-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d21c-113">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6d21c-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d21c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6d21c-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6d21c-115">Optional query parameters</span></span>
<span data-ttu-id="6d21c-116">Esse método **não** tem suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="6d21c-116">This method does **not** support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d21c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d21c-117">Request headers</span></span>
| <span data-ttu-id="6d21c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6d21c-118">Name</span></span>       | <span data-ttu-id="6d21c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d21c-119">Type</span></span> | <span data-ttu-id="6d21c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d21c-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6d21c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d21c-121">Authorization</span></span>  | <span data-ttu-id="6d21c-122">string</span><span class="sxs-lookup"><span data-stu-id="6d21c-122">string</span></span>  | <span data-ttu-id="6d21c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d21c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d21c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d21c-125">Request body</span></span>
<span data-ttu-id="6d21c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d21c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d21c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d21c-127">Response</span></span>

<span data-ttu-id="6d21c-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryRoleTemplate](../resources/directoryroletemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d21c-128">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6d21c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d21c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d21c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d21c-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates
```
##### <a name="response"></a><span data-ttu-id="6d21c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d21c-131">Response</span></span>
<span data-ttu-id="6d21c-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d21c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
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
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
