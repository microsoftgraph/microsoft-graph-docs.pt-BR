# <a name="mailfolder-move"></a><span data-ttu-id="e37cc-101">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="e37cc-101">mailFolder: move</span></span>

<span data-ttu-id="e37cc-102">Mova uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="e37cc-102">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="e37cc-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="e37cc-103">Permissions</span></span>

<span data-ttu-id="e37cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e37cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="e37cc-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e37cc-106">Permission type</span></span> | <span data-ttu-id="e37cc-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e37cc-107">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="e37cc-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e37cc-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e37cc-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e37cc-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e37cc-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e37cc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e37cc-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e37cc-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e37cc-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e37cc-112">Application</span></span> | <span data-ttu-id="e37cc-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e37cc-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e37cc-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e37cc-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="e37cc-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e37cc-115">Request headers</span></span>

| <span data-ttu-id="e37cc-116">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e37cc-116">Header</span></span> | <span data-ttu-id="e37cc-117">Valor</span><span class="sxs-lookup"><span data-stu-id="e37cc-117">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="e37cc-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="e37cc-118">Authorization</span></span> | <span data-ttu-id="e37cc-119">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="e37cc-119"></span></span> <span data-ttu-id="e37cc-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e37cc-120">Required.</span></span> |
| <span data-ttu-id="e37cc-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e37cc-121">Content-Type</span></span> | <span data-ttu-id="e37cc-122">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="e37cc-122"></span></span> <span data-ttu-id="e37cc-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e37cc-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e37cc-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e37cc-124">Request body</span></span>

<span data-ttu-id="e37cc-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e37cc-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e37cc-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e37cc-126">Parameter</span></span> | <span data-ttu-id="e37cc-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="e37cc-127">Type</span></span> | <span data-ttu-id="e37cc-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e37cc-128">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="e37cc-129">destinationId</span><span class="sxs-lookup"><span data-stu-id="e37cc-129">destinationId</span></span>|<span data-ttu-id="e37cc-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e37cc-130">String</span></span>|<span data-ttu-id="e37cc-131">O ID da pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="e37cc-131">The destination folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="e37cc-132">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="e37cc-132">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="e37cc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e37cc-133">Response</span></span>

<span data-ttu-id="e37cc-134">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e37cc-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e37cc-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e37cc-135">Example</span></span>

<span data-ttu-id="e37cc-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e37cc-136">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e37cc-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e37cc-137">Request</span></span>

<span data-ttu-id="e37cc-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e37cc-138">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e37cc-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e37cc-139">Response</span></span>

<span data-ttu-id="e37cc-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e37cc-140">Here is an example of the response.</span></span>

> <span data-ttu-id="e37cc-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e37cc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
