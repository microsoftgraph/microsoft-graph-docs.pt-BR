# <a name="message-copy"></a><span data-ttu-id="8d99b-101">message: copy</span><span class="sxs-lookup"><span data-stu-id="8d99b-101">message: copy</span></span>

<span data-ttu-id="8d99b-102">Copie uma mensagem para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="8d99b-102">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d99b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d99b-103">Permissions</span></span>

<span data-ttu-id="8d99b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8d99b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="8d99b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d99b-106">Permission type</span></span> | <span data-ttu-id="8d99b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d99b-107">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="8d99b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d99b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="8d99b-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d99b-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8d99b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d99b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d99b-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d99b-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="8d99b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d99b-112">Application</span></span> | <span data-ttu-id="8d99b-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d99b-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d99b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d99b-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="8d99b-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d99b-115">Request headers</span></span>

| <span data-ttu-id="8d99b-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d99b-116">Header</span></span> | <span data-ttu-id="8d99b-117">Valor</span><span class="sxs-lookup"><span data-stu-id="8d99b-117">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="8d99b-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d99b-118">Authorization</span></span> | <span data-ttu-id="8d99b-119">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="8d99b-119"></span></span> <span data-ttu-id="8d99b-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d99b-120">Required.</span></span> |
| <span data-ttu-id="8d99b-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d99b-121">Content-Type</span></span> | <span data-ttu-id="8d99b-122">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="8d99b-122"></span></span> <span data-ttu-id="8d99b-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d99b-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d99b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d99b-124">Request body</span></span>

<span data-ttu-id="8d99b-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d99b-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8d99b-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8d99b-126">Parameter</span></span> | <span data-ttu-id="8d99b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d99b-127">Type</span></span> | <span data-ttu-id="8d99b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d99b-128">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="8d99b-129">destinationId</span><span class="sxs-lookup"><span data-stu-id="8d99b-129">destinationId</span></span>|<span data-ttu-id="8d99b-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d99b-130">String</span></span>|<span data-ttu-id="8d99b-131">O ID da pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="8d99b-131">The destination folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="8d99b-132">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="8d99b-132">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="8d99b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d99b-133">Response</span></span>

<span data-ttu-id="8d99b-134">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um recurso de [mensagem](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d99b-134">If successful, this method returns a `201 Created` response code and a [sharedDriveItem](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d99b-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d99b-135">Example</span></span>

<span data-ttu-id="8d99b-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8d99b-136">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8d99b-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d99b-137">Request</span></span>
<span data-ttu-id="8d99b-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d99b-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="8d99b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d99b-139">Response</span></span>

<span data-ttu-id="8d99b-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d99b-140">Here is an example of the response.</span></span>

> <span data-ttu-id="8d99b-p105">**Observação:** o objeto de resposta mostrado aqui pode estar encurtado para maior legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d99b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
