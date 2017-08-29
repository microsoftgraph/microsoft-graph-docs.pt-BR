# <a name="create-mailfolder"></a><span data-ttu-id="2b143-101">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="2b143-101">Create MailFolder</span></span>

<span data-ttu-id="2b143-102">Use essa API para criar uma nova pasta de email na pasta raiz da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="2b143-102">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b143-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b143-103">Permissions</span></span>
<span data-ttu-id="2b143-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2b143-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2b143-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b143-106">Permission type</span></span>      | <span data-ttu-id="2b143-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b143-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b143-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b143-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2b143-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b143-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2b143-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b143-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b143-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b143-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2b143-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b143-112">Application</span></span> | <span data-ttu-id="2b143-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b143-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b143-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b143-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="2b143-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b143-115">Request headers</span></span>
| <span data-ttu-id="2b143-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2b143-116">Header</span></span>       | <span data-ttu-id="2b143-117">Valor</span><span class="sxs-lookup"><span data-stu-id="2b143-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2b143-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b143-118">Authorization</span></span>  | <span data-ttu-id="2b143-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b143-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2b143-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b143-121">Content-Type</span></span>  | <span data-ttu-id="2b143-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2b143-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b143-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b143-123">Request body</span></span>
<span data-ttu-id="2b143-p103">No corpo da solicitação, forneça um objeto JSON com os parâmetros a seguir. **displayName** é a única propriedade gravável para um objeto [MailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="2b143-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="2b143-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2b143-126">Parameter</span></span>    | <span data-ttu-id="2b143-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b143-127">Type</span></span>   |<span data-ttu-id="2b143-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b143-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b143-129">displayName</span><span class="sxs-lookup"><span data-stu-id="2b143-129">displayName</span></span>|<span data-ttu-id="2b143-130">String</span><span class="sxs-lookup"><span data-stu-id="2b143-130">String</span></span>|<span data-ttu-id="2b143-131">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="2b143-131">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="2b143-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b143-132">Response</span></span>

<span data-ttu-id="2b143-133">Se bem-sucedido, este método retorna o código de resposta `201, Created` e um objeto [MailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b143-133">If successful, this method returns `201, Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b143-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b143-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b143-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b143-135">Request</span></span>
<span data-ttu-id="2b143-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b143-136">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2b143-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b143-137">Response</span></span>
<span data-ttu-id="2b143-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2b143-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
