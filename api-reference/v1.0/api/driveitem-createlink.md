---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Compartilhar um arquivo com um link
ms.openlocfilehash: b65efe24534d5b366f25241bea79c70967fbb73e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005522"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="2c9c8-102">Criar um link de compartilhamento para um DriveItem</span><span class="sxs-lookup"><span data-stu-id="2c9c8-102">Create a sharing link for a DriveItem</span></span>

<span data-ttu-id="2c9c8-103">Você pode usar a ação **createLink** para compartilhar um [DriveItem](../resources/driveitem.md) por meio de um link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-103">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="2c9c8-p101">A ação **createLink** criará um novo link de compartilhamento se o tipo de link especificado não existir para o aplicativo de chamada. Se um link de compartilhamento do tipo especificado já existir para o aplicativo, o link de compartilhamento existente será retornado.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="2c9c8-106">Recursos de DriveItem herdam permissões de compartilhamento de seus ancestrais.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-106">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c9c8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c9c8-107">Permissions</span></span>

<span data-ttu-id="2c9c8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c9c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c9c8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c9c8-110">Permission type</span></span>      | <span data-ttu-id="2c9c8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c9c8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c9c8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c9c8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2c9c8-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c9c8-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c9c8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c9c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c9c8-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c9c8-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c9c8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c9c8-116">Application</span></span> | <span data-ttu-id="2c9c8-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c9c8-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c9c8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c9c8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a><span data-ttu-id="2c9c8-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c9c8-119">Request body</span></span>

<span data-ttu-id="2c9c8-120">O corpo da solicitação define as propriedades do link de compartilhamento que seu aplicativo está solicitando.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-120">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="2c9c8-121">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-121">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="2c9c8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2c9c8-122">Name</span></span>    |  <span data-ttu-id="2c9c8-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c9c8-123">Type</span></span>  |                                 <span data-ttu-id="2c9c8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c9c8-124">Description</span></span>                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="2c9c8-125">**type**</span><span class="sxs-lookup"><span data-stu-id="2c9c8-125">**type**</span></span>  | <span data-ttu-id="2c9c8-126">string</span><span class="sxs-lookup"><span data-stu-id="2c9c8-126">string</span></span> | <span data-ttu-id="2c9c8-p104">O tipo de link de compartilhamento a ser criado. Pode ser `view`, `edit` ou `embed`.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-p104">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="2c9c8-129">**scope**</span><span class="sxs-lookup"><span data-stu-id="2c9c8-129">**scope**</span></span> | <span data-ttu-id="2c9c8-130">string</span><span class="sxs-lookup"><span data-stu-id="2c9c8-130">string</span></span> | <span data-ttu-id="2c9c8-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-131">Optional.</span></span> <span data-ttu-id="2c9c8-132">O escopo do link a ser criado.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-132">The scope of link to create.</span></span> <span data-ttu-id="2c9c8-133">Pode ser `anonymous` ou `organization`.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-133">Either `anonymous` or `organization`.</span></span> |


### <a name="link-types"></a><span data-ttu-id="2c9c8-134">Tipos de link</span><span class="sxs-lookup"><span data-stu-id="2c9c8-134">Link types</span></span>

<span data-ttu-id="2c9c8-135">Os seguintes valores são permitidos para o parâmetro **type**.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-135">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="2c9c8-136">Valor do tipo</span><span class="sxs-lookup"><span data-stu-id="2c9c8-136">Type value</span></span> | <span data-ttu-id="2c9c8-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c9c8-137">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="2c9c8-138">Cria um link somente leitura para DriveItem.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-138">Creates a read-only link to the DriveItem.</span></span>                                                        |
| `edit`     | <span data-ttu-id="2c9c8-139">Cria um link de leitura e gravação para DriveItem.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-139">Creates a read-write link to the DriveItem.</span></span>                                                       |
| `embed`    | <span data-ttu-id="2c9c8-140">Cria um link incorporado para DriveItem.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-140">Creates an embeddable link to the DriveItem.</span></span> <span data-ttu-id="2c9c8-141">Essa opção só está disponível para arquivos no OneDrive Pessoal.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-141">This option is only available for files in OneDrive personal.</span></span> |

### <a name="scope-types"></a><span data-ttu-id="2c9c8-142">Tipos de escopo</span><span class="sxs-lookup"><span data-stu-id="2c9c8-142">Scope types</span></span>

<span data-ttu-id="2c9c8-143">Os seguintes valores são permitidos para o parâmetro **scope**.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-143">The following values are allowed for the **scope** parameter.</span></span>
<span data-ttu-id="2c9c8-144">Se o parâmetro **scope** não for especificado, o tipo de link padrão será criado para a organização.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-144">If the **scope** parameter is not specified, the default link type for the organization is created.</span></span>

| <span data-ttu-id="2c9c8-145">Valor</span><span class="sxs-lookup"><span data-stu-id="2c9c8-145">Value</span></span>          | <span data-ttu-id="2c9c8-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c9c8-146">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="2c9c8-147">Qualquer pessoa com o link possui acesso, sem precisar entrar.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-147">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="2c9c8-148">Isso pode incluir pessoas fora da sua organização.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-148">This may include people outside of your organization.</span></span> <span data-ttu-id="2c9c8-149">Suporte ao link anônimos pode ser desabilitado por um administrador.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-149">Anonymous link support may be disabled by an administrator.</span></span>
| `organization` | <span data-ttu-id="2c9c8-150">Qualquer pessoa entrado na sua organização (inquilino) pode usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-150">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="2c9c8-151">Disponível somente no OneDrive for Business e o SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-151">Only available in OneDrive for Business and SharePoint.</span></span>


## <a name="response"></a><span data-ttu-id="2c9c8-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c9c8-152">Response</span></span>

<span data-ttu-id="2c9c8-153">Se for bem-sucedido, esse método retornará um único recurso [Permission](../resources/permission.md) no corpo da resposta, que representa as permissões de compartilhamento solicitadas.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-153">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="2c9c8-154">A resposta será `201 Created` se um novo link de compartilhamento for criado para o item ou `200 OK` se um link existente for retornado.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-154">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="2c9c8-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c9c8-155">Example</span></span>

<span data-ttu-id="2c9c8-156">O exemplo a seguir solicita um link de compartilhamento que será criado para o DriveItem especificado por {itemId} no OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-156">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="2c9c8-157">O link de compartilhamento é configurado como somente leitura e utilizável por qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-157">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

### <a name="request"></a><span data-ttu-id="2c9c8-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c9c8-158">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create-link"
}-->

```http
POST /me/drive/items/{item-id}/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

### <a name="response"></a><span data-ttu-id="2c9c8-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c9c8-159">Response</span></span>

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

## <a name="creating-company-sharable-links"></a><span data-ttu-id="2c9c8-160">Criando links compartilháveis pela empresa</span><span class="sxs-lookup"><span data-stu-id="2c9c8-160">Creating company sharable links</span></span>

<span data-ttu-id="2c9c8-161">O OneDrive for Business e o SharePoint oferecem suporte a links compartilháveis pela empresa.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-161">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="2c9c8-162">Estes são semelhantes a links anônimos, com a diferença de que apenas funcionam para membros da organização proprietária.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-162">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="2c9c8-163">Para criar um link compartilhável pela empresa, use o parâmetro **scope** com um valor de `organization`.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-163">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

### <a name="request"></a><span data-ttu-id="2c9c8-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c9c8-164">Request</span></span>

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite", "tags": "service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

### <a name="response"></a><span data-ttu-id="2c9c8-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c9c8-165">Response</span></span>

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

## <a name="creating-embeddable-links"></a><span data-ttu-id="2c9c8-166">Criar links inseríveis</span><span class="sxs-lookup"><span data-stu-id="2c9c8-166">Creating embeddable links</span></span>

<span data-ttu-id="2c9c8-p112">Ao usar o tipo de link `embed`, a webUrl retornada pode ser inserida em um elemento HTML `<iframe>`. Quando um link de inserção é criado, a propriedade `webHtml` contém o código HTML de um `<iframe>` para hospedar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-p112">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="2c9c8-169">**Observação:** os links de inseridos só tem suporte no OneDrive Pessoal.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-169">**Note:** Embed links are only supported for OneDrive personal.</span></span>

### <a name="request"></a><span data-ttu-id="2c9c8-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c9c8-170">Request</span></span>

<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite", "tags": "service.onedrive service.graph" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

### <a name="response"></a><span data-ttu-id="2c9c8-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c9c8-171">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="2c9c8-172">Comentários</span><span class="sxs-lookup"><span data-stu-id="2c9c8-172">Remarks</span></span>

* <span data-ttu-id="2c9c8-173">Links criados usando esta ação não expiram, a menos que uma política de expiração padrão seja imposta à organização.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-173">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="2c9c8-174">Os links ficam visíveis nas permissões de compartilhamento do item e podem ser removidos por um proprietário desse item.</span><span class="sxs-lookup"><span data-stu-id="2c9c8-174">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="2c9c8-175">Os links sempre apontam para a versão atual de um item, a menos que esse item esteja em check-out (apenas no SharePoint).</span><span class="sxs-lookup"><span data-stu-id="2c9c8-175">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link"
} -->
