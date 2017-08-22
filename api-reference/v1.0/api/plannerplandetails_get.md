# <a name="get-plannerplandetails"></a><span data-ttu-id="138a4-101">Obter plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="138a4-101">Get plannerPlanDetails</span></span>

<span data-ttu-id="138a4-102">Recupere as propriedades e os relacionamentos de um objeto **plannerplandetails**.</span><span class="sxs-lookup"><span data-stu-id="138a4-102">Retrieve the properties and relationships of **plannerplandetails** object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="138a4-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="138a4-103">Prerequisites</span></span>
<span data-ttu-id="138a4-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="138a4-104">The following **scopes** are required to execute this API:</span></span> 

<span data-ttu-id="138a4-105">*Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="138a4-105">*Group.Read.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="138a4-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="138a4-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/<id>/details
```

## <a name="request-headers"></a><span data-ttu-id="138a4-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="138a4-107">Request headers</span></span>
| <span data-ttu-id="138a4-108">Nome</span><span class="sxs-lookup"><span data-stu-id="138a4-108">Name</span></span>      |<span data-ttu-id="138a4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="138a4-109">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="138a4-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="138a4-110">Authorization</span></span>  | <span data-ttu-id="138a4-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="138a4-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="138a4-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="138a4-113">Request body</span></span>
<span data-ttu-id="138a4-114">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="138a4-114">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="138a4-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="138a4-115">Response</span></span>

<span data-ttu-id="138a4-116">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerPlanDetails](../resources/plannerplandetails.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="138a4-116">If successful, this method returns a `200 OK` response code and [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="138a4-p102">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="138a4-p102">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="138a4-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="138a4-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="138a4-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="138a4-121">Request</span></span>
<span data-ttu-id="138a4-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="138a4-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
```
##### <a name="response"></a><span data-ttu-id="138a4-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="138a4-123">Response</span></span>
<span data-ttu-id="138a4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="138a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerPlanDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->