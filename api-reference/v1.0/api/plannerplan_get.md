# <a name="get-plannerplan"></a><span data-ttu-id="375a8-101">Obter plannerPlan</span><span class="sxs-lookup"><span data-stu-id="375a8-101">Get plannerPlan</span></span>

<span data-ttu-id="375a8-102">Recupere as propriedades e os relacionamentos do objeto **plannerplan**.</span><span class="sxs-lookup"><span data-stu-id="375a8-102">Retrieve the properties and relationships of **plannerplan** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="375a8-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="375a8-103">Permissions</span></span>
<span data-ttu-id="375a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="375a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="375a8-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="375a8-106">Permission type</span></span>      | <span data-ttu-id="375a8-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="375a8-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="375a8-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="375a8-108">Delegated (work or school account)</span></span> | <span data-ttu-id="375a8-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="375a8-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="375a8-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="375a8-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="375a8-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="375a8-111">Not supported.</span></span>    |
|<span data-ttu-id="375a8-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="375a8-112">Application</span></span> | <span data-ttu-id="375a8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="375a8-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="375a8-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="375a8-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/{id}
```
## <a name="request-headers"></a><span data-ttu-id="375a8-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="375a8-115">Request headers</span></span>
| <span data-ttu-id="375a8-116">Nome</span><span class="sxs-lookup"><span data-stu-id="375a8-116">Name</span></span>      |<span data-ttu-id="375a8-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="375a8-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="375a8-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="375a8-118">Authorization</span></span>  | <span data-ttu-id="375a8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="375a8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="375a8-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="375a8-121">Request body</span></span>
<span data-ttu-id="375a8-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="375a8-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="375a8-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="375a8-123">Response</span></span>

<span data-ttu-id="375a8-124">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="375a8-124">If successful, this method returns a `200 OK` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="375a8-p103">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="375a8-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="375a8-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="375a8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="375a8-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="375a8-129">Request</span></span>
<span data-ttu-id="375a8-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="375a8-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans/{plan-id}
```
##### <a name="response"></a><span data-ttu-id="375a8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="375a8-131">Response</span></span>
<span data-ttu-id="375a8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="375a8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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