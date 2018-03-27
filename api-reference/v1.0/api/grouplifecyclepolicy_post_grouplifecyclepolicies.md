# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="27ac2-101">Criar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="27ac2-101">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="27ac2-102">Cria um novo objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="27ac2-102">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="27ac2-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="27ac2-103">Permissions</span></span>

<span data-ttu-id="27ac2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="27ac2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="27ac2-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27ac2-106">Permission type</span></span>      | <span data-ttu-id="27ac2-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27ac2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27ac2-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27ac2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="27ac2-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27ac2-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="27ac2-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27ac2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27ac2-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27ac2-111">Not supported.</span></span>    |
|<span data-ttu-id="27ac2-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27ac2-112">Application</span></span> | <span data-ttu-id="27ac2-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27ac2-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27ac2-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27ac2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="27ac2-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27ac2-115">Request headers</span></span>

| <span data-ttu-id="27ac2-116">Nome</span><span class="sxs-lookup"><span data-stu-id="27ac2-116">Name</span></span> | <span data-ttu-id="27ac2-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="27ac2-117">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="27ac2-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="27ac2-118">Authorization</span></span> | <span data-ttu-id="27ac2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27ac2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="27ac2-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27ac2-121">Content-Type</span></span>  | <span data-ttu-id="27ac2-122">application/json</span><span class="sxs-lookup"><span data-stu-id="27ac2-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="27ac2-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27ac2-123">Request body</span></span>
<span data-ttu-id="27ac2-124">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="27ac2-124">In the request body, supply a JSON representation of [plannerPlan](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="27ac2-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="27ac2-125">Response</span></span>

<span data-ttu-id="27ac2-126">Quando é bem-sucedido, este método retorna o código de resposta `201 Created` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27ac2-126">If successful, this method returns a `201 Created` response code and [profilePhoto](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27ac2-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27ac2-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="27ac2-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27ac2-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
<span data-ttu-id="27ac2-129">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="27ac2-129">In the request body, supply a JSON representation of [plannerPlan](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="27ac2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="27ac2-130">Response</span></span>

<span data-ttu-id="27ac2-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27ac2-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->