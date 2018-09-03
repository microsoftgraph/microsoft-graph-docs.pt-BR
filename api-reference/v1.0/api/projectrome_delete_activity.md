# <a name="delete-an-activity"></a><span data-ttu-id="6f6ee-101">Excluir uma atividade</span><span class="sxs-lookup"><span data-stu-id="6f6ee-101">Delete an activity</span></span>

<span data-ttu-id="6f6ee-102">Exclua uma atividade do usuário existente para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6f6ee-102">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f6ee-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f6ee-103">Permissions</span></span>

<span data-ttu-id="6f6ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6f6ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="6f6ee-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f6ee-106">Permission type</span></span>      | <span data-ttu-id="6f6ee-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f6ee-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f6ee-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f6ee-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6f6ee-109">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="6f6ee-109">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="6f6ee-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f6ee-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f6ee-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="6f6ee-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="6f6ee-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f6ee-112">Application</span></span> | <span data-ttu-id="6f6ee-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f6ee-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f6ee-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f6ee-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6f6ee-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f6ee-115">Request headers</span></span>

|<span data-ttu-id="6f6ee-116">Nome</span><span class="sxs-lookup"><span data-stu-id="6f6ee-116">Name</span></span> | <span data-ttu-id="6f6ee-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f6ee-117">Type</span></span> | <span data-ttu-id="6f6ee-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f6ee-118">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="6f6ee-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f6ee-119">Authorization</span></span> | <span data-ttu-id="6f6ee-120">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f6ee-120">string</span></span> | <span data-ttu-id="6f6ee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f6ee-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f6ee-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f6ee-123">Request body</span></span>

<span data-ttu-id="6f6ee-124">Sem corpo de requisição.</span><span class="sxs-lookup"><span data-stu-id="6f6ee-124">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="6f6ee-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f6ee-125">Response</span></span>

<span data-ttu-id="6f6ee-126">Se tiver êxito, este método retornará o `204 No Content` código de resposta se a atividade tiver sido excluída.</span><span class="sxs-lookup"><span data-stu-id="6f6ee-126">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="6f6ee-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f6ee-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6f6ee-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f6ee-128">Request</span></span>

<span data-ttu-id="6f6ee-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f6ee-129">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```

##### <a name="response"></a><span data-ttu-id="6f6ee-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f6ee-130">Response</span></span>

<span data-ttu-id="6f6ee-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f6ee-131">Here is an example of the response.</span></span>

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
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->