# <a name="get-outlook-category"></a><span data-ttu-id="b4786-101">Obter categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="b4786-101">Get Outlook category</span></span>


<span data-ttu-id="b4786-102">Obtenha as propriedades e as relações do objeto [outlookCategory](../resources/outlookCategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="b4786-102">Get the properties and relationships of the specified [outlookCategory](../resources/outlookCategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4786-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b4786-103">Permissions</span></span>
<span data-ttu-id="b4786-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4786-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b4786-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4786-106">Permission type</span></span>      | <span data-ttu-id="b4786-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b4786-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4786-108">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4786-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b4786-109">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="b4786-109">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="b4786-110">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4786-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4786-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="b4786-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="b4786-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4786-112">Application</span></span> | <span data-ttu-id="b4786-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="b4786-113">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4786-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4786-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b4786-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b4786-115">Optional query parameters</span></span>
<span data-ttu-id="b4786-116">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b4786-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4786-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4786-117">Request headers</span></span>
| <span data-ttu-id="b4786-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b4786-118">Name</span></span>      |<span data-ttu-id="b4786-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4786-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b4786-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4786-120">Authorization</span></span>  | <span data-ttu-id="b4786-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4786-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4786-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4786-123">Request body</span></span>
<span data-ttu-id="b4786-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b4786-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4786-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4786-125">Response</span></span>

<span data-ttu-id="b4786-126">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [outlookCategory](../resources/outlookCategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4786-126">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookCategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b4786-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4786-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4786-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4786-128">Request</span></span>
<span data-ttu-id="b4786-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4786-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["de912e4d-c790-4da9-949c-ccd933aaa0f7"],
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7
```
##### <a name="response"></a><span data-ttu-id="b4786-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4786-130">Response</span></span>
<span data-ttu-id="b4786-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4786-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 249

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
  "displayName":"Yellow category",
  "color":"preset3"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->