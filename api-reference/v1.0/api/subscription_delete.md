# <a name="delete-subscription"></a><span data-ttu-id="7e362-101">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="7e362-101">Delete subscription</span></span>

<span data-ttu-id="7e362-102">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="7e362-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e362-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e362-103">Permissions</span></span>

<span data-ttu-id="7e362-p101">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7e362-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="7e362-106">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="7e362-106">Resource type / Item</span></span>        | <span data-ttu-id="7e362-107">Permissão</span><span class="sxs-lookup"><span data-stu-id="7e362-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="7e362-108">Contatos</span><span class="sxs-lookup"><span data-stu-id="7e362-108">Contacts</span></span>                    | <span data-ttu-id="7e362-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7e362-109">Contacts.Read</span></span>       |
| <span data-ttu-id="7e362-110">Conversas</span><span class="sxs-lookup"><span data-stu-id="7e362-110">Conversations</span></span>               | <span data-ttu-id="7e362-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e362-111">Group.Read.All</span></span>      |
| <span data-ttu-id="7e362-112">Eventos</span><span class="sxs-lookup"><span data-stu-id="7e362-112">Events</span></span>                      | <span data-ttu-id="7e362-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7e362-113">Calendars.Read</span></span>      |
| <span data-ttu-id="7e362-114">Mensagens</span><span class="sxs-lookup"><span data-stu-id="7e362-114">Messages</span></span>                    | <span data-ttu-id="7e362-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7e362-115">Mail.Read</span></span>           |
| <span data-ttu-id="7e362-116">Grupos</span><span class="sxs-lookup"><span data-stu-id="7e362-116">Groups</span></span>                      | <span data-ttu-id="7e362-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e362-117">Group.Read.All</span></span>      |
| <span data-ttu-id="7e362-118">Usuários</span><span class="sxs-lookup"><span data-stu-id="7e362-118">Users</span></span>                       | <span data-ttu-id="7e362-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e362-119">User.Read.All</span></span>       |
| <span data-ttu-id="7e362-120">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="7e362-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="7e362-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e362-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="7e362-122">Drives (conteúdo do SharePoint shared e unidades)</span><span class="sxs-lookup"><span data-stu-id="7e362-122">Drives (SharePoint shared content and drives)</span></span> | <span data-ttu-id="7e362-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e362-123">Files.ReadWrite.All</span></span> |
|<span data-ttu-id="7e362-124">Alerta de segurança</span><span class="sxs-lookup"><span data-stu-id="7e362-124">Security alert</span></span>| <span data-ttu-id="7e362-125">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e362-125">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e362-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e362-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7e362-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e362-127">Request headers</span></span>

| <span data-ttu-id="7e362-128">Nome</span><span class="sxs-lookup"><span data-stu-id="7e362-128">Name</span></span>       | <span data-ttu-id="7e362-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e362-129">Type</span></span> | <span data-ttu-id="7e362-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e362-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7e362-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e362-131">Authorization</span></span>  | <span data-ttu-id="7e362-132">string</span><span class="sxs-lookup"><span data-stu-id="7e362-132">string</span></span>  | <span data-ttu-id="7e362-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e362-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e362-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e362-135">Request body</span></span>

<span data-ttu-id="7e362-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e362-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e362-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e362-137">Response</span></span>

<span data-ttu-id="7e362-138">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7e362-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7e362-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e362-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7e362-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e362-140">Request</span></span>

<span data-ttu-id="7e362-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e362-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="7e362-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e362-142">Response</span></span>

<span data-ttu-id="7e362-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e362-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
