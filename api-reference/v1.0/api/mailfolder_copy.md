# <a name="mailfolder-copy"></a><span data-ttu-id="b77d3-101">mailFolder: copy</span><span class="sxs-lookup"><span data-stu-id="b77d3-101">mailFolder: copy</span></span>

<span data-ttu-id="b77d3-102">Copie uma pasta de email e seu conteúdo para outra pasta de email.</span><span class="sxs-lookup"><span data-stu-id="b77d3-102">Copy a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b77d3-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b77d3-103">Permissions</span></span>
<span data-ttu-id="b77d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b77d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b77d3-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b77d3-106">Permission type</span></span>      | <span data-ttu-id="b77d3-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b77d3-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="b77d3-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b77d3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b77d3-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b77d3-109">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="b77d3-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b77d3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b77d3-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b77d3-111">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="b77d3-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b77d3-112">Application</span></span> | <span data-ttu-id="b77d3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b77d3-113">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b77d3-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b77d3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/copy
```
## <a name="request-headers"></a><span data-ttu-id="b77d3-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b77d3-115">Request headers</span></span>
| <span data-ttu-id="b77d3-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b77d3-116">Header</span></span>       | <span data-ttu-id="b77d3-117">Valor</span><span class="sxs-lookup"><span data-stu-id="b77d3-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b77d3-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="b77d3-118">Authorization</span></span>  | <span data-ttu-id="b77d3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b77d3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b77d3-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b77d3-121">Content-Type</span></span>  | <span data-ttu-id="b77d3-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b77d3-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b77d3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b77d3-124">Request body</span></span>
<span data-ttu-id="b77d3-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b77d3-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b77d3-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b77d3-126">Parameter</span></span>    | <span data-ttu-id="b77d3-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b77d3-127">Type</span></span>   |<span data-ttu-id="b77d3-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b77d3-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b77d3-129">destinationId</span><span class="sxs-lookup"><span data-stu-id="b77d3-129">destinationId</span></span>|<span data-ttu-id="b77d3-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b77d3-130">String</span></span>|<span data-ttu-id="b77d3-131">A ID da pasta ou um nome de pasta conhecido, como *Inbox*, *Drafts*, *SentItems* ou *DeletedItems*.</span><span class="sxs-lookup"><span data-stu-id="b77d3-131">The folder ID, or the *Inbox*, *Drafts*, *SentItems*, or *DeletedItems* well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="b77d3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b77d3-132">Response</span></span>

<span data-ttu-id="b77d3-133">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b77d3-133">If successful, this method returns `200, OK` response code and [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b77d3-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b77d3-134">Example</span></span>
<span data-ttu-id="b77d3-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b77d3-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b77d3-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b77d3-136">Request</span></span>
<span data-ttu-id="b77d3-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b77d3-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_copy"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="b77d3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b77d3-138">Response</span></span>
<span data-ttu-id="b77d3-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b77d3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "mailFolder: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
