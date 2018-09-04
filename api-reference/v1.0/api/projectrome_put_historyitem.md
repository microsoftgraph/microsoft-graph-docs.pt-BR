# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="164a9-101">Criar ou substituir um historyItem</span><span class="sxs-lookup"><span data-stu-id="164a9-101">Create or replace a history item</span></span>

<span data-ttu-id="164a9-102">Criar um novo ou substituir um item de histórico existente para uma atividade existente do usuário.</span><span class="sxs-lookup"><span data-stu-id="164a9-102">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="164a9-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="164a9-103">Permissions</span></span>

<span data-ttu-id="164a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="164a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="164a9-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="164a9-106">Permission type</span></span>      | <span data-ttu-id="164a9-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="164a9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="164a9-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="164a9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="164a9-109">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="164a9-109">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="164a9-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="164a9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="164a9-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="164a9-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="164a9-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="164a9-112">Application</span></span> | <span data-ttu-id="164a9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="164a9-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="164a9-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="164a9-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="164a9-115">O Id deve ser um GUID.</span><span class="sxs-lookup"><span data-stu-id="164a9-115">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="164a9-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="164a9-116">Request headers</span></span>

|<span data-ttu-id="164a9-117">Nome</span><span class="sxs-lookup"><span data-stu-id="164a9-117">Name</span></span> | <span data-ttu-id="164a9-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="164a9-118">Type</span></span> | <span data-ttu-id="164a9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="164a9-119">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="164a9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="164a9-120">Authorization</span></span> | <span data-ttu-id="164a9-121">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="164a9-121">string</span></span> | <span data-ttu-id="164a9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="164a9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="164a9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="164a9-124">Request body</span></span>

<span data-ttu-id="164a9-125">No corpo da solicitação, forneça uma representação JSON de um objeto [historyItem](../resources/projectrome_historyitem.md).</span><span class="sxs-lookup"><span data-stu-id="164a9-125">In the request body, supply a JSON representation of [directoryObject](../resources/projectrome_historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="164a9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="164a9-126">Response</span></span>

<span data-ttu-id="164a9-127">Se tiver êxito, este método retornará o código de resposta `201 Created` se o historyItem foi criado ou `200 OK` se o historyItem foi substituído.</span><span class="sxs-lookup"><span data-stu-id="164a9-127">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="164a9-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="164a9-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="164a9-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="164a9-129">Request</span></span>

<span data-ttu-id="164a9-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="164a9-130">Here is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_historyItem"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
Content-type: application/json
Content-length: 364

{
    "startedDateTime": "2015-02-11T20:54:04.3457274+00:00",
    "userTimezone": "Africa/Casablanca",
    "lastActiveDateTime": "2015-02-11T20:54:04.3457274+00:00"
}
```

#### <a name="response"></a><span data-ttu-id="164a9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="164a9-131">Response</span></span>

<span data-ttu-id="164a9-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="164a9-132">Here is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activityHistoryItem"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('user%40contoso.com')/activities('13881113971988980728')/historyItems/$entity",
    "status": "updated",
    "userTimezone": "Africa/Casablanca",
    "createdDateTime": "2018-02-26T20:28:22.14Z",
    "lastModifiedDateTime": "2018-02-26T20:28:22.155Z",
    "id": "9d0b74e4-4b41-43ea-b34d-f9c1bf9f809c",
    "startedDateTime": "2018-02-26T20:54:04.345Z",
    "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
    "expirationDateTime": "2018-03-28T20:28:22.14Z",
    "activeDurationSeconds": 20
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->