# <a name="create-mailfolder"></a><span data-ttu-id="6badb-101">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="6badb-101">Create MailFolder</span></span>

<span data-ttu-id="6badb-102">Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="6badb-102">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6badb-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6badb-103">Prerequisites</span></span>
<span data-ttu-id="6badb-104">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="6badb-104">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="6badb-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6badb-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="6badb-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6badb-106">Request headers</span></span>
| <span data-ttu-id="6badb-107">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6badb-107">Header</span></span>       | <span data-ttu-id="6badb-108">Valor</span><span class="sxs-lookup"><span data-stu-id="6badb-108">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6badb-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="6badb-109">Authorization</span></span>  | <span data-ttu-id="6badb-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6badb-p101">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6badb-112">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6badb-112">Content-Type</span></span>  | <span data-ttu-id="6badb-113">application/json</span><span class="sxs-lookup"><span data-stu-id="6badb-113">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6badb-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6badb-114">Request body</span></span>
<span data-ttu-id="6badb-p102">No corpo da solicitação, forneça um objeto JSON com os parâmetros a seguir. **displayName** é a única propriedade gravável para um objeto [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="6badb-p102">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="6badb-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6badb-117">Parameter</span></span>    | <span data-ttu-id="6badb-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="6badb-118">Type</span></span>   |<span data-ttu-id="6badb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6badb-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6badb-120">displayName</span><span class="sxs-lookup"><span data-stu-id="6badb-120">displayName</span></span>|<span data-ttu-id="6badb-121">String</span><span class="sxs-lookup"><span data-stu-id="6badb-121">String</span></span>|<span data-ttu-id="6badb-122">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="6badb-122">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="6badb-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="6badb-123">Response</span></span>

<span data-ttu-id="6badb-124">Se bem-sucedido, este método retorna o código de resposta `201, Created` e um objeto [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6badb-124">If successful, this method returns `201, Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6badb-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6badb-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6badb-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6badb-126">Request</span></span>
<span data-ttu-id="6badb-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6badb-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="6badb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6badb-128">Response</span></span>
<span data-ttu-id="6badb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6badb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 201 Created
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
