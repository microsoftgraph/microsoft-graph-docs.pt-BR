# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="66d8b-101">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="66d8b-101">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="66d8b-102">Remove um grupo de uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="66d8b-102">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="66d8b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="66d8b-103">Permissions</span></span>

<span data-ttu-id="66d8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="66d8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="66d8b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66d8b-106">Permission type</span></span>      | <span data-ttu-id="66d8b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="66d8b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66d8b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66d8b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="66d8b-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66d8b-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="66d8b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66d8b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66d8b-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66d8b-111">Not supported.</span></span>    |
|<span data-ttu-id="66d8b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66d8b-112">Application</span></span> | <span data-ttu-id="66d8b-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66d8b-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66d8b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66d8b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="66d8b-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66d8b-115">Request headers</span></span>

| <span data-ttu-id="66d8b-116">Nome</span><span class="sxs-lookup"><span data-stu-id="66d8b-116">Name</span></span> | <span data-ttu-id="66d8b-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="66d8b-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="66d8b-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="66d8b-118">Authorization</span></span> | <span data-ttu-id="66d8b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66d8b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66d8b-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66d8b-121">Content-Type</span></span>  | <span data-ttu-id="66d8b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="66d8b-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="66d8b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66d8b-123">Request body</span></span>
<span data-ttu-id="66d8b-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66d8b-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="66d8b-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="66d8b-125">Parameter</span></span> | <span data-ttu-id="66d8b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="66d8b-126">Type</span></span> | <span data-ttu-id="66d8b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="66d8b-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="66d8b-128">groupId</span><span class="sxs-lookup"><span data-stu-id="66d8b-128">groupId</span></span>|<span data-ttu-id="66d8b-129">Guid</span><span class="sxs-lookup"><span data-stu-id="66d8b-129">Guid</span></span>| <span data-ttu-id="66d8b-130">A ID do grupo que será removido da política.</span><span class="sxs-lookup"><span data-stu-id="66d8b-130">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="66d8b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="66d8b-131">Response</span></span>

<span data-ttu-id="66d8b-132">Quando é bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="66d8b-132">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="66d8b-133">Quando o grupo é removido da política, o valor **true** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66d8b-133">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="66d8b-134">Caso contrário, um valor **false** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66d8b-134">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="66d8b-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66d8b-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="66d8b-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66d8b-136">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="66d8b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="66d8b-137">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->