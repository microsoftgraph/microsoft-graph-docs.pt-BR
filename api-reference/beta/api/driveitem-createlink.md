---
author: JeremyKelley
description: Você pode usar a ação createLink para compartilhar um DriveItem por meio de um link de compartilhamento.
title: 'driveItem: createLink'
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e65cdc780b5c38441471dd14292f0420bf0ca629
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990725"
---
# <a name="driveitem-createlink"></a><span data-ttu-id="766a2-103">driveItem: createLink</span><span class="sxs-lookup"><span data-stu-id="766a2-103">driveItem: createLink</span></span>

<span data-ttu-id="766a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="766a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="766a2-105">Você pode usar **a ação createLink** para compartilhar um [driveItem](../resources/driveitem.md) por meio de um link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="766a2-105">You can use **createLink** action to share a [driveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="766a2-p101">A ação **createLink** criará um novo link de compartilhamento se o tipo de link especificado não existir para o aplicativo de chamada. Se um link de compartilhamento do tipo especificado já existir para o aplicativo, o link de compartilhamento existente será retornado.</span><span class="sxs-lookup"><span data-stu-id="766a2-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="766a2-108">Recursos de DriveItem herdam permissões de compartilhamento de seus ancestrais.</span><span class="sxs-lookup"><span data-stu-id="766a2-108">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="766a2-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="766a2-109">Permissions</span></span>

<span data-ttu-id="766a2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="766a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="766a2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="766a2-112">Permission type</span></span>      | <span data-ttu-id="766a2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="766a2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="766a2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="766a2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="766a2-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="766a2-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="766a2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="766a2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="766a2-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="766a2-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="766a2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="766a2-118">Application</span></span> | <span data-ttu-id="766a2-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="766a2-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="766a2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="766a2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```
## <a name="request-headers"></a><span data-ttu-id="766a2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="766a2-121">Request headers</span></span>
|<span data-ttu-id="766a2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="766a2-122">Name</span></span>|<span data-ttu-id="766a2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="766a2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="766a2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="766a2-124">Authorization</span></span>|<span data-ttu-id="766a2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="766a2-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="766a2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="766a2-127">Content-Type</span></span>|<span data-ttu-id="766a2-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="766a2-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="766a2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="766a2-130">Request body</span></span>

<span data-ttu-id="766a2-131">O corpo da solicitação define as propriedades do link de compartilhamento que seu aplicativo está solicitando.</span><span class="sxs-lookup"><span data-stu-id="766a2-131">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="766a2-132">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="766a2-132">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="766a2-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="766a2-133">Property</span></span>                 |  <span data-ttu-id="766a2-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="766a2-134">Type</span></span>  |                                 <span data-ttu-id="766a2-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="766a2-135">Description</span></span>                                                               |
| :----------------------| :----- | :---------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="766a2-136">tipo</span><span class="sxs-lookup"><span data-stu-id="766a2-136">type</span></span>|<span data-ttu-id="766a2-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="766a2-137">String</span></span>|<span data-ttu-id="766a2-138">Optional.O tipo de link de compartilhamento a ser criado.</span><span class="sxs-lookup"><span data-stu-id="766a2-138">Optional.The type of sharing link to create.</span></span>   |
|<span data-ttu-id="766a2-139">escopo</span><span class="sxs-lookup"><span data-stu-id="766a2-139">scope</span></span>|<span data-ttu-id="766a2-140">String</span><span class="sxs-lookup"><span data-stu-id="766a2-140">String</span></span>|<span data-ttu-id="766a2-141">Opcional.</span><span class="sxs-lookup"><span data-stu-id="766a2-141">Optional.</span></span> <span data-ttu-id="766a2-142">O escopo do link a ser criado.</span><span class="sxs-lookup"><span data-stu-id="766a2-142">The scope of link to create.</span></span> <span data-ttu-id="766a2-143">Anônimos, organização ou usuários.</span><span class="sxs-lookup"><span data-stu-id="766a2-143">Either anonymous, organization or users.</span></span>|
|<span data-ttu-id="766a2-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="766a2-144">expirationDateTime</span></span>|<span data-ttu-id="766a2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="766a2-145">DateTimeOffset</span></span>|<span data-ttu-id="766a2-146">Opcional.</span><span class="sxs-lookup"><span data-stu-id="766a2-146">Optional.</span></span> <span data-ttu-id="766a2-147">Uma cadeia de caracteres com formato de yyyy-MM-ddTHH:mm:ssZ de DateTime indica o tempo de expiração da permissão.</span><span class="sxs-lookup"><span data-stu-id="766a2-147">A String with format of yyyy-MM-ddTHH:mm:ssZ of DateTime indicates the expiration time of the permission.</span></span>|
|<span data-ttu-id="766a2-148">password</span><span class="sxs-lookup"><span data-stu-id="766a2-148">password</span></span>|<span data-ttu-id="766a2-149">String</span><span class="sxs-lookup"><span data-stu-id="766a2-149">String</span></span>|<span data-ttu-id="766a2-150">Optional.A senha do link de compartilhamento que é definido pelo criador.</span><span class="sxs-lookup"><span data-stu-id="766a2-150">Optional.The password of the sharing link that is set by the creator.</span></span>|
|<span data-ttu-id="766a2-151">destinatários</span><span class="sxs-lookup"><span data-stu-id="766a2-151">recipients</span></span>|<span data-ttu-id="766a2-152">[Coleção driveRecipient](../resources/driverecipient.md)</span><span class="sxs-lookup"><span data-stu-id="766a2-152">[driveRecipient](../resources/driverecipient.md) collection</span></span>|<span data-ttu-id="766a2-153">Opcional.</span><span class="sxs-lookup"><span data-stu-id="766a2-153">Optional.</span></span> <span data-ttu-id="766a2-154">Uma coleção de destinatários que receberão acesso ao link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="766a2-154">A collection of recipients who will receive access to the sharing link.</span></span>|

### <a name="link-types"></a><span data-ttu-id="766a2-155">Tipos de link</span><span class="sxs-lookup"><span data-stu-id="766a2-155">Link types</span></span>

<span data-ttu-id="766a2-156">Os seguintes valores são permitidos para o parâmetro **type**.</span><span class="sxs-lookup"><span data-stu-id="766a2-156">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="766a2-157">Valor do tipo</span><span class="sxs-lookup"><span data-stu-id="766a2-157">Type value</span></span> | <span data-ttu-id="766a2-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="766a2-158">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| <span data-ttu-id="766a2-159">modo de exibição</span><span class="sxs-lookup"><span data-stu-id="766a2-159">view</span></span>           | <span data-ttu-id="766a2-160">Cria um link somente leitura para **o driveItem**.</span><span class="sxs-lookup"><span data-stu-id="766a2-160">Creates a read-only link to the **driveItem**.</span></span>                                                                        |
| <span data-ttu-id="766a2-161">review</span><span class="sxs-lookup"><span data-stu-id="766a2-161">review</span></span>         | <span data-ttu-id="766a2-162">Cria um link de revisão para **o driveItem**.</span><span class="sxs-lookup"><span data-stu-id="766a2-162">Creates a review link to the **driveItem**.</span></span> <span data-ttu-id="766a2-163">Essa opção só está disponível para arquivos em OneDrive for Business e SharePoint.</span><span class="sxs-lookup"><span data-stu-id="766a2-163">This option is only available for files in OneDrive for Business and SharePoint.</span></span>                   |
| <span data-ttu-id="766a2-164">edit</span><span class="sxs-lookup"><span data-stu-id="766a2-164">edit</span></span>           | <span data-ttu-id="766a2-165">Cria um link de leitura-gravação para **o driveItem**.</span><span class="sxs-lookup"><span data-stu-id="766a2-165">Creates an read-write link to the **driveItem**.</span></span>                                                                       |
| <span data-ttu-id="766a2-166">Incorporar</span><span class="sxs-lookup"><span data-stu-id="766a2-166">embed</span></span>          | <span data-ttu-id="766a2-167">Cria um link inbeddable para **o driveItem**.</span><span class="sxs-lookup"><span data-stu-id="766a2-167">Creates an embeddable link to the **driveItem**.</span></span>                                                                      |
| <span data-ttu-id="766a2-168">blocksDownload</span><span class="sxs-lookup"><span data-stu-id="766a2-168">blocksDownload</span></span> | <span data-ttu-id="766a2-169">Cria um link somente leitura que bloqueia o download para **o driveItem**.</span><span class="sxs-lookup"><span data-stu-id="766a2-169">Creates a read-only link that blocks download to the **driveItem**.</span></span> <span data-ttu-id="766a2-170">Essa opção só está disponível para arquivos em OneDrive for Business e SharePoint.</span><span class="sxs-lookup"><span data-stu-id="766a2-170">This option is only available for files in OneDrive for Business and SharePoint.</span></span>  |
| <span data-ttu-id="766a2-171">createOnly</span><span class="sxs-lookup"><span data-stu-id="766a2-171">createOnly</span></span>     | <span data-ttu-id="766a2-172">Cria um link somente para upload para **o driveItem**.</span><span class="sxs-lookup"><span data-stu-id="766a2-172">Creates an upload-only link to the **driveItem**.</span></span> <span data-ttu-id="766a2-173">Essa opção só está disponível para pastas em OneDrive for Business e SharePoint.</span><span class="sxs-lookup"><span data-stu-id="766a2-173">This option is only available for folders in OneDrive for Business and SharePoint.</span></span>             |
| <span data-ttu-id="766a2-174">addressBar</span><span class="sxs-lookup"><span data-stu-id="766a2-174">addressBar</span></span>     | <span data-ttu-id="766a2-175">Cria o link padrão mostrado nas barras de endereço do navegador para arquivos recém-criados.</span><span class="sxs-lookup"><span data-stu-id="766a2-175">Creates the default link that is shown in the browser address bars for newly created files.</span></span> <span data-ttu-id="766a2-176">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="766a2-176">Only available in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="766a2-177">O administrador da organização configura se esse tipo de link tem suporte e quais recursos são suportados por esse tipo de link.</span><span class="sxs-lookup"><span data-stu-id="766a2-177">The organization admin configures whether this link type is supported, and what features are supported by this link type.</span></span> |
| <span data-ttu-id="766a2-178">adminDefault</span><span class="sxs-lookup"><span data-stu-id="766a2-178">adminDefault</span></span>   | <span data-ttu-id="766a2-179">Cria o link padrão para **o driveItem** conforme determinado pelo administrador da organização.</span><span class="sxs-lookup"><span data-stu-id="766a2-179">Creates the default link to the **driveItem** as determined by the administrator of the organization.</span></span> <span data-ttu-id="766a2-180">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="766a2-180">Only available in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="766a2-181">A política é imposta para a organização pelo administrador</span><span class="sxs-lookup"><span data-stu-id="766a2-181">The policy is enforced for the organization by the admin</span></span> |

### <a name="scope-types"></a><span data-ttu-id="766a2-182">Tipos de escopo</span><span class="sxs-lookup"><span data-stu-id="766a2-182">Scope types</span></span>

<span data-ttu-id="766a2-183">Os seguintes valores são permitidos para o parâmetro **scope**.</span><span class="sxs-lookup"><span data-stu-id="766a2-183">The following values are allowed for the **scope** parameter.</span></span>

| <span data-ttu-id="766a2-184">Valor</span><span class="sxs-lookup"><span data-stu-id="766a2-184">Value</span></span>          | <span data-ttu-id="766a2-185">Descrição</span><span class="sxs-lookup"><span data-stu-id="766a2-185">Description</span></span>
|:---------------|:------------------------------------------------------------
| <span data-ttu-id="766a2-186">anonymous</span><span class="sxs-lookup"><span data-stu-id="766a2-186">anonymous</span></span>    | <span data-ttu-id="766a2-187">Qualquer pessoa com o link tem acesso, sem precisar fazer logon.</span><span class="sxs-lookup"><span data-stu-id="766a2-187">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="766a2-188">Isso pode incluir pessoas de fora da organização.</span><span class="sxs-lookup"><span data-stu-id="766a2-188">This may include people outside of your organization.</span></span> <span data-ttu-id="766a2-189">O suporte para links anônimos pode ser desativado por um administrador.</span><span class="sxs-lookup"><span data-stu-id="766a2-189">Anonymous link support may be disabled by an administrator.</span></span>
| <span data-ttu-id="766a2-190">organization</span><span class="sxs-lookup"><span data-stu-id="766a2-190">organization</span></span> | <span data-ttu-id="766a2-191">Qualquer pessoa que tenha feito logon em sua organização (locatário) pode usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="766a2-191">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="766a2-192">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="766a2-192">Only available in OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="766a2-193">usuários</span><span class="sxs-lookup"><span data-stu-id="766a2-193">users</span></span>        | <span data-ttu-id="766a2-194">Pessoas específicas no conjunto de destinatários podem usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="766a2-194">Specific people in the recipients collection can use the link to get access.</span></span> <span data-ttu-id="766a2-195">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="766a2-195">Only available in OneDrive for Business and SharePoint.</span></span>

## <a name="response"></a><span data-ttu-id="766a2-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="766a2-196">Response</span></span>

<span data-ttu-id="766a2-197">Se for bem-sucedido, esse método retornará um único recurso [Permission](../resources/permission.md) no corpo da resposta, que representa as permissões de compartilhamento solicitadas.</span><span class="sxs-lookup"><span data-stu-id="766a2-197">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="766a2-198">A resposta será `201 Created` se um novo link de compartilhamento for criado para o **driveItem** ou `200 OK` se um link existente for retornado.</span><span class="sxs-lookup"><span data-stu-id="766a2-198">The response will be `201 Created` if a new sharing link is created for the **driveItem** or `200 OK` if an existing link is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="766a2-199">Exemplos</span><span class="sxs-lookup"><span data-stu-id="766a2-199">Examples</span></span>

### <a name="example-1-create-an-anonymous-sharing-link"></a><span data-ttu-id="766a2-200">Exemplo 1: Criar um link de compartilhamento anônimo</span><span class="sxs-lookup"><span data-stu-id="766a2-200">Example 1: Create an anonymous sharing link</span></span>
<span data-ttu-id="766a2-201">O exemplo a seguir solicita que um link de compartilhamento seja criado para **o driveItem** especificado por {itemId} no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="766a2-201">The following example requests a sharing link to be created for the **driveItem** specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="766a2-202">O link de compartilhamento é configurado como somente leitura e utilizável por qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="766a2-202">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

#### <a name="request"></a><span data-ttu-id="766a2-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="766a2-203">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "driveItem_createlink",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-Type: application/json
Content-length: 212

{
  "type": "view",
  "scope": "anonymous",
  "password": "String",
  "recipients": [
    {
      "@odata.type": "microsoft.graph.driveRecipient"
    }
  ]
}
```

# <a name="c"></a>[<span data-ttu-id="766a2-204">C#</span><span class="sxs-lookup"><span data-stu-id="766a2-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/driveitem-createlink-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="766a2-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="766a2-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/driveitem-createlink-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="766a2-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="766a2-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/driveitem-createlink-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="766a2-207">Java</span><span class="sxs-lookup"><span data-stu-id="766a2-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/driveitem-createlink-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="766a2-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="766a2-208">Response</span></span>
><span data-ttu-id="766a2-209">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="766a2-209">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->

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

### <a name="example-2-creating-company-sharable-links"></a><span data-ttu-id="766a2-210">Exemplo 2: Criação de links compartilháveis da empresa</span><span class="sxs-lookup"><span data-stu-id="766a2-210">Example 2: Creating company sharable links</span></span>

<span data-ttu-id="766a2-211">O OneDrive for Business e o SharePoint oferecem suporte a links compartilháveis pela empresa.</span><span class="sxs-lookup"><span data-stu-id="766a2-211">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="766a2-212">Estes são semelhantes a links anônimos, com a diferença de que apenas funcionam para membros da organização proprietária.</span><span class="sxs-lookup"><span data-stu-id="766a2-212">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="766a2-213">Para criar um link compartilhável pela empresa, use o parâmetro **scope** com um valor de `organization`.</span><span class="sxs-lookup"><span data-stu-id="766a2-213">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

#### <a name="request"></a><span data-ttu-id="766a2-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="766a2-214">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create-link-scoped",
  "scopes": "files.readwrite service.sharepoint",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
 } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```
# <a name="c"></a>[<span data-ttu-id="766a2-215">C#</span><span class="sxs-lookup"><span data-stu-id="766a2-215">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-scoped-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="766a2-216">JavaScript</span><span class="sxs-lookup"><span data-stu-id="766a2-216">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-scoped-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="766a2-217">Objective-C</span><span class="sxs-lookup"><span data-stu-id="766a2-217">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-scoped-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="766a2-218">Java</span><span class="sxs-lookup"><span data-stu-id="766a2-218">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-link-scoped-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="766a2-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="766a2-219">Response</span></span>

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

### <a name="example-3-creating-embeddable-links"></a><span data-ttu-id="766a2-220">Exemplo 3: Criação de links inbeddáveis</span><span class="sxs-lookup"><span data-stu-id="766a2-220">Example 3: Creating embeddable links</span></span>

<span data-ttu-id="766a2-p119">Ao usar o tipo de link `embed`, a webUrl retornada pode ser inserida em um elemento HTML `<iframe>`. Quando um link de inserção é criado, a propriedade `webHtml` contém o código HTML de um `<iframe>` para hospedar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="766a2-p119">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

><span data-ttu-id="766a2-223">**Observação:** os links de inseridos só tem suporte no OneDrive Pessoal.</span><span class="sxs-lookup"><span data-stu-id="766a2-223">**Note:** Embed links are only supported for OneDrive personal.</span></span>

#### <a name="request"></a><span data-ttu-id="766a2-224">Solicitar</span><span class="sxs-lookup"><span data-stu-id="766a2-224">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create-embedded-link",
  "scopes": "files.readwrite service.onedrive",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
} -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```
# <a name="c"></a>[<span data-ttu-id="766a2-225">C#</span><span class="sxs-lookup"><span data-stu-id="766a2-225">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-embedded-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="766a2-226">JavaScript</span><span class="sxs-lookup"><span data-stu-id="766a2-226">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-embedded-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="766a2-227">Objective-C</span><span class="sxs-lookup"><span data-stu-id="766a2-227">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-embedded-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="766a2-228">Java</span><span class="sxs-lookup"><span data-stu-id="766a2-228">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-embedded-link-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="766a2-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="766a2-229">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="766a2-230">Comentários</span><span class="sxs-lookup"><span data-stu-id="766a2-230">Remarks</span></span>

* <span data-ttu-id="766a2-231">Para criar um link com base na política padrão da organização e nas permissões do chamador no **driveItem,** omita os parâmetros de escopo e de tipo</span><span class="sxs-lookup"><span data-stu-id="766a2-231">To create a link based on the organization's default policy and the caller's permissions on the **driveItem**, omit the scope and type parameters</span></span>
* <span data-ttu-id="766a2-232">Links criados usando esta ação não expiram, a menos que uma política de expiração padrão seja imposta à organização.</span><span class="sxs-lookup"><span data-stu-id="766a2-232">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="766a2-233">Os links ficam visíveis nas permissões de compartilhamento do **driveItem** e podem ser removidos por um proprietário do **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="766a2-233">Links are visible in the sharing permissions for the **driveItem** and can be removed by an owner of the **driveItem**.</span></span>
* <span data-ttu-id="766a2-234">Os links sempre apontam para a versão atual de **um driveItem,** a menos que **o driveItem** esteja com check-out (SharePoint somente).</span><span class="sxs-lookup"><span data-stu-id="766a2-234">Links always point to the current version of a **driveItem** unless the **driveItem** is checked out (SharePoint only).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for a driveItem.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
}
-->
