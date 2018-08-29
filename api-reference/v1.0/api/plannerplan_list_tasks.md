# <a name="list-tasks"></a><span data-ttu-id="55528-101">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="55528-101">List tasks</span></span>

<span data-ttu-id="55528-102">Recupere uma lista de objetos **plannertask** associada a um objeto [plannerPlan](../resources/plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="55528-102">Retrieve a list of **plannertask** objects associated to a [plannerPlan](../resources/plannerplan.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="55528-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="55528-103">Permissions</span></span>
<span data-ttu-id="55528-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="55528-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="55528-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55528-106">Permission type</span></span>      | <span data-ttu-id="55528-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55528-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55528-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55528-108">Delegated (work or school account)</span></span> | <span data-ttu-id="55528-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55528-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="55528-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55528-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55528-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55528-111">Not supported.</span></span>    |
|<span data-ttu-id="55528-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55528-112">Application</span></span> | <span data-ttu-id="55528-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55528-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="55528-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55528-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="55528-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55528-115">Request headers</span></span>
| <span data-ttu-id="55528-116">Nome</span><span class="sxs-lookup"><span data-stu-id="55528-116">Name</span></span>      |<span data-ttu-id="55528-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="55528-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="55528-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="55528-118">Authorization</span></span>  | <span data-ttu-id="55528-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55528-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55528-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55528-121">Request body</span></span>
<span data-ttu-id="55528-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55528-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55528-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="55528-123">Response</span></span>

<span data-ttu-id="55528-124">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [plannerTask](../resources/plannertask.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55528-124">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="55528-p103">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="55528-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="55528-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55528-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55528-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55528-129">Request</span></span>
<span data-ttu-id="55528-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55528-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}/tasks
```
##### <a name="response"></a><span data-ttu-id="55528-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="55528-131">Response</span></span>
<span data-ttu-id="55528-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55528-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
          "@odata.type": "#microsoft.graph.plannerAssignment",
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