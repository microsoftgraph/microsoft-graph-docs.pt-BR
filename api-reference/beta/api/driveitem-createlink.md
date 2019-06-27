---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Compartilhar um arquivo com um link
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: da6b1972d029b9e780575b1bf985f4d3c9d6d906
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260227"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="15ece-102">Criar um link de compartilhamento para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="15ece-102">Create a sharing link for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15ece-103">Você pode usar a ação **createLink** para compartilhar um [DriveItem](../resources/driveitem.md) por meio de um link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="15ece-103">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="15ece-p101">A ação **createLink** criará um novo link de compartilhamento se o tipo de link especificado não existir para o aplicativo de chamada. Se um link de compartilhamento do tipo especificado já existir para o aplicativo, o link de compartilhamento existente será retornado.</span><span class="sxs-lookup"><span data-stu-id="15ece-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="15ece-106">Recursos de DriveItem herdam permissões de compartilhamento de seus ancestrais.</span><span class="sxs-lookup"><span data-stu-id="15ece-106">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="15ece-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="15ece-107">Permissions</span></span>

<span data-ttu-id="15ece-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15ece-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15ece-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15ece-110">Permission type</span></span>      | <span data-ttu-id="15ece-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15ece-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15ece-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15ece-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15ece-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15ece-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="15ece-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15ece-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15ece-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15ece-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="15ece-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15ece-116">Application</span></span> | <span data-ttu-id="15ece-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15ece-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15ece-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15ece-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a><span data-ttu-id="15ece-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15ece-119">Request body</span></span>

<span data-ttu-id="15ece-120">O corpo da solicitação define as propriedades do link de compartilhamento que seu aplicativo está solicitando.</span><span class="sxs-lookup"><span data-stu-id="15ece-120">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="15ece-121">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="15ece-121">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="15ece-122">Nome</span><span class="sxs-lookup"><span data-stu-id="15ece-122">Name</span></span>    |  <span data-ttu-id="15ece-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="15ece-123">Type</span></span>  |                                 <span data-ttu-id="15ece-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="15ece-124">Description</span></span>                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="15ece-125">**type**</span><span class="sxs-lookup"><span data-stu-id="15ece-125">**type**</span></span>  | <span data-ttu-id="15ece-126">string</span><span class="sxs-lookup"><span data-stu-id="15ece-126">string</span></span> | <span data-ttu-id="15ece-p104">O tipo de link de compartilhamento a ser criado. Pode ser `view`, `edit` ou `embed`.</span><span class="sxs-lookup"><span data-stu-id="15ece-p104">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="15ece-129">**scope**</span><span class="sxs-lookup"><span data-stu-id="15ece-129">**scope**</span></span> | <span data-ttu-id="15ece-130">string</span><span class="sxs-lookup"><span data-stu-id="15ece-130">string</span></span> | <span data-ttu-id="15ece-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="15ece-131">Optional.</span></span> <span data-ttu-id="15ece-132">O escopo do link a ser criado.</span><span class="sxs-lookup"><span data-stu-id="15ece-132">The scope of link to create.</span></span> <span data-ttu-id="15ece-133">Pode ser `anonymous` ou `organization`.</span><span class="sxs-lookup"><span data-stu-id="15ece-133">Either `anonymous` or `organization`.</span></span> |


### <a name="link-types"></a><span data-ttu-id="15ece-134">Tipos de link</span><span class="sxs-lookup"><span data-stu-id="15ece-134">Link types</span></span>

<span data-ttu-id="15ece-135">Os seguintes valores são permitidos para o parâmetro **type**.</span><span class="sxs-lookup"><span data-stu-id="15ece-135">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="15ece-136">Valor do tipo</span><span class="sxs-lookup"><span data-stu-id="15ece-136">Type value</span></span> | <span data-ttu-id="15ece-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="15ece-137">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="15ece-138">Cria um link somente leitura para DriveItem.</span><span class="sxs-lookup"><span data-stu-id="15ece-138">Creates a read-only link to the DriveItem.</span></span>                                                        |
| `edit`     | <span data-ttu-id="15ece-139">Cria um link de leitura e gravação para DriveItem.</span><span class="sxs-lookup"><span data-stu-id="15ece-139">Creates a read-write link to the DriveItem.</span></span>                                                       |
| `embed`    | <span data-ttu-id="15ece-140">Cria um link incorporado para DriveItem.</span><span class="sxs-lookup"><span data-stu-id="15ece-140">Creates an embeddable link to the DriveItem.</span></span> <span data-ttu-id="15ece-141">Essa opção só está disponível para arquivos no OneDrive Pessoal.</span><span class="sxs-lookup"><span data-stu-id="15ece-141">This option is only available for files in OneDrive personal.</span></span> |

### <a name="scope-types"></a><span data-ttu-id="15ece-142">Tipos de escopo</span><span class="sxs-lookup"><span data-stu-id="15ece-142">Scope types</span></span>

<span data-ttu-id="15ece-143">Os seguintes valores são permitidos para o parâmetro **scope**.</span><span class="sxs-lookup"><span data-stu-id="15ece-143">The following values are allowed for the **scope** parameter.</span></span>
<span data-ttu-id="15ece-144">Se o parâmetro **scope** não for especificado, o tipo de link padrão será criado para a organização.</span><span class="sxs-lookup"><span data-stu-id="15ece-144">If the **scope** parameter is not specified, the default link type for the organization is created.</span></span>

| <span data-ttu-id="15ece-145">Valor do tipo</span><span class="sxs-lookup"><span data-stu-id="15ece-145">Type value</span></span>     | <span data-ttu-id="15ece-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="15ece-146">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="15ece-147">Cria um link para o DriveItem, que pode ser acessado por qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="15ece-147">Creates a link to the DriveItem accessible to anyone with the link.</span></span> <span data-ttu-id="15ece-148">Links anônimos podem ser desabilitados por um administrador.</span><span class="sxs-lookup"><span data-stu-id="15ece-148">Anonymous links may be disabled by an administrator.</span></span>                 |
| `organization` | <span data-ttu-id="15ece-149">Cria um link para o DriveItem, que pode ser acessado por qualquer pessoa dentro da organização do usuário.</span><span class="sxs-lookup"><span data-stu-id="15ece-149">Creates a link to the DriveItem accessible to anyone within the user's organization.</span></span> <span data-ttu-id="15ece-150">O escopo do link da organização não está disponível para uso pessoal do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="15ece-150">Organization link scope is not available for OneDrive personal.</span></span> |

## <a name="response"></a><span data-ttu-id="15ece-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="15ece-151">Response</span></span>

<span data-ttu-id="15ece-152">Se for bem-sucedido, esse método retornará um único recurso [Permission](../resources/permission.md) no corpo da resposta, que representa as permissões de compartilhamento solicitadas.</span><span class="sxs-lookup"><span data-stu-id="15ece-152">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="15ece-153">A resposta será `201 Created` se um novo link de compartilhamento for criado para o item ou `200 OK` se um link existente for retornado.</span><span class="sxs-lookup"><span data-stu-id="15ece-153">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="15ece-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15ece-154">Example</span></span>

<span data-ttu-id="15ece-155">O exemplo a seguir solicita um link de compartilhamento que será criado para o DriveItem especificado por {itemId} no OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="15ece-155">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="15ece-156">O link de compartilhamento é configurado como somente leitura e utilizável por qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="15ece-156">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

### <a name="request"></a><span data-ttu-id="15ece-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15ece-157">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

### <a name="response"></a><span data-ttu-id="15ece-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="15ece-158">Response</span></span>

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
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="15ece-159">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="15ece-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="15ece-160">C#</span><span class="sxs-lookup"><span data-stu-id="15ece-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/item_createlink-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15ece-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="15ece-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/item_createlink-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="15ece-162">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="15ece-162">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/item_createlink-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="creating-company-sharable-links"></a><span data-ttu-id="15ece-163">Criando links compartilháveis pela empresa</span><span class="sxs-lookup"><span data-stu-id="15ece-163">Creating company sharable links</span></span>

<span data-ttu-id="15ece-164">O OneDrive for Business e o SharePoint oferecem suporte a links compartilháveis pela empresa.</span><span class="sxs-lookup"><span data-stu-id="15ece-164">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="15ece-165">Estes são semelhantes a links anônimos, com a diferença de que apenas funcionam para membros da organização proprietária.</span><span class="sxs-lookup"><span data-stu-id="15ece-165">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="15ece-166">Para criar um link compartilhável pela empresa, use o parâmetro **scope** com um valor de `organization`.</span><span class="sxs-lookup"><span data-stu-id="15ece-166">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

### <a name="request"></a><span data-ttu-id="15ece-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15ece-167">Request</span></span>

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

### <a name="response"></a><span data-ttu-id="15ece-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="15ece-168">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="15ece-169">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="15ece-169">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="15ece-170">C#</span><span class="sxs-lookup"><span data-stu-id="15ece-170">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-link-scoped-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15ece-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="15ece-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-link-scoped-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="15ece-172">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="15ece-172">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-link-scoped-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="creating-embeddable-links"></a><span data-ttu-id="15ece-173">Criar links inseríveis</span><span class="sxs-lookup"><span data-stu-id="15ece-173">Creating embeddable links</span></span>

<span data-ttu-id="15ece-p112">Ao usar o tipo de link `embed`, a webUrl retornada pode ser inserida em um elemento HTML `<iframe>`. Quando um link de inserção é criado, a propriedade `webHtml` contém o código HTML de um `<iframe>` para hospedar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="15ece-p112">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="15ece-176">**Observação:** os links de inseridos só tem suporte no OneDrive Pessoal.</span><span class="sxs-lookup"><span data-stu-id="15ece-176">**Note:** Embed links are only supported for OneDrive personal.</span></span>

### <a name="request"></a><span data-ttu-id="15ece-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15ece-177">Request</span></span>

<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite service.onedrive" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

### <a name="response"></a><span data-ttu-id="15ece-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="15ece-178">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="15ece-179">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="15ece-179">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="15ece-180">C#</span><span class="sxs-lookup"><span data-stu-id="15ece-180">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-embedded-link-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15ece-181">Javascript</span><span class="sxs-lookup"><span data-stu-id="15ece-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-embedded-link-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="15ece-182">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="15ece-182">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-embedded-link-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="15ece-183">Comentários</span><span class="sxs-lookup"><span data-stu-id="15ece-183">Remarks</span></span>

* <span data-ttu-id="15ece-184">Links criados usando esta ação não expiram, a menos que uma política de expiração padrão seja imposta à organização.</span><span class="sxs-lookup"><span data-stu-id="15ece-184">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="15ece-185">Os links ficam visíveis nas permissões de compartilhamento do item e podem ser removidos por um proprietário desse item.</span><span class="sxs-lookup"><span data-stu-id="15ece-185">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="15ece-186">Os links sempre apontam para a versão atual de um item, a menos que esse item esteja em check-out (apenas no SharePoint).</span><span class="sxs-lookup"><span data-stu-id="15ece-186">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
