# <a name="mailfolder-move"></a><span data-ttu-id="c84ae-101">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="c84ae-101">mailFolder: move</span></span>

<span data-ttu-id="c84ae-102">Mova uma pasta de email e seu conteúdo para outra pasta de email.</span><span class="sxs-lookup"><span data-stu-id="c84ae-102">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c84ae-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c84ae-103">Prerequisites</span></span>
<span data-ttu-id="c84ae-104">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="c84ae-104">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="c84ae-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c84ae-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="c84ae-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c84ae-106">Request headers</span></span>
| <span data-ttu-id="c84ae-107">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c84ae-107">Header</span></span>       | <span data-ttu-id="c84ae-108">Valor</span><span class="sxs-lookup"><span data-stu-id="c84ae-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c84ae-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="c84ae-109">Authorization</span></span>  | <span data-ttu-id="c84ae-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c84ae-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c84ae-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c84ae-112">Content-Type</span></span>  | <span data-ttu-id="c84ae-p102">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c84ae-p102">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c84ae-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c84ae-115">Request body</span></span>
<span data-ttu-id="c84ae-116">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c84ae-116">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c84ae-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c84ae-117">Parameter</span></span>    | <span data-ttu-id="c84ae-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="c84ae-118">Type</span></span>   |<span data-ttu-id="c84ae-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c84ae-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c84ae-120">destinationId</span><span class="sxs-lookup"><span data-stu-id="c84ae-120">destinationId</span></span>|<span data-ttu-id="c84ae-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c84ae-121">String</span></span>|<span data-ttu-id="c84ae-122">A ID da pasta ou um nome de pasta conhecido, como *Inbox*, *Drafts*, *SentItems* ou *DeletedItems*.</span><span class="sxs-lookup"><span data-stu-id="c84ae-122">The folder ID, or the *Inbox*, *Drafts*, *SentItems*, or *DeletedItems* well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="c84ae-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="c84ae-123">Response</span></span>

<span data-ttu-id="c84ae-124">Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c84ae-124">If successful, this method returns `200, OK` response code and [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c84ae-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c84ae-125">Example</span></span>
<span data-ttu-id="c84ae-126">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c84ae-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c84ae-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c84ae-127">Request</span></span>
<span data-ttu-id="c84ae-128">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c84ae-128">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c84ae-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c84ae-129">Response</span></span>
<span data-ttu-id="c84ae-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c84ae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
