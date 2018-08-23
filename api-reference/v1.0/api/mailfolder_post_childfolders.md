# <a name="create-mailfolder"></a><span data-ttu-id="c5bd7-101">Criar MailFolder</span><span class="sxs-lookup"><span data-stu-id="c5bd7-101">Create MailFolder</span></span>

<span data-ttu-id="c5bd7-102">Use essa API para criar uma nova mailfolder filha.</span><span class="sxs-lookup"><span data-stu-id="c5bd7-102">Use this API to create a new child mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5bd7-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="c5bd7-103">Permissions</span></span>

<span data-ttu-id="c5bd7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5bd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="c5bd7-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5bd7-106">Permission type</span></span> | <span data-ttu-id="c5bd7-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c5bd7-107">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="c5bd7-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5bd7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c5bd7-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5bd7-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c5bd7-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5bd7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5bd7-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5bd7-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="c5bd7-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c5bd7-112">Application</span></span> | <span data-ttu-id="c5bd7-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c5bd7-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5bd7-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5bd7-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

<span data-ttu-id="c5bd7-115">Especifique a pasta pai na URL de consulta como uma ID de pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="c5bd7-115">Specify the parent folder in the query URL as a folder ID, or the , , , or  well-known folder name.</span></span> <span data-ttu-id="c5bd7-116">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c5bd7-116">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5bd7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5bd7-117">Request headers</span></span>

| <span data-ttu-id="c5bd7-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5bd7-118">Header</span></span> | <span data-ttu-id="c5bd7-119">Valor</span><span class="sxs-lookup"><span data-stu-id="c5bd7-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="c5bd7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5bd7-120">Authorization</span></span> | <span data-ttu-id="c5bd7-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="c5bd7-121"></span></span> <span data-ttu-id="c5bd7-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5bd7-122">Required.</span></span> |
| <span data-ttu-id="c5bd7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5bd7-123">Content-Type</span></span> | <span data-ttu-id="c5bd7-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="c5bd7-124"></span></span> <span data-ttu-id="c5bd7-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5bd7-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5bd7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5bd7-126">Request body</span></span>

<span data-ttu-id="c5bd7-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5bd7-127">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="c5bd7-128">**displayName** é a única propriedade gravável para um objeto [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="c5bd7-128">**displayName** is the only writable property for a [mailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="c5bd7-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c5bd7-129">Parameter</span></span> | <span data-ttu-id="c5bd7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5bd7-130">Type</span></span> | <span data-ttu-id="c5bd7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5bd7-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="c5bd7-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c5bd7-132">displayName</span></span>|<span data-ttu-id="c5bd7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5bd7-133">String</span></span>|<span data-ttu-id="c5bd7-134">O nome de exibição da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="c5bd7-134">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="c5bd7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5bd7-135">Response</span></span>

<span data-ttu-id="c5bd7-136">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o recurso [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5bd7-136">If successful, this method returns a `201 Created` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5bd7-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5bd7-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c5bd7-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5bd7-138">Request</span></span>

<span data-ttu-id="c5bd7-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5bd7-139">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c5bd7-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5bd7-140">Response</span></span>
<span data-ttu-id="c5bd7-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c5bd7-141">Here is an example of the response.</span></span>

> <span data-ttu-id="c5bd7-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5bd7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
