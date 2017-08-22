# <a name="list-directoryroletemplates"></a><span data-ttu-id="e7f27-101">Listar directoryRoleTemplates</span><span class="sxs-lookup"><span data-stu-id="e7f27-101">List directoryRoleTemplates</span></span>

<span data-ttu-id="e7f27-102">Recupera uma lista de objetos directoryRoleTemplate.</span><span class="sxs-lookup"><span data-stu-id="e7f27-102">Retrieve a list of directoryRoleTemplate objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7f27-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7f27-103">Prerequisites</span></span>
<span data-ttu-id="e7f27-104">Um dos seguintes **escopos** é necessário para executar esta API: *Directory.Read.All*, *Directory.ReadWrite.All* OU *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="e7f27-104">One of the following **scopes** is required to execute this API: *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="e7f27-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7f27-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e7f27-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e7f27-106">Optional query parameters</span></span>
<span data-ttu-id="e7f27-107">Esse método **não** tem suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="e7f27-107">This method does **not** support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7f27-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7f27-108">Request headers</span></span>
| <span data-ttu-id="e7f27-109">Nome</span><span class="sxs-lookup"><span data-stu-id="e7f27-109">Name</span></span>       | <span data-ttu-id="e7f27-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7f27-110">Type</span></span> | <span data-ttu-id="e7f27-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7f27-111">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e7f27-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7f27-112">Authorization</span></span>  | <span data-ttu-id="e7f27-113">string</span><span class="sxs-lookup"><span data-stu-id="e7f27-113">string</span></span>  | <span data-ttu-id="e7f27-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7f27-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7f27-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7f27-116">Request body</span></span>
<span data-ttu-id="e7f27-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e7f27-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7f27-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7f27-118">Response</span></span>

<span data-ttu-id="e7f27-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryRoleTemplate](../resources/directoryroletemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7f27-119">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7f27-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7f27-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7f27-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7f27-121">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates
```
##### <a name="response"></a><span data-ttu-id="e7f27-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7f27-122">Response</span></span>
<span data-ttu-id="e7f27-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7f27-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
