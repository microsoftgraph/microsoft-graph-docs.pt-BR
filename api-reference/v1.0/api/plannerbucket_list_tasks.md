# <a name="list-tasks"></a><span data-ttu-id="7b60a-101">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="7b60a-101">List tasks</span></span>

<span data-ttu-id="7b60a-102">Recupere uma lista de objetos **plannerTask** associados a um objeto [plannerBucket](../resources/plannerBucket.md).</span><span class="sxs-lookup"><span data-stu-id="7b60a-102">Retrieve a list of **plannerTask** objects associated to a [plannerBucket](../resources/plannerBucket.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b60a-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7b60a-103">Prerequisites</span></span>
<span data-ttu-id="7b60a-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="7b60a-104">The following **scopes** are required to execute this API:</span></span> 

<span data-ttu-id="7b60a-105">*Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="7b60a-105">*Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="7b60a-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b60a-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets/<id>/tasks
```

## <a name="request-headers"></a><span data-ttu-id="7b60a-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b60a-107">Request headers</span></span>
| <span data-ttu-id="7b60a-108">Nome</span><span class="sxs-lookup"><span data-stu-id="7b60a-108">Name</span></span>      |<span data-ttu-id="7b60a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b60a-109">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7b60a-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b60a-110">Authorization</span></span>  | <span data-ttu-id="7b60a-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b60a-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b60a-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b60a-113">Request body</span></span>
<span data-ttu-id="7b60a-114">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b60a-114">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b60a-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b60a-115">Response</span></span>

<span data-ttu-id="7b60a-116">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerTask](../resources/plannertask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b60a-116">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="7b60a-p102">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="7b60a-p102">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="7b60a-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b60a-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b60a-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b60a-121">Request</span></span>
<span data-ttu-id="7b60a-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b60a-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/buckets/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/tasks
```
##### <a name="response"></a><span data-ttu-id="7b60a-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b60a-123">Response</span></span>
<span data-ttu-id="7b60a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7b60a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 833

{
  "value": [
    {
      "createdBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
      "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
      "title": "title-value",
      "orderHint": "9223370609546166567W",
      "assigneePriority": "90057581\"",
      "createdDateTime": "2015-03-25T18:36:49.2407981Z",
      "assignments": {
        "fbab97d0-4932-4511-b675-204639209557": {
          "@odata.type": "#microsoft.graph.plannerassignment",
          "assignedBy": {
            "user": {
              "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
            }
          },
          "assignedDateTime": "2015-03-25T18:38:21.956Z",
          "orderHint": "RWk1"
         }
      },
      "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->