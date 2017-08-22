# <a name="get-plannerplan"></a><span data-ttu-id="7f771-101">Obter plannerPlan</span><span class="sxs-lookup"><span data-stu-id="7f771-101">Get plannerPlan</span></span>

<span data-ttu-id="7f771-102">Recupere as propriedades e os relacionamentos do objeto **plannerplan**.</span><span class="sxs-lookup"><span data-stu-id="7f771-102">Retrieve the properties and relationships of **plannerplan** object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f771-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7f771-103">Prerequisites</span></span>
<span data-ttu-id="7f771-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="7f771-104">The following **scopes** are required to execute this API:</span></span> 

<span data-ttu-id="7f771-105">*Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="7f771-105">*Group.Read.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="7f771-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f771-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/<id>
```
## <a name="request-headers"></a><span data-ttu-id="7f771-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f771-107">Request headers</span></span>
| <span data-ttu-id="7f771-108">Nome</span><span class="sxs-lookup"><span data-stu-id="7f771-108">Name</span></span>      |<span data-ttu-id="7f771-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f771-109">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7f771-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f771-110">Authorization</span></span>  | <span data-ttu-id="7f771-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f771-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f771-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f771-113">Request body</span></span>
<span data-ttu-id="7f771-114">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f771-114">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f771-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f771-115">Response</span></span>

<span data-ttu-id="7f771-116">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f771-116">If successful, this method returns a `200 OK` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="7f771-p102">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="7f771-p102">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="7f771-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f771-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f771-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f771-121">Request</span></span>
<span data-ttu-id="7f771-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f771-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM
```
##### <a name="response"></a><span data-ttu-id="7f771-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f771-123">Response</span></span>
<span data-ttu-id="7f771-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f771-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->