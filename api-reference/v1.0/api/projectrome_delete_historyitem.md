# <a name="delete-a-historyitem"></a><span data-ttu-id="c0698-101">Excluir um historyItem</span><span class="sxs-lookup"><span data-stu-id="c0698-101">Delete a historyItem</span></span>

<span data-ttu-id="c0698-102">Exclua um item de histórico existente para uma atividade de usuário existente.</span><span class="sxs-lookup"><span data-stu-id="c0698-102">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0698-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0698-103">Permissions</span></span>

<span data-ttu-id="c0698-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c0698-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="c0698-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0698-106">Permission type</span></span>      | <span data-ttu-id="c0698-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0698-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0698-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0698-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c0698-109">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="c0698-109">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="c0698-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0698-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0698-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="c0698-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="c0698-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0698-112">Application</span></span> | <span data-ttu-id="c0698-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0698-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0698-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0698-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c0698-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0698-115">Request headers</span></span>

|<span data-ttu-id="c0698-116">Nome</span><span class="sxs-lookup"><span data-stu-id="c0698-116">Name</span></span> | <span data-ttu-id="c0698-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0698-117">Type</span></span> | <span data-ttu-id="c0698-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0698-118">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="c0698-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0698-119">Authorization</span></span> | <span data-ttu-id="c0698-120">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0698-120">string</span></span> | <span data-ttu-id="c0698-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0698-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0698-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0698-123">Request body</span></span>

<span data-ttu-id="c0698-124">Sem corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0698-124">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="c0698-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0698-125">Response</span></span>

<span data-ttu-id="c0698-126">Se tiver êxito, este método retornará o código de resposta `204 No Content` se o histórico tiver sido excluído.</span><span class="sxs-lookup"><span data-stu-id="c0698-126">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="c0698-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0698-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c0698-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0698-128">Request</span></span>

<span data-ttu-id="c0698-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0698-129">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
```

##### <a name="response"></a><span data-ttu-id="c0698-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0698-130">Response</span></span>

<span data-ttu-id="c0698-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0698-131">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->