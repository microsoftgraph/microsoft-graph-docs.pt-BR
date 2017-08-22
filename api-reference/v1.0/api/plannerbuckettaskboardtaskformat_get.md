# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="dcf78-101">Get plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="dcf78-101">Get plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="dcf78-102">Recupere as propriedades e os relacionamentos do objeto **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="dcf78-102">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dcf78-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dcf78-103">Prerequisites</span></span>
<span data-ttu-id="dcf78-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="dcf78-104">The following **scopes** are required to execute this API:</span></span> 

<span data-ttu-id="dcf78-105">*Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="dcf78-105">*Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="dcf78-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcf78-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/<id>/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="dcf78-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcf78-107">Request headers</span></span>
| <span data-ttu-id="dcf78-108">Nome</span><span class="sxs-lookup"><span data-stu-id="dcf78-108">Name</span></span>      |<span data-ttu-id="dcf78-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcf78-109">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dcf78-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcf78-110">Authorization</span></span>  | <span data-ttu-id="dcf78-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcf78-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcf78-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcf78-113">Request body</span></span>
<span data-ttu-id="dcf78-114">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dcf78-114">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcf78-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcf78-115">Response</span></span>

<span data-ttu-id="dcf78-116">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcf78-116">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="dcf78-p102">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="dcf78-p102">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="dcf78-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dcf78-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dcf78-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcf78-121">Request</span></span>
<span data-ttu-id="dcf78-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcf78-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/bucketTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="dcf78-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcf78-123">Response</span></span>
<span data-ttu-id="dcf78-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcf78-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 76

{
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh",
  "orderHint": "85752723360752+"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerBucketTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->