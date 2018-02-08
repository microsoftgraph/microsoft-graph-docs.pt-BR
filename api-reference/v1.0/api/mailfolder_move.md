# <a name="mailfolder-move"></a><span data-ttu-id="a752c-101">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="a752c-101">mailFolder: move</span></span>

<span data-ttu-id="a752c-102">Mova uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="a752c-102">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="a752c-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="a752c-103">Permissions</span></span>
<span data-ttu-id="a752c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a752c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a752c-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a752c-106">Permission type</span></span>      | <span data-ttu-id="a752c-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a752c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a752c-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a752c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a752c-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a752c-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a752c-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a752c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a752c-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a752c-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a752c-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a752c-112">Application</span></span> | <span data-ttu-id="a752c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a752c-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a752c-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a752c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="a752c-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a752c-115">Request headers</span></span>
| <span data-ttu-id="a752c-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a752c-116">Header</span></span>       | <span data-ttu-id="a752c-117">Valor</span><span class="sxs-lookup"><span data-stu-id="a752c-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a752c-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="a752c-118">Authorization</span></span>  | <span data-ttu-id="a752c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a752c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a752c-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a752c-121">Content-Type</span></span>  | <span data-ttu-id="a752c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a752c-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a752c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a752c-124">Request body</span></span>
<span data-ttu-id="a752c-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a752c-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a752c-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a752c-126">Parameter</span></span>    | <span data-ttu-id="a752c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a752c-127">Type</span></span>   |<span data-ttu-id="a752c-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a752c-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a752c-129">destinationId</span><span class="sxs-lookup"><span data-stu-id="a752c-129">destinationId</span></span>|<span data-ttu-id="a752c-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a752c-130">String</span></span>|<span data-ttu-id="a752c-131">A ID da pasta ou um nome de pasta comum, como *Caixa de Entrada*, *Rascunhos*, *Itens Enviados* ou *Itens Excluídos*.</span><span class="sxs-lookup"><span data-stu-id="a752c-131">The folder ID, or a well-known folder name such as *Inbox*, *Drafts*, *SentItems*, or *DeletedItems*.</span></span> <span data-ttu-id="a752c-132">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a752c-132">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="a752c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a752c-133">Response</span></span>

<span data-ttu-id="a752c-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a752c-134">If successful, this method returns `200 OK` response code and [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a752c-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a752c-135">Example</span></span>
<span data-ttu-id="a752c-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a752c-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a752c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a752c-137">Request</span></span>
<span data-ttu-id="a752c-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a752c-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="a752c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a752c-139">Response</span></span>
<span data-ttu-id="a752c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a752c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
