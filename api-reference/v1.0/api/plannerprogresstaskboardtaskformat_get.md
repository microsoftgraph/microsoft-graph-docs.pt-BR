# <a name="get-plannerprogresstaskboardtaskformat"></a><span data-ttu-id="e37cc-101">Obter plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e37cc-101">Get plannerProgressTaskBoardTaskFormat</span></span>

<span data-ttu-id="e37cc-102">Recupere as propriedades e os relacionamentos do objeto **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="e37cc-102">Retrieve the properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e37cc-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="e37cc-103">Permissions</span></span>
<span data-ttu-id="e37cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e37cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e37cc-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e37cc-106">Permission type</span></span>      | <span data-ttu-id="e37cc-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e37cc-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e37cc-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e37cc-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e37cc-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e37cc-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e37cc-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e37cc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e37cc-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e37cc-111">Not supported.</span></span>    |
|<span data-ttu-id="e37cc-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e37cc-112">Application</span></span> | <span data-ttu-id="e37cc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e37cc-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e37cc-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e37cc-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/progressTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="e37cc-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e37cc-115">Request headers</span></span>
| <span data-ttu-id="e37cc-116">Nome</span><span class="sxs-lookup"><span data-stu-id="e37cc-116">Name</span></span>      |<span data-ttu-id="e37cc-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="e37cc-117">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e37cc-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="e37cc-118">Authorization</span></span>  | <span data-ttu-id="e37cc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e37cc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e37cc-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e37cc-121">Request body</span></span>
<span data-ttu-id="e37cc-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e37cc-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e37cc-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="e37cc-123">Response</span></span>

<span data-ttu-id="e37cc-124">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e37cc-124">If successful, this method returns a `200 OK` response code and [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="e37cc-p103">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="e37cc-p103">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="e37cc-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e37cc-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e37cc-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e37cc-129">Request</span></span>
<span data-ttu-id="e37cc-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e37cc-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerprogresstaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/progressTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="e37cc-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e37cc-131">Response</span></span>
<span data-ttu-id="e37cc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e37cc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
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
  "description": "Get plannerProgressTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->