# <a name="delete-plannerplan"></a><span data-ttu-id="81a22-101">Excluir plannerPlan</span><span class="sxs-lookup"><span data-stu-id="81a22-101">Delete plannerPlan</span></span>

<span data-ttu-id="81a22-102">Exclua **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="81a22-102">Delete **plannerPlan**.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="81a22-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81a22-103">Prerequisites</span></span>
<span data-ttu-id="81a22-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="81a22-104">The following **scopes** are required to execute this API:</span></span> 

<span data-ttu-id="81a22-105">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="81a22-105">*Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="81a22-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81a22-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/plans/<id>

```
## <a name="request-headers"></a><span data-ttu-id="81a22-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81a22-107">Request headers</span></span>
| <span data-ttu-id="81a22-108">Nome</span><span class="sxs-lookup"><span data-stu-id="81a22-108">Name</span></span>       | <span data-ttu-id="81a22-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="81a22-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="81a22-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="81a22-110">Authorization</span></span>  | <span data-ttu-id="81a22-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81a22-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81a22-113">If-Match</span><span class="sxs-lookup"><span data-stu-id="81a22-113">If-Match</span></span>  | <span data-ttu-id="81a22-p102">O último valor ETag conhecido do objeto **plannerPlan** a ser excluído. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81a22-p102">Last known ETag value for the **plannerPlan** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="81a22-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81a22-116">Request body</span></span>
<span data-ttu-id="81a22-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81a22-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81a22-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="81a22-118">Response</span></span>

<span data-ttu-id="81a22-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81a22-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="81a22-p104">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="81a22-p104">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="81a22-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81a22-124">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81a22-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81a22-125">Request</span></span>
<span data-ttu-id="81a22-126">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81a22-126">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannerplan"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/plans/<id>
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="81a22-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="81a22-127">Response</span></span>
<span data-ttu-id="81a22-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81a22-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->