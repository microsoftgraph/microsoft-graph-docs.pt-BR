# <a name="delete-subscription"></a><span data-ttu-id="3d0e4-101">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="3d0e4-101">Delete subscription</span></span>

<span data-ttu-id="3d0e4-102">Exclua uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="3d0e4-102">Delete a subscription.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d0e4-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3d0e4-103">Prerequisites</span></span>

<span data-ttu-id="3d0e4-104">A tabela a seguir lista a permissão sugerida necessária para cada recurso.</span><span class="sxs-lookup"><span data-stu-id="3d0e4-104">The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="3d0e4-105">Tipo de recurso / item</span><span class="sxs-lookup"><span data-stu-id="3d0e4-105">Resource type / Item</span></span>        | <span data-ttu-id="3d0e4-106">Escopo</span><span class="sxs-lookup"><span data-stu-id="3d0e4-106">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="3d0e4-107">Contatos</span><span class="sxs-lookup"><span data-stu-id="3d0e4-107">Contacts</span></span>                    | <span data-ttu-id="3d0e4-108">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="3d0e4-108">Contacts.Read</span></span>       |
| <span data-ttu-id="3d0e4-109">Conversas</span><span class="sxs-lookup"><span data-stu-id="3d0e4-109">Conversations</span></span>               | <span data-ttu-id="3d0e4-110">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d0e4-110">Group.Read.All</span></span>      |
| <span data-ttu-id="3d0e4-111">Eventos</span><span class="sxs-lookup"><span data-stu-id="3d0e4-111">Events</span></span>                      | <span data-ttu-id="3d0e4-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3d0e4-112">Calendars.Read</span></span>      |
| <span data-ttu-id="3d0e4-113">Mensagens</span><span class="sxs-lookup"><span data-stu-id="3d0e4-113">Messages</span></span>                    | <span data-ttu-id="3d0e4-114">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3d0e4-114">Mail.Read</span></span>           |
| <span data-ttu-id="3d0e4-115">Drive (o OneDrive do usuário)</span><span class="sxs-lookup"><span data-stu-id="3d0e4-115">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="3d0e4-116">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d0e4-116">Files.ReadWrite</span></span>     |
| <span data-ttu-id="3d0e4-117">Unidades (unidades e conteúdo compartilhados do Sharepoint)</span><span class="sxs-lookup"><span data-stu-id="3d0e4-117">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="3d0e4-118">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d0e4-118">Files.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d0e4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d0e4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /subscriptions/{subscriptionId}
```
## <a name="request-headers"></a><span data-ttu-id="3d0e4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d0e4-120">Request headers</span></span>
| <span data-ttu-id="3d0e4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3d0e4-121">Name</span></span>       | <span data-ttu-id="3d0e4-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d0e4-122">Type</span></span> | <span data-ttu-id="3d0e4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d0e4-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3d0e4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d0e4-124">Authorization</span></span>  | <span data-ttu-id="3d0e4-125">string</span><span class="sxs-lookup"><span data-stu-id="3d0e4-125">string</span></span>  | <span data-ttu-id="3d0e4-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d0e4-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d0e4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d0e4-128">Request body</span></span>
<span data-ttu-id="3d0e4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d0e4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d0e4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d0e4-130">Response</span></span>

<span data-ttu-id="3d0e4-131">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3d0e4-131">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="3d0e4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d0e4-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d0e4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d0e4-133">Request</span></span>
<span data-ttu-id="3d0e4-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d0e4-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <a name="response"></a><span data-ttu-id="3d0e4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d0e4-135">Response</span></span>
<span data-ttu-id="3d0e4-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d0e4-136">Here is an example of the response.</span></span>
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
