# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="e1ef6-101">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="e1ef6-101">groupLifecyclePolicy: addGroup</span></span>

<span data-ttu-id="e1ef6-102">Adiciona um grupo a uma política de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="e1ef6-102">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1ef6-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1ef6-103">Permissions</span></span>

<span data-ttu-id="e1ef6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1ef6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="e1ef6-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1ef6-106">Permission type</span></span>      | <span data-ttu-id="e1ef6-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1ef6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1ef6-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1ef6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e1ef6-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1ef6-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1ef6-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1ef6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1ef6-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1ef6-111">Not supported.</span></span>    |
|<span data-ttu-id="e1ef6-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1ef6-112">Application</span></span> | <span data-ttu-id="e1ef6-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1ef6-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1ef6-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1ef6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="e1ef6-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1ef6-115">Request headers</span></span>

| <span data-ttu-id="e1ef6-116">Nome</span><span class="sxs-lookup"><span data-stu-id="e1ef6-116">Name</span></span> | <span data-ttu-id="e1ef6-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1ef6-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e1ef6-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1ef6-118">Authorization</span></span> | <span data-ttu-id="e1ef6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1ef6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1ef6-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1ef6-121">Content-Type</span></span>  | <span data-ttu-id="e1ef6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e1ef6-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1ef6-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1ef6-123">Request body</span></span>
<span data-ttu-id="e1ef6-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1ef6-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e1ef6-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e1ef6-125">Parameter</span></span> | <span data-ttu-id="e1ef6-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1ef6-126">Type</span></span> | <span data-ttu-id="e1ef6-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1ef6-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e1ef6-128">groupId</span><span class="sxs-lookup"><span data-stu-id="e1ef6-128">groupId</span></span>|<span data-ttu-id="e1ef6-129">Guid</span><span class="sxs-lookup"><span data-stu-id="e1ef6-129">Guid</span></span>| <span data-ttu-id="e1ef6-130">A ID do grupo que será adicionado à política.</span><span class="sxs-lookup"><span data-stu-id="e1ef6-130">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="e1ef6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1ef6-131">Response</span></span>

<span data-ttu-id="e1ef6-132">Quando é bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="e1ef6-132">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="e1ef6-133">Quando o grupo é adicionado à política, o valor **true** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1ef6-133">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="e1ef6-134">Caso contrário, um valor **false** é retornado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1ef6-134">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="e1ef6-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1ef6-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e1ef6-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1ef6-136">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a><span data-ttu-id="e1ef6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1ef6-137">Response</span></span>
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
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->