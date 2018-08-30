# <a name="delete-plannertask"></a><span data-ttu-id="3dbd5-101">Excluir plannerTask</span><span class="sxs-lookup"><span data-stu-id="3dbd5-101">Delete plannerTask</span></span>

<span data-ttu-id="3dbd5-102">Exclua **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="3dbd5-102">Delete **plannerTask**.</span></span>
## <a name="permissions"></a><span data-ttu-id="3dbd5-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="3dbd5-103">Permissions</span></span>
<span data-ttu-id="3dbd5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3dbd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3dbd5-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3dbd5-106">Permission type</span></span>      | <span data-ttu-id="3dbd5-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3dbd5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3dbd5-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3dbd5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="3dbd5-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dbd5-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3dbd5-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3dbd5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dbd5-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dbd5-111">Not supported.</span></span>    |
|<span data-ttu-id="3dbd5-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3dbd5-112">Application</span></span> | <span data-ttu-id="3dbd5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3dbd5-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3dbd5-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3dbd5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/tasks/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3dbd5-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3dbd5-115">Request headers</span></span>
| <span data-ttu-id="3dbd5-116">Nome</span><span class="sxs-lookup"><span data-stu-id="3dbd5-116">Name</span></span>       | <span data-ttu-id="3dbd5-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="3dbd5-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3dbd5-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="3dbd5-118">Authorization</span></span>  | <span data-ttu-id="3dbd5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3dbd5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3dbd5-121">If-Match</span><span class="sxs-lookup"><span data-stu-id="3dbd5-121">If-Match</span></span>  | <span data-ttu-id="3dbd5-p103">O último valor ETag conhecido do objeto **plannerTask** a ser excluído. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3dbd5-p103">Last known ETag value for the **plannerTask** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dbd5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3dbd5-124">Request body</span></span>
<span data-ttu-id="3dbd5-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3dbd5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3dbd5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dbd5-126">Response</span></span>

<span data-ttu-id="3dbd5-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3dbd5-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="3dbd5-p105">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="3dbd5-p105">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="3dbd5-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3dbd5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3dbd5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3dbd5-133">Request</span></span>
<span data-ttu-id="3dbd5-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3dbd5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannertask"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/tasks/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="3dbd5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3dbd5-135">Response</span></span>
<span data-ttu-id="3dbd5-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3dbd5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete plannerTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->