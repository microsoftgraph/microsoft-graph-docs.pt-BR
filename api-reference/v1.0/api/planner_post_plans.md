# <a name="create-plannerplan"></a><span data-ttu-id="c17a6-101">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c17a6-101">Create plannerPlan</span></span>

<span data-ttu-id="c17a6-102">Use essa API para criar um novo **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="c17a6-102">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="c17a6-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="c17a6-103">Permissions</span></span>
<span data-ttu-id="c17a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c17a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c17a6-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c17a6-106">Permission type</span></span>      | <span data-ttu-id="c17a6-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c17a6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c17a6-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c17a6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c17a6-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c17a6-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c17a6-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c17a6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c17a6-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c17a6-111">Not supported.</span></span>    |
|<span data-ttu-id="c17a6-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c17a6-112">Application</span></span> | <span data-ttu-id="c17a6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c17a6-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c17a6-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c17a6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/plans

```
## <a name="request-headers"></a><span data-ttu-id="c17a6-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c17a6-115">Request headers</span></span>
| <span data-ttu-id="c17a6-116">Nome</span><span class="sxs-lookup"><span data-stu-id="c17a6-116">Name</span></span>       | <span data-ttu-id="c17a6-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="c17a6-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c17a6-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="c17a6-118">Authorization</span></span>  | <span data-ttu-id="c17a6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c17a6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c17a6-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c17a6-121">Request body</span></span>
<span data-ttu-id="c17a6-p103">No corpo da solicitação, forneça uma representação JSON do objeto [plannerPlan](../resources/plannerplan.md). A propriedade owner do **plannerPlan** deve ser definida com uma identificação de um objeto [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="c17a6-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c17a6-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="c17a6-124">Response</span></span>

<span data-ttu-id="c17a6-125">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c17a6-125">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="c17a6-p104">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="c17a6-p104">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="c17a6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c17a6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c17a6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c17a6-130">Request</span></span>
<span data-ttu-id="c17a6-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c17a6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```
<span data-ttu-id="c17a6-132">No corpo da solicitação, forneça uma representação JSON do objeto [plannerPlan](../resources/plannerplan.md).</span><span class="sxs-lookup"><span data-stu-id="c17a6-132">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c17a6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c17a6-133">Response</span></span>
<span data-ttu-id="c17a6-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c17a6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->