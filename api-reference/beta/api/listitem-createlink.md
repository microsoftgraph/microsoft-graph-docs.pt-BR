---
title: 'listItem: createLink'
description: Criar um link para compartilhar um listItem
author: learafa
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b0d490139763e619a151e3152868f98c1f1b96e4
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941575"
---
# <a name="listitem-createlink"></a><span data-ttu-id="8ed2c-103">listItem: createLink</span><span class="sxs-lookup"><span data-stu-id="8ed2c-103">listItem: createLink</span></span>

<span data-ttu-id="8ed2c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ed2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ed2c-105">Criar um link de compartilhamento para [um listItem](../resources/listitem.md).</span><span class="sxs-lookup"><span data-stu-id="8ed2c-105">Create a sharing link for a [listItem](../resources/listitem.md).</span></span>

<span data-ttu-id="8ed2c-106">A **ação createLink** criará um novo link de compartilhamento se o tipo de link especificado ainda não existir para o aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-106">The **createLink** action creates a new sharing link if the specified link type doesn't already exist for the calling application.</span></span>
<span data-ttu-id="8ed2c-107">Se um link de compartilhamento do tipo especificado já existir para o aplicativo, essa ação retornará o link de compartilhamento existente.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-107">If a sharing link of the specified type already exists for the app, this action will return the existing sharing link.</span></span>

<span data-ttu-id="8ed2c-108">**os recursos listItem** herdam permissões de compartilhamento da [lista](../resources/list.md) em que o item reside.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-108">**listItem** resources inherit sharing permissions from the [list](../resources/list.md) the item resides in.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ed2c-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ed2c-109">Permissions</span></span>
<span data-ttu-id="8ed2c-110">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8ed2c-111">Para saber mais, incluindo como escolher permissões, consulte [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ed2c-111">To learn more, including how to choose permissions, see [permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ed2c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ed2c-112">Permission type</span></span>|<span data-ttu-id="8ed2c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ed2c-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ed2c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ed2c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8ed2c-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ed2c-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8ed2c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ed2c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ed2c-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ed2c-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8ed2c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ed2c-118">Application</span></span> | <span data-ttu-id="8ed2c-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ed2c-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ed2c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ed2c-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}
-->
``` http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
```

## <a name="request-headers"></a><span data-ttu-id="8ed2c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed2c-121">Request headers</span></span>
|<span data-ttu-id="8ed2c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8ed2c-122">Name</span></span>|<span data-ttu-id="8ed2c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ed2c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8ed2c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ed2c-124">Authorization</span></span>|<span data-ttu-id="8ed2c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8ed2c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ed2c-127">Content-Type</span></span>|<span data-ttu-id="8ed2c-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ed2c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed2c-130">Request body</span></span>
<span data-ttu-id="8ed2c-131">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-131">In the request body, provide a JSON representation of the parameters.</span></span>

<span data-ttu-id="8ed2c-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-132">The following table shows the parameters that can be used with this action.</span></span>

|   <span data-ttu-id="8ed2c-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ed2c-133">Property</span></span>             |  <span data-ttu-id="8ed2c-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ed2c-134">Type</span></span>  |           <span data-ttu-id="8ed2c-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ed2c-135">Description</span></span>                        |
| :----------------------| :----- | :--------------------------------------------|
|<span data-ttu-id="8ed2c-136">tipo</span><span class="sxs-lookup"><span data-stu-id="8ed2c-136">type</span></span>|<span data-ttu-id="8ed2c-137">String</span><span class="sxs-lookup"><span data-stu-id="8ed2c-137">String</span></span>|<span data-ttu-id="8ed2c-138">O tipo de link de compartilhamento a ser criado.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-138">The type of sharing link to create.</span></span> <span data-ttu-id="8ed2c-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-139">Optional.</span></span> |
|<span data-ttu-id="8ed2c-140">escopo</span><span class="sxs-lookup"><span data-stu-id="8ed2c-140">scope</span></span>|<span data-ttu-id="8ed2c-141">String</span><span class="sxs-lookup"><span data-stu-id="8ed2c-141">String</span></span>|<span data-ttu-id="8ed2c-142">O escopo do link a ser criado.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-142">The scope of link to create.</span></span> <span data-ttu-id="8ed2c-143">Ou `anonymous` `organization` `users` .</span><span class="sxs-lookup"><span data-stu-id="8ed2c-143">Either `anonymous`, `organization` or `users`.</span></span> <span data-ttu-id="8ed2c-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-144">Optional.</span></span> |
|<span data-ttu-id="8ed2c-145">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8ed2c-145">expirationDateTime</span></span>|<span data-ttu-id="8ed2c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ed2c-146">DateTimeOffset</span></span>|<span data-ttu-id="8ed2c-147">Uma cadeia de caracteres com formato de yyyy-MM-ddTHH:mm:ssZ de DateTime indica o tempo de expiração da permissão.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-147">A string with format of yyyy-MM-ddTHH:mm:ssZ of DateTime indicates the expiration time of the permission.</span></span> <span data-ttu-id="8ed2c-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-148">Optional.</span></span> |
|<span data-ttu-id="8ed2c-149">password</span><span class="sxs-lookup"><span data-stu-id="8ed2c-149">password</span></span>|<span data-ttu-id="8ed2c-150">String</span><span class="sxs-lookup"><span data-stu-id="8ed2c-150">String</span></span>|<span data-ttu-id="8ed2c-151">A senha do link de compartilhamento definido pelo criador.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-151">The password of the sharing link that is set by the creator.</span></span> <span data-ttu-id="8ed2c-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-152">Optional.</span></span> |
|<span data-ttu-id="8ed2c-153">destinatários</span><span class="sxs-lookup"><span data-stu-id="8ed2c-153">recipients</span></span>|<span data-ttu-id="8ed2c-154">[Coleção driveRecipient](../resources/driverecipient.md)</span><span class="sxs-lookup"><span data-stu-id="8ed2c-154">[driveRecipient](../resources/driverecipient.md) collection</span></span>|<span data-ttu-id="8ed2c-155">Uma coleção de destinatários que receberão acesso ao link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-155">A collection of recipients who will receive access to the sharing link.</span></span> <span data-ttu-id="8ed2c-156">Opcional.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-156">Optional.</span></span> |

### <a name="link-types"></a><span data-ttu-id="8ed2c-157">Tipos de link</span><span class="sxs-lookup"><span data-stu-id="8ed2c-157">Link types</span></span>

<span data-ttu-id="8ed2c-158">Os seguintes valores são permitidos para o parâmetro **type**.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-158">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="8ed2c-159">Valor do tipo</span><span class="sxs-lookup"><span data-stu-id="8ed2c-159">Type value</span></span> | <span data-ttu-id="8ed2c-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ed2c-160">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| <span data-ttu-id="8ed2c-161">modo de exibição</span><span class="sxs-lookup"><span data-stu-id="8ed2c-161">view</span></span>           | <span data-ttu-id="8ed2c-162">Cria um link somente leitura para o item.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-162">Creates a read-only link to the item.</span></span>                                                                        |
| <span data-ttu-id="8ed2c-163">review</span><span class="sxs-lookup"><span data-stu-id="8ed2c-163">review</span></span>         | <span data-ttu-id="8ed2c-164">Cria um link de revisão para o item.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-164">Creates a review link to the item.</span></span> <span data-ttu-id="8ed2c-165">Essa opção só está disponível para arquivos em OneDrive for Business e SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-165">This option is only available for files in OneDrive for Business and SharePoint.</span></span>                   |
| <span data-ttu-id="8ed2c-166">edit</span><span class="sxs-lookup"><span data-stu-id="8ed2c-166">edit</span></span>           | <span data-ttu-id="8ed2c-167">Cria um link de leitura-gravação para o item.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-167">Creates an read-write link to the item.</span></span>                                                                       |
| <span data-ttu-id="8ed2c-168">Incorporar</span><span class="sxs-lookup"><span data-stu-id="8ed2c-168">embed</span></span>          | <span data-ttu-id="8ed2c-169">Cria um link inserível para o item.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-169">Creates an embeddable link to the item.</span></span>                                                                      |
| <span data-ttu-id="8ed2c-170">blocksDownload</span><span class="sxs-lookup"><span data-stu-id="8ed2c-170">blocksDownload</span></span> | <span data-ttu-id="8ed2c-171">Cria um link somente leitura que bloqueia o download para o item.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-171">Creates a read-only link that blocks download to the item.</span></span> <span data-ttu-id="8ed2c-172">Essa opção só está disponível para arquivos em OneDrive for Business e SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-172">This option is only available for files in OneDrive for Business and SharePoint.</span></span>  |
| <span data-ttu-id="8ed2c-173">createOnly</span><span class="sxs-lookup"><span data-stu-id="8ed2c-173">createOnly</span></span>     | <span data-ttu-id="8ed2c-174">Cria um link somente carregamento para o item.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-174">Creates an upload-only link to the item.</span></span> <span data-ttu-id="8ed2c-175">Essa opção só está disponível para pastas em OneDrive for Business e SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-175">This option is only available for folders in OneDrive for Business and SharePoint.</span></span>             |
| <span data-ttu-id="8ed2c-176">addressBar</span><span class="sxs-lookup"><span data-stu-id="8ed2c-176">addressBar</span></span>     | <span data-ttu-id="8ed2c-177">Cria o link padrão mostrado nas barras de endereço do navegador para arquivos recém-criados.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-177">Creates the default link that is shown in the browser address bars for newly created files.</span></span> <span data-ttu-id="8ed2c-178">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-178">Only available in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="8ed2c-179">O administrador da organização configura se esse tipo de link tem suporte e quais recursos são suportados por esse tipo de link.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-179">The organization admin configures whether this link type is supported, and what features are supported by this link type.</span></span> |
| <span data-ttu-id="8ed2c-180">adminDefault</span><span class="sxs-lookup"><span data-stu-id="8ed2c-180">adminDefault</span></span>   | <span data-ttu-id="8ed2c-181">Cria o link padrão para o item conforme determinado pelo administrador da organização.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-181">Creates the default link to the item as determined by the administrator of the organization.</span></span> <span data-ttu-id="8ed2c-182">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-182">Only available in OneDrive for Business and SharePoint.</span></span> <span data-ttu-id="8ed2c-183">A política é imposta para a organização pelo administrador</span><span class="sxs-lookup"><span data-stu-id="8ed2c-183">The policy is enforced for the organization by the admin</span></span> |

### <a name="scope-types"></a><span data-ttu-id="8ed2c-184">Tipos de escopo</span><span class="sxs-lookup"><span data-stu-id="8ed2c-184">Scope types</span></span>

<span data-ttu-id="8ed2c-185">Os seguintes valores são permitidos para o parâmetro **scope**.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-185">The following values are allowed for the **scope** parameter.</span></span>

| <span data-ttu-id="8ed2c-186">Valor</span><span class="sxs-lookup"><span data-stu-id="8ed2c-186">Value</span></span>          | <span data-ttu-id="8ed2c-187">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ed2c-187">Description</span></span>
|:---------------|:------------------------------------------------------------
| <span data-ttu-id="8ed2c-188">anonymous</span><span class="sxs-lookup"><span data-stu-id="8ed2c-188">anonymous</span></span>    | <span data-ttu-id="8ed2c-189">Qualquer pessoa com o link tem acesso, sem precisar fazer logon.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-189">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="8ed2c-190">Isso pode incluir pessoas de fora da organização.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-190">This may include people outside of your organization.</span></span> <span data-ttu-id="8ed2c-191">O suporte para links anônimos pode ser desativado por um administrador.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-191">Anonymous link support may be disabled by an administrator.</span></span>
| <span data-ttu-id="8ed2c-192">organization</span><span class="sxs-lookup"><span data-stu-id="8ed2c-192">organization</span></span> | <span data-ttu-id="8ed2c-193">Qualquer pessoa que tenha feito logon em sua organização (locatário) pode usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-193">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="8ed2c-194">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-194">Only available in OneDrive for Business and SharePoint.</span></span>
| <span data-ttu-id="8ed2c-195">usuários</span><span class="sxs-lookup"><span data-stu-id="8ed2c-195">users</span></span>        | <span data-ttu-id="8ed2c-196">Pessoas específicas no conjunto de destinatários podem usar o link para obter acesso.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-196">Specific people in the recipients collection can use the link to get access.</span></span> <span data-ttu-id="8ed2c-197">Disponível apenas no OneDrive for Business e no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-197">Only available in OneDrive for Business and SharePoint.</span></span>

## <a name="response"></a><span data-ttu-id="8ed2c-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed2c-198">Response</span></span>

<span data-ttu-id="8ed2c-199">Se tiver êxito, este método retornará um [único](../resources/permission.md) recurso de permissão no corpo da resposta que representa as permissões de compartilhamento solicitadas.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-199">If successful, this method returns a single [permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="8ed2c-200">A resposta será `201 Created` se um novo link de compartilhamento for criado para o listItem ou se um link existente for `200 OK` retornado.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-200">The response will be `201 Created` if a new sharing link is created for the listItem or `200 OK` if an existing link is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="8ed2c-201">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8ed2c-201">Examples</span></span>

### <a name="example-1-create-an-anonymous-sharing-link"></a><span data-ttu-id="8ed2c-202">Exemplo 1: Criar um link de compartilhamento anônimo</span><span class="sxs-lookup"><span data-stu-id="8ed2c-202">Example 1: Create an anonymous sharing link</span></span>
<span data-ttu-id="8ed2c-203">O exemplo a seguir solicita que um link de compartilhamento seja criado para o listItem especificado por {itemId} na lista especificada {listId}.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-203">The following example requests a sharing link to be created for the listItem specified by {itemId} in the list specified {listId}.</span></span>
<span data-ttu-id="8ed2c-204">O link de compartilhamento é configurado como somente leitura e utilizável por qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-204">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

#### <a name="request"></a><span data-ttu-id="8ed2c-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed2c-205">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST sites/{siteId}/lists/{listId}/items/{itemId}/createLink
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

#### <a name="response"></a><span data-ttu-id="8ed2c-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed2c-206">Response</span></span>
><span data-ttu-id="8ed2c-207">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-207">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
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

### <a name="example-2-creating-company-sharable-links"></a><span data-ttu-id="8ed2c-208">Exemplo 2: Criação de links compartilháveis da empresa</span><span class="sxs-lookup"><span data-stu-id="8ed2c-208">Example 2: Creating company sharable links</span></span>

<span data-ttu-id="8ed2c-209">O OneDrive for Business e o SharePoint oferecem suporte a links compartilháveis pela empresa.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-209">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="8ed2c-210">Estes são semelhantes a links anônimos, com a diferença de que apenas funcionam para membros da organização proprietária.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-210">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="8ed2c-211">Para criar um link compartilhável pela empresa, use o parâmetro **scope** com um valor de `organization`.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-211">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

#### <a name="request"></a><span data-ttu-id="8ed2c-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed2c-212">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

#### <a name="response"></a><span data-ttu-id="8ed2c-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed2c-213">Response</span></span>

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

### <a name="example-3-creating-embeddable-links"></a><span data-ttu-id="8ed2c-214">Exemplo 3: Criação de links inbeddáveis</span><span class="sxs-lookup"><span data-stu-id="8ed2c-214">Example 3: Creating embeddable links</span></span>

<span data-ttu-id="8ed2c-p120">Ao usar o tipo de link `embed`, a webUrl retornada pode ser inserida em um elemento HTML `<iframe>`. Quando um link de inserção é criado, a propriedade `webHtml` contém o código HTML de um `<iframe>` para hospedar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-p120">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

><span data-ttu-id="8ed2c-217">**Observação:** os links de inseridos só tem suporte no OneDrive Pessoal.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-217">**Note:** Embed links are only supported for OneDrive personal.</span></span>

#### <a name="request"></a><span data-ttu-id="8ed2c-218">Solicitar</span><span class="sxs-lookup"><span data-stu-id="8ed2c-218">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

#### <a name="response"></a><span data-ttu-id="8ed2c-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed2c-219">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="8ed2c-220">Comentários</span><span class="sxs-lookup"><span data-stu-id="8ed2c-220">Remarks</span></span>

* <span data-ttu-id="8ed2c-221">Para criar um link com base na política padrão da organização e nas permissões do chamador no listItem, omita os parâmetros de escopo e de tipo</span><span class="sxs-lookup"><span data-stu-id="8ed2c-221">To create a link based on the organization's default policy and the caller's permissions on the listItem, omit the scope and type parameters</span></span>
* <span data-ttu-id="8ed2c-222">Links criados usando esta ação não expiram, a menos que uma política de expiração padrão seja imposta à organização.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-222">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="8ed2c-223">Os links ficam visíveis nas permissões de compartilhamento do listItem e podem ser removidos por um proprietário do listItem.</span><span class="sxs-lookup"><span data-stu-id="8ed2c-223">Links are visible in the sharing permissions for the listItem and can be removed by an owner of the listItem.</span></span>
* <span data-ttu-id="8ed2c-224">Os links sempre apontam para a versão atual de um listItem, a menos que listItem esteja com check-out (SharePoint somente).</span><span class="sxs-lookup"><span data-stu-id="8ed2c-224">Links always point to the current version of a listItem unless the listItem is checked out (SharePoint only).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an listItem.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
}
-->