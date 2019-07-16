---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Compartilhar um arquivo com um link
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 249b67852d4b796be465c79cadde9b07d97f695a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713139"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="8d1b0-102">Criar um link de compartilhamento para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="8d1b0-102">Create a sharing link for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d1b0-103">Você pode usar a ação **createLink** para compartilhar um [DriveItem](../resources/driveitem.md) por meio de um link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-103">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="8d1b0-p101">A ação **createLink** criará um novo link de compartilhamento se o tipo de link especificado não existir para o aplicativo de chamada. Se um link de compartilhamento do tipo especificado já existir para o aplicativo, o link de compartilhamento existente será retornado.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="8d1b0-106">Recursos de DriveItem herdam permissões de compartilhamento de seus ancestrais.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-106">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d1b0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d1b0-107">Permissions</span></span>

<span data-ttu-id="8d1b0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d1b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d1b0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d1b0-110">Permission type</span></span>      | <span data-ttu-id="8d1b0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d1b0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d1b0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d1b0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8d1b0-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d1b0-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8d1b0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d1b0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d1b0-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d1b0-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8d1b0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d1b0-116">Application</span></span> | <span data-ttu-id="8d1b0-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d1b0-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d1b0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d1b0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a><span data-ttu-id="8d1b0-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d1b0-119">Request body</span></span>

<span data-ttu-id="8d1b0-120">O corpo da solicitação define as propriedades do link de compartilhamento que seu aplicativo está solicitando.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-120">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="8d1b0-121">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-121">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="8d1b0-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d1b0-122">Property</span></span>                 |  <span data-ttu-id="8d1b0-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d1b0-123">Type</span></span>  |                                 <span data-ttu-id="8d1b0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d1b0-124">Description</span></span>                                                               |
| :----------------------| :----- | :---------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="8d1b0-125">type</span><span class="sxs-lookup"><span data-stu-id="8d1b0-125">type</span></span>               | <span data-ttu-id="8d1b0-126">string</span><span class="sxs-lookup"><span data-stu-id="8d1b0-126">string</span></span> | <span data-ttu-id="8d1b0-127">O tipo de link de compartilhamento a ser criado.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-127">The type of sharing link to create.</span></span> <span data-ttu-id="8d1b0-128">Exibir, editar ou incorporar.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-128">Either view, edit, or embed.</span></span>                                    |
|<span data-ttu-id="8d1b0-129">password</span><span class="sxs-lookup"><span data-stu-id="8d1b0-129">password</span></span>           | <span data-ttu-id="8d1b0-130">string</span><span class="sxs-lookup"><span data-stu-id="8d1b0-130">string</span></span> | <span data-ttu-id="8d1b0-131">A senha do link de compartilhamento que é definida pelo criador.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-131">The password of the sharing link that is set by the creator.</span></span> <span data-ttu-id="8d1b0-132">Opcional e o OneDrive somente pessoal.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-132">Optional and OneDrive Personal only.</span></span>         |
|<span data-ttu-id="8d1b0-133">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8d1b0-133">expirationDateTime</span></span> | <span data-ttu-id="8d1b0-134">string</span><span class="sxs-lookup"><span data-stu-id="8d1b0-134">string</span></span> | <span data-ttu-id="8d1b0-135">Uma cadeia de caracteres com formato AAAA-MM-ddTHH: mm: ssZ de DateTime indica o tempo de expiração da permissão.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-135">A String with format of yyyy-MM-ddTHH:mm:ssZ of DateTime indicates the expiration time of the permission.</span></span> |
|<span data-ttu-id="8d1b0-136">escopo</span><span class="sxs-lookup"><span data-stu-id="8d1b0-136">scope</span></span>              | <span data-ttu-id="8d1b0-137">string</span><span class="sxs-lookup"><span data-stu-id="8d1b0-137">string</span></span> | <span data-ttu-id="8d1b0-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-138">Optional.</span></span> <span data-ttu-id="8d1b0-139">O escopo do link a ser criado.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-139">The scope of link to create.</span></span> <span data-ttu-id="8d1b0-140">Anônimo ou organização.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-140">Either anonymous or organization.</span></span>                              |


### <a name="link-types"></a><span data-ttu-id="8d1b0-141">Tipos de link</span><span class="sxs-lookup"><span data-stu-id="8d1b0-141">Link types</span></span>

<span data-ttu-id="8d1b0-142">Os seguintes valores são permitidos para o parâmetro **type**.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-142">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="8d1b0-143">Valor do tipo</span><span class="sxs-lookup"><span data-stu-id="8d1b0-143">Type value</span></span> | <span data-ttu-id="8d1b0-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d1b0-144">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| <span data-ttu-id="8d1b0-145">modo de exibição</span><span class="sxs-lookup"><span data-stu-id="8d1b0-145">view</span></span>     | <span data-ttu-id="8d1b0-146">Cria um link somente leitura para DriveItem.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-146">Creates a read-only link to the DriveItem.</span></span>                                                        |
| <span data-ttu-id="8d1b0-147">edit</span><span class="sxs-lookup"><span data-stu-id="8d1b0-147">edit</span></span>     | <span data-ttu-id="8d1b0-148">Cria um link de leitura e gravação para DriveItem.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-148">Creates a read-write link to the DriveItem.</span></span>                                                       |
| <span data-ttu-id="8d1b0-149">Incorporar</span><span class="sxs-lookup"><span data-stu-id="8d1b0-149">embed</span></span>    | <span data-ttu-id="8d1b0-150">Cria um link incorporado para DriveItem.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-150">Creates an embeddable link to the DriveItem.</span></span> <span data-ttu-id="8d1b0-151">Essa opção só está disponível para arquivos no OneDrive Pessoal.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-151">This option is only available for files in OneDrive personal.</span></span> |

### <a name="scope-types"></a><span data-ttu-id="8d1b0-152">Tipos de escopo</span><span class="sxs-lookup"><span data-stu-id="8d1b0-152">Scope types</span></span>

<span data-ttu-id="8d1b0-153">Os seguintes valores são permitidos para o parâmetro **scope**.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-153">The following values are allowed for the **scope** parameter.</span></span>
<span data-ttu-id="8d1b0-154">Se o parâmetro **scope** não for especificado, o tipo de link padrão será criado para a organização.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-154">If the **scope** parameter is not specified, the default link type for the organization is created.</span></span>

| <span data-ttu-id="8d1b0-155">Valor</span><span class="sxs-lookup"><span data-stu-id="8d1b0-155">Value</span></span>          | <span data-ttu-id="8d1b0-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d1b0-156">Description</span></span>
|:---------------|:------------------------------------------------------------
| <span data-ttu-id="8d1b0-157">sejam</span><span class="sxs-lookup"><span data-stu-id="8d1b0-157">anonymous</span></span>    | <span data-ttu-id="8d1b0-158">Qualquer pessoa com o link tem acesso, sem a necessidade de fazer logon.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-158">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="8d1b0-159">Isso pode incluir pessoas de fora da sua organização.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-159">This may include people outside of your organization.</span></span> <span data-ttu-id="8d1b0-160">O suporte a link anônimo pode ser desabilitado por um administrador.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-160">Anonymous link support may be disabled by an administrator.</span></span>
| <span data-ttu-id="8d1b0-161">organization</span><span class="sxs-lookup"><span data-stu-id="8d1b0-161">organization</span></span> | <span data-ttu-id="8d1b0-162">Qualquer pessoa que se inscreveu em sua organização (locatário) pode usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-162">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="8d1b0-163">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-163">Only available in OneDrive for Business and SharePoint.</span></span>


## <a name="response"></a><span data-ttu-id="8d1b0-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d1b0-164">Response</span></span>

<span data-ttu-id="8d1b0-165">Se for bem-sucedido, esse método retornará um único recurso [Permission](../resources/permission.md) no corpo da resposta, que representa as permissões de compartilhamento solicitadas.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-165">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="8d1b0-166">A resposta será `201 Created` se um novo link de compartilhamento for criado para o item ou `200 OK` se um link existente for retornado.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-166">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="8d1b0-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d1b0-167">Example</span></span>

<span data-ttu-id="8d1b0-168">O exemplo a seguir solicita um link de compartilhamento que será criado para o DriveItem especificado por {itemId} no OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-168">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="8d1b0-169">O link de compartilhamento é configurado como somente leitura e utilizável por qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-169">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

### <a name="request"></a><span data-ttu-id="8d1b0-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d1b0-170">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8d1b0-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d1b0-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-type: application/json

{
  "type": "view",
  "password": "ThisIsMyPrivatePassword",
  "scope": "anonymous"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8d1b0-172">C#</span><span class="sxs-lookup"><span data-stu-id="8d1b0-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-createlink-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d1b0-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="8d1b0-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-createlink-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8d1b0-174">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8d1b0-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-createlink-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8d1b0-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d1b0-175">Response</span></span>

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

## <a name="creating-company-sharable-links"></a><span data-ttu-id="8d1b0-176">Criando links compartilháveis pela empresa</span><span class="sxs-lookup"><span data-stu-id="8d1b0-176">Creating company sharable links</span></span>

<span data-ttu-id="8d1b0-177">O OneDrive for Business e o SharePoint oferecem suporte a links compartilháveis pela empresa.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-177">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="8d1b0-178">Estes são semelhantes a links anônimos, com a diferença de que apenas funcionam para membros da organização proprietária.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-178">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="8d1b0-179">Para criar um link compartilhável pela empresa, use o parâmetro **scope** com um valor de `organization`.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-179">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

### <a name="request"></a><span data-ttu-id="8d1b0-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d1b0-180">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8d1b0-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d1b0-181">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8d1b0-182">C#</span><span class="sxs-lookup"><span data-stu-id="8d1b0-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-scoped-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d1b0-183">Javascript</span><span class="sxs-lookup"><span data-stu-id="8d1b0-183">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-scoped-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8d1b0-184">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8d1b0-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-scoped-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8d1b0-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d1b0-185">Response</span></span>

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
  }
}
```

## <a name="creating-embeddable-links"></a><span data-ttu-id="8d1b0-186">Criar links inseríveis</span><span class="sxs-lookup"><span data-stu-id="8d1b0-186">Creating embeddable links</span></span>

<span data-ttu-id="8d1b0-p113">Ao usar o tipo de link `embed`, a webUrl retornada pode ser inserida em um elemento HTML `<iframe>`. Quando um link de inserção é criado, a propriedade `webHtml` contém o código HTML de um `<iframe>` para hospedar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-p113">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="8d1b0-189">**Observação:** os links de inseridos só tem suporte no OneDrive Pessoal.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-189">**Note:** Embed links are only supported for OneDrive personal.</span></span>

### <a name="request"></a><span data-ttu-id="8d1b0-190">Solicitar</span><span class="sxs-lookup"><span data-stu-id="8d1b0-190">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8d1b0-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d1b0-191">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite service.onedrive" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8d1b0-192">C#</span><span class="sxs-lookup"><span data-stu-id="8d1b0-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-embedded-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d1b0-193">Javascript</span><span class="sxs-lookup"><span data-stu-id="8d1b0-193">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-embedded-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8d1b0-194">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8d1b0-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-embedded-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8d1b0-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d1b0-195">Response</span></span>

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
    "webUrl": "https://onedive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a><span data-ttu-id="8d1b0-196">Comentários</span><span class="sxs-lookup"><span data-stu-id="8d1b0-196">Remarks</span></span>

* <span data-ttu-id="8d1b0-197">Links criados usando esta ação não expiram, a menos que uma política de expiração padrão seja imposta à organização.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-197">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="8d1b0-198">Os links ficam visíveis nas permissões de compartilhamento do item e podem ser removidos por um proprietário desse item.</span><span class="sxs-lookup"><span data-stu-id="8d1b0-198">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="8d1b0-199">Os links sempre apontam para a versão atual de um item, a menos que esse item esteja em check-out (apenas no SharePoint).</span><span class="sxs-lookup"><span data-stu-id="8d1b0-199">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
}
-->
