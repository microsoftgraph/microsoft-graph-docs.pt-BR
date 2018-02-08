# <a name="create-mailfolder"></a><span data-ttu-id="7d0e5-101">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="7d0e5-101">Create MailFolder</span></span>

<span data-ttu-id="7d0e5-102">Use essa API para criar uma nova mailfolder filha.</span><span class="sxs-lookup"><span data-stu-id="7d0e5-102">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d0e5-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d0e5-103">Permissions</span></span>
<span data-ttu-id="7d0e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7d0e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7d0e5-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d0e5-106">Permission type</span></span>      | <span data-ttu-id="7d0e5-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d0e5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d0e5-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d0e5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7d0e5-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d0e5-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7d0e5-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d0e5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d0e5-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d0e5-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7d0e5-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d0e5-112">Application</span></span> | <span data-ttu-id="7d0e5-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7d0e5-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d0e5-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d0e5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="7d0e5-115">Especifique a pasta pai na URL de consulta como uma ID da pasta ou um nome de pasta comum, como *Caixa de Entrada*, *Rascunhos*, *Itens Enviados* ou *Itens Excluídos*.</span><span class="sxs-lookup"><span data-stu-id="7d0e5-115">Specify the parent folder in the query URL as a folder ID, or a well-known folder name such as *Inbox*, *Drafts*, *SentItems*, or *DeletedItems*.</span></span> <span data-ttu-id="7d0e5-116">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="7d0e5-116">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d0e5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d0e5-117">Request headers</span></span>
| <span data-ttu-id="7d0e5-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d0e5-118">Header</span></span>       | <span data-ttu-id="7d0e5-119">Valor</span><span class="sxs-lookup"><span data-stu-id="7d0e5-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7d0e5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d0e5-120">Authorization</span></span>  | <span data-ttu-id="7d0e5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d0e5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7d0e5-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7d0e5-123">Content-Type</span></span>  | <span data-ttu-id="7d0e5-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d0e5-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7d0e5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d0e5-126">Request body</span></span>
<span data-ttu-id="7d0e5-p105">No corpo da solicitação, forneça um objeto JSON com os parâmetros a seguir. **displayName** é a única propriedade gravável para um objeto [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="7d0e5-p105">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="7d0e5-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7d0e5-129">Parameter</span></span>    | <span data-ttu-id="7d0e5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d0e5-130">Type</span></span>   |<span data-ttu-id="7d0e5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d0e5-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d0e5-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7d0e5-132">displayName</span></span>|<span data-ttu-id="7d0e5-133">String</span><span class="sxs-lookup"><span data-stu-id="7d0e5-133">String</span></span>|<span data-ttu-id="7d0e5-134">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="7d0e5-134">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="7d0e5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d0e5-135">Response</span></span>

<span data-ttu-id="7d0e5-136">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d0e5-136">If successful, this method returns `201 Created` response code and [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d0e5-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d0e5-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d0e5-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d0e5-138">Request</span></span>
<span data-ttu-id="7d0e5-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d0e5-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7d0e5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d0e5-140">Response</span></span>
<span data-ttu-id="7d0e5-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d0e5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
