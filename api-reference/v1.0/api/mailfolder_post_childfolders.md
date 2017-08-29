# <a name="create-mailfolder"></a><span data-ttu-id="e65c0-101">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="e65c0-101">Create MailFolder</span></span>

<span data-ttu-id="e65c0-102">Use essa API para criar uma nova mailfolder filha.</span><span class="sxs-lookup"><span data-stu-id="e65c0-102">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="e65c0-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="e65c0-103">Permissions</span></span>
<span data-ttu-id="e65c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e65c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e65c0-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e65c0-106">Permission type</span></span>      | <span data-ttu-id="e65c0-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e65c0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e65c0-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e65c0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e65c0-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e65c0-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e65c0-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e65c0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e65c0-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e65c0-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e65c0-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e65c0-112">Application</span></span> | <span data-ttu-id="e65c0-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e65c0-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e65c0-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e65c0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="e65c0-115">Especifique a pasta pai na URL de consulta como uma ID de pasta, ou os nomes de pasta já conhecidos `Inbox`, `Drafts`, `SentItems` ou `DeletedItems`.</span><span class="sxs-lookup"><span data-stu-id="e65c0-115">Specify the parent folder in the query URL as a folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e65c0-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e65c0-116">Request headers</span></span>
| <span data-ttu-id="e65c0-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e65c0-117">Header</span></span>       | <span data-ttu-id="e65c0-118">Valor</span><span class="sxs-lookup"><span data-stu-id="e65c0-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e65c0-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="e65c0-119">Authorization</span></span>  | <span data-ttu-id="e65c0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e65c0-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e65c0-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e65c0-122">Content-Type</span></span>  | <span data-ttu-id="e65c0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e65c0-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e65c0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e65c0-125">Request body</span></span>
<span data-ttu-id="e65c0-p104">No corpo da solicitação, forneça um objeto JSON com os parâmetros a seguir. **displayName** é a única propriedade gravável para um objeto [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="e65c0-p104">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="e65c0-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e65c0-128">Parameter</span></span>    | <span data-ttu-id="e65c0-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e65c0-129">Type</span></span>   |<span data-ttu-id="e65c0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e65c0-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e65c0-131">displayName</span><span class="sxs-lookup"><span data-stu-id="e65c0-131">displayName</span></span>|<span data-ttu-id="e65c0-132">String</span><span class="sxs-lookup"><span data-stu-id="e65c0-132">String</span></span>|<span data-ttu-id="e65c0-133">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="e65c0-133">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="e65c0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e65c0-134">Response</span></span>

<span data-ttu-id="e65c0-135">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e65c0-135">If successful, this method returns `201, Created` response code and [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e65c0-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e65c0-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e65c0-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e65c0-137">Request</span></span>
<span data-ttu-id="e65c0-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e65c0-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```

##### <a name="response"></a><span data-ttu-id="e65c0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e65c0-139">Response</span></span>
<span data-ttu-id="e65c0-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e65c0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
