---
author: JeremyKelley
ms.date: 09/10/2017
title: Compartilhar um arquivo com um link
localization_priority: Normal
ms.prod: sharepoint
description: Você pode usar a ação createLink para compartilhar um DriveItem por meio de um link de compartilhamento.
doc_type: apiPageType
ms.openlocfilehash: 51470bd3f0ebc0044b0dbe06d718002a368d66eb
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239027"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="e4ffe-103">Criar um link de compartilhamento para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="e4ffe-103">Create a sharing link for a DriveItem</span></span>

<span data-ttu-id="e4ffe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4ffe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4ffe-105">Você pode usar a ação **createLink** para compartilhar um [DriveItem](../resources/driveitem.md) por meio de um link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-105">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="e4ffe-p101">A ação **createLink** criará um novo link de compartilhamento se o tipo de link especificado não existir para o aplicativo de chamada. Se um link de compartilhamento do tipo especificado já existir para o aplicativo, o link de compartilhamento existente será retornado.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="e4ffe-108">Recursos de DriveItem herdam permissões de compartilhamento de seus ancestrais.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-108">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4ffe-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="e4ffe-109">Permissions</span></span>

<span data-ttu-id="e4ffe-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4ffe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4ffe-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4ffe-112">Permission type</span></span>      | <span data-ttu-id="e4ffe-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4ffe-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4ffe-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4ffe-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e4ffe-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4ffe-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4ffe-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4ffe-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4ffe-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4ffe-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e4ffe-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4ffe-118">Application</span></span> | <span data-ttu-id="e4ffe-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4ffe-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4ffe-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4ffe-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a><span data-ttu-id="e4ffe-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4ffe-121">Request body</span></span>

<span data-ttu-id="e4ffe-122">O corpo da solicitação define as propriedades do link de compartilhamento que seu aplicativo está solicitando.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-122">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="e4ffe-123">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-123">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="e4ffe-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e4ffe-124">Name</span></span>       |  <span data-ttu-id="e4ffe-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4ffe-125">Type</span></span>  |                                 <span data-ttu-id="e4ffe-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4ffe-126">Description</span></span>                                  |
| :------------| :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="e4ffe-127">**type**</span><span class="sxs-lookup"><span data-stu-id="e4ffe-127">**type**</span></span>     | <span data-ttu-id="e4ffe-128">string</span><span class="sxs-lookup"><span data-stu-id="e4ffe-128">string</span></span> | <span data-ttu-id="e4ffe-p104">O tipo de link de compartilhamento a ser criado. Pode ser `view`, `edit` ou `embed`.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-p104">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="e4ffe-131">**password**</span><span class="sxs-lookup"><span data-stu-id="e4ffe-131">**password**</span></span> | <span data-ttu-id="e4ffe-132">string</span><span class="sxs-lookup"><span data-stu-id="e4ffe-132">string</span></span> | <span data-ttu-id="e4ffe-133">A senha do link de compartilhamento definido pelo criador.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-133">The password of the sharing link that is set by the creator.</span></span> <span data-ttu-id="e4ffe-134">Opcional e somente OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-134">Optional and OneDrive Personal only.</span></span>
| <span data-ttu-id="e4ffe-135">**expirationDateTime**</span><span class="sxs-lookup"><span data-stu-id="e4ffe-135">**expirationDateTime**</span></span> | <span data-ttu-id="e4ffe-136">string</span><span class="sxs-lookup"><span data-stu-id="e4ffe-136">string</span></span> | <span data-ttu-id="e4ffe-137">Uma cadeia de caracteres com formato yyyy-MM-ddTHH:mm:ssZ de DateTime indica a hora de expiração da permissão.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-137">A String with format of yyyy-MM-ddTHH:mm:ssZ of DateTime indicates the expiration time of the permission.</span></span> |
| <span data-ttu-id="e4ffe-138">**scope**</span><span class="sxs-lookup"><span data-stu-id="e4ffe-138">**scope**</span></span> | <span data-ttu-id="e4ffe-139">string</span><span class="sxs-lookup"><span data-stu-id="e4ffe-139">string</span></span> | <span data-ttu-id="e4ffe-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-140">Optional.</span></span> <span data-ttu-id="e4ffe-141">O escopo do link a ser criado.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-141">The scope of link to create.</span></span> <span data-ttu-id="e4ffe-142">Pode ser `anonymous` ou `organization`.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-142">Either `anonymous` or `organization`.</span></span> |


### <a name="link-types"></a><span data-ttu-id="e4ffe-143">Tipos de link</span><span class="sxs-lookup"><span data-stu-id="e4ffe-143">Link types</span></span>

<span data-ttu-id="e4ffe-144">Os seguintes valores são permitidos para o parâmetro **type**.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-144">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="e4ffe-145">Valor do tipo</span><span class="sxs-lookup"><span data-stu-id="e4ffe-145">Type value</span></span> | <span data-ttu-id="e4ffe-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4ffe-146">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="e4ffe-147">Cria um link somente leitura para DriveItem.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-147">Creates a read-only link to the DriveItem.</span></span>                                                        |
| `edit`     | <span data-ttu-id="e4ffe-148">Cria um link de leitura e gravação para DriveItem.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-148">Creates a read-write link to the DriveItem.</span></span>                                                       |
| `embed`    | <span data-ttu-id="e4ffe-149">Cria um link incorporado para DriveItem.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-149">Creates an embeddable link to the DriveItem.</span></span> <span data-ttu-id="e4ffe-150">Essa opção só está disponível para arquivos no OneDrive Pessoal.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-150">This option is only available for files in OneDrive personal.</span></span> |

### <a name="scope-types"></a><span data-ttu-id="e4ffe-151">Tipos de escopo</span><span class="sxs-lookup"><span data-stu-id="e4ffe-151">Scope types</span></span>

<span data-ttu-id="e4ffe-152">Os seguintes valores são permitidos para o parâmetro **scope**.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-152">The following values are allowed for the **scope** parameter.</span></span>
<span data-ttu-id="e4ffe-153">Se o parâmetro **scope** não for especificado, o tipo de link padrão será criado para a organização.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-153">If the **scope** parameter is not specified, the default link type for the organization is created.</span></span>

| <span data-ttu-id="e4ffe-154">Valor</span><span class="sxs-lookup"><span data-stu-id="e4ffe-154">Value</span></span>          | <span data-ttu-id="e4ffe-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4ffe-155">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="e4ffe-156">Qualquer pessoa com o link tem acesso, sem precisar fazer logon.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-156">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="e4ffe-157">Isso pode incluir pessoas de fora da organização.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-157">This may include people outside of your organization.</span></span> <span data-ttu-id="e4ffe-158">O suporte para links anônimos pode ser desativado por um administrador.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-158">Anonymous link support may be disabled by an administrator.</span></span>
| `organization` | <span data-ttu-id="e4ffe-159">Qualquer pessoa que tenha feito logon em sua organização (locatário) pode usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-159">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="e4ffe-160">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-160">Only available in OneDrive for Business and SharePoint.</span></span>


## <a name="response"></a><span data-ttu-id="e4ffe-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4ffe-161">Response</span></span>

<span data-ttu-id="e4ffe-162">Se for bem-sucedido, esse método retornará um único recurso [Permission](../resources/permission.md) no corpo da resposta, que representa as permissões de compartilhamento solicitadas.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-162">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="e4ffe-163">A resposta será `201 Created` se um novo link de compartilhamento for criado para o item ou `200 OK` se um link existente for retornado.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-163">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="e4ffe-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4ffe-164">Example</span></span>

<span data-ttu-id="e4ffe-165">O exemplo a seguir solicita um link de compartilhamento que será criado para o DriveItem especificado por {itemId} no OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-165">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="e4ffe-166">O link de compartilhamento é configurado como somente leitura e utilizável por qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-166">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

### <a name="request"></a><span data-ttu-id="e4ffe-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4ffe-167">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e4ffe-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4ffe-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-link"
}-->

```http
POST /me/drive/items/{item-id}/createLink
Content-type: application/json

{
  "type": "view",
  "password": "ThisIsMyPrivatePassword",
  "scope": "anonymous"
}
```
# <a name="c"></a>[<span data-ttu-id="e4ffe-169">C#</span><span class="sxs-lookup"><span data-stu-id="e4ffe-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4ffe-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4ffe-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4ffe-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4ffe-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4ffe-172">Java</span><span class="sxs-lookup"><span data-stu-id="e4ffe-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-link-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e4ffe-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4ffe-173">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  },
  "hasPassword": true
}
```

## <a name="creating-company-sharable-links"></a><span data-ttu-id="e4ffe-174">Criando links compartilháveis pela empresa</span><span class="sxs-lookup"><span data-stu-id="e4ffe-174">Creating company sharable links</span></span>

<span data-ttu-id="e4ffe-175">O OneDrive for Business e o SharePoint oferecem suporte a links compartilháveis pela empresa.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-175">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="e4ffe-176">Estes são semelhantes a links anônimos, com a diferença de que apenas funcionam para membros da organização proprietária.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-176">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="e4ffe-177">Para criar um link compartilhável pela empresa, use o parâmetro **scope** com um valor de `organization`.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-177">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

### <a name="request"></a><span data-ttu-id="e4ffe-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4ffe-178">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e4ffe-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4ffe-179">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite", "tags": "service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```
# <a name="c"></a>[<span data-ttu-id="e4ffe-180">C#</span><span class="sxs-lookup"><span data-stu-id="e4ffe-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-scoped-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4ffe-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4ffe-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-scoped-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4ffe-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4ffe-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-scoped-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4ffe-183">Java</span><span class="sxs-lookup"><span data-stu-id="e4ffe-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-link-scoped-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e4ffe-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4ffe-184">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  },
}
```

## <a name="creating-embeddable-links"></a><span data-ttu-id="e4ffe-185">Criar links inseríveis</span><span class="sxs-lookup"><span data-stu-id="e4ffe-185">Creating embeddable links</span></span>

<span data-ttu-id="e4ffe-p113">Ao usar o tipo de link `embed`, a webUrl retornada pode ser inserida em um elemento HTML `<iframe>`. Quando um link de inserção é criado, a propriedade `webHtml` contém o código HTML de um `<iframe>` para hospedar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-p113">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="e4ffe-188">**Observação:** os links de inseridos só tem suporte no OneDrive Pessoal.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-188">**Note:** Embed links are only supported for OneDrive personal.</span></span>

### <a name="request"></a><span data-ttu-id="e4ffe-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4ffe-189">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e4ffe-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4ffe-190">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite", "tags": "service.onedrive service.graph" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```
# <a name="c"></a>[<span data-ttu-id="e4ffe-191">C#</span><span class="sxs-lookup"><span data-stu-id="e4ffe-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-embedded-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4ffe-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4ffe-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-embedded-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4ffe-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4ffe-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-embedded-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4ffe-194">Java</span><span class="sxs-lookup"><span data-stu-id="e4ffe-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-embedded-link-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e4ffe-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4ffe-195">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["read"],
  "link": {
    "type": "embed",
    "webHtml": "<IFRAME src=\"https://onedrive.live.com/...\"></IFRAME>",
    "webUrl": "https://onedrive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a><span data-ttu-id="e4ffe-196">Comentários</span><span class="sxs-lookup"><span data-stu-id="e4ffe-196">Remarks</span></span>

* <span data-ttu-id="e4ffe-197">Links criados usando esta ação não expiram, a menos que uma política de expiração padrão seja imposta à organização.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-197">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="e4ffe-198">Os links ficam visíveis nas permissões de compartilhamento do item e podem ser removidos por um proprietário desse item.</span><span class="sxs-lookup"><span data-stu-id="e4ffe-198">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="e4ffe-199">Os links sempre apontam para a versão atual de um item, a menos que esse item esteja em check-out (apenas no SharePoint).</span><span class="sxs-lookup"><span data-stu-id="e4ffe-199">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
} -->

