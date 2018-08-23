# <a name="delete-subscription"></a><span data-ttu-id="9a637-101">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="9a637-101">Delete subscription</span></span>

<span data-ttu-id="9a637-102">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="9a637-102">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a637-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a637-103">Permissions</span></span>

<span data-ttu-id="9a637-p101">A tabela a seguir lista a permissão sugerida necessária para cada recurso. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9a637-p101">The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="9a637-106">Tipo de recurso/item</span><span class="sxs-lookup"><span data-stu-id="9a637-106">Resource type / Item</span></span>        | <span data-ttu-id="9a637-107">Permissão</span><span class="sxs-lookup"><span data-stu-id="9a637-107">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="9a637-108">Contatos</span><span class="sxs-lookup"><span data-stu-id="9a637-108">Contacts</span></span>                    | <span data-ttu-id="9a637-109">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="9a637-109">Contacts.Read</span></span>       |
| <span data-ttu-id="9a637-110">Conversas</span><span class="sxs-lookup"><span data-stu-id="9a637-110">Conversations</span></span>               | <span data-ttu-id="9a637-111">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a637-111">Group.Read.All</span></span>      |
| <span data-ttu-id="9a637-112">Eventos</span><span class="sxs-lookup"><span data-stu-id="9a637-112">Events</span></span>                      | <span data-ttu-id="9a637-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="9a637-113">Calendars.Read</span></span>      |
| <span data-ttu-id="9a637-114">Mensagens</span><span class="sxs-lookup"><span data-stu-id="9a637-114">Messages</span></span>                    | <span data-ttu-id="9a637-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="9a637-115">Mail.Read</span></span>           |
| <span data-ttu-id="9a637-116">Grupos</span><span class="sxs-lookup"><span data-stu-id="9a637-116">Groups</span></span>                      | <span data-ttu-id="9a637-117">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a637-117">Group.Read.All</span></span>      |
| <span data-ttu-id="9a637-118">Usuários</span><span class="sxs-lookup"><span data-stu-id="9a637-118">Users</span></span>                       | <span data-ttu-id="9a637-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="9a637-119">User.Read.All</span></span>       |
| <span data-ttu-id="9a637-120">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="9a637-120">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="9a637-121">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a637-121">Files.ReadWrite</span></span>     |
| <span data-ttu-id="9a637-122">Unidades (unidades e conteúdo compartilhados do SharePoint)</span><span class="sxs-lookup"><span data-stu-id="9a637-122">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="9a637-123">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a637-123">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a637-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a637-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9a637-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a637-125">Request headers</span></span>

| <span data-ttu-id="9a637-126">Nome</span><span class="sxs-lookup"><span data-stu-id="9a637-126">Name</span></span>       | <span data-ttu-id="9a637-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a637-127">Type</span></span> | <span data-ttu-id="9a637-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a637-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9a637-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a637-129">Authorization</span></span>  | <span data-ttu-id="9a637-130">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a637-130">string</span></span>  | <span data-ttu-id="9a637-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a637-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a637-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a637-133">Request body</span></span>

<span data-ttu-id="9a637-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a637-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a637-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a637-135">Response</span></span>

<span data-ttu-id="9a637-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9a637-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9a637-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a637-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9a637-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a637-138">Request</span></span>

<span data-ttu-id="9a637-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a637-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

##### <a name="response"></a><span data-ttu-id="9a637-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a637-140">Response</span></span>

<span data-ttu-id="9a637-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a637-141">Here is an example of the response.</span></span>
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
