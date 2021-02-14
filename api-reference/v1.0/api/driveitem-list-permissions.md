---
author: JeremyKelley
ms.date: 09/10/2017
title: Listar quem tem acesso a um arquivo
localization_priority: Normal
ms.prod: sharepoint
description: Listar as permissões efetivas de compartilhamento de um driveItem.
doc_type: apiPageType
ms.openlocfilehash: a89dc20289ee86933d4eee0c217f769b9fbd426e
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240273"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a><span data-ttu-id="0b826-103">Listar permissões de compartilhamento em um driveItem</span><span class="sxs-lookup"><span data-stu-id="0b826-103">List sharing permissions on a driveItem</span></span>

<span data-ttu-id="0b826-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b826-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b826-105">Listar as permissões efetivas de compartilhamento em [um driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0b826-105">List the effective sharing permissions on a [driveItem](../resources/driveitem.md).</span></span>

## <a name="access-to-sharing-permissions"></a><span data-ttu-id="0b826-106">Acessar permissões de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="0b826-106">Access to sharing permissions</span></span>

<span data-ttu-id="0b826-107">A coleção de permissões inclui informações potencialmente confidenciais e pode não estar disponível para todos os chamadores.</span><span class="sxs-lookup"><span data-stu-id="0b826-107">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="0b826-108">Para o proprietário do item, todas as permissões de compartilhamento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="0b826-108">For the owner of the item, all sharing permissions will be returned.</span></span> <span data-ttu-id="0b826-109">Isto inclui os coproprietários.</span><span class="sxs-lookup"><span data-stu-id="0b826-109">This includes co-owners.</span></span>
* <span data-ttu-id="0b826-110">Para um chamador não proprietário, somente as permissões de compartilhamento que se aplicam ao chamador são retornadas.</span><span class="sxs-lookup"><span data-stu-id="0b826-110">For a non-owner caller, only the sharing permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="0b826-111">Propriedades de permissão de compartilhamento que contêm segredos (por exemplo, `shareId` e `webUrl`) são retornadas somente para chamadores que são capazes de criar a permissão de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="0b826-111">Sharing permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the sharing permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b826-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b826-112">Permissions</span></span>

<span data-ttu-id="0b826-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b826-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b826-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b826-115">Permission type</span></span>      | <span data-ttu-id="0b826-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b826-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b826-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b826-117">Delegated (work or school account)</span></span> | <span data-ttu-id="0b826-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b826-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0b826-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b826-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b826-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b826-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0b826-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b826-121">Application</span></span> | <span data-ttu-id="0b826-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b826-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b826-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b826-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b826-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0b826-124">Optional query parameters</span></span>

<span data-ttu-id="0b826-125">Este método oferece suporte aos [Parâmetros de consulta OData](/graph/query-parameters) `$select` para personalizar as resposta.</span><span class="sxs-lookup"><span data-stu-id="0b826-125">This method supports the `$select` [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="0b826-126">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="0b826-126">Optional request headers</span></span>

| <span data-ttu-id="0b826-127">Nome</span><span class="sxs-lookup"><span data-stu-id="0b826-127">Name</span></span>          | <span data-ttu-id="0b826-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b826-128">Type</span></span>   | <span data-ttu-id="0b826-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b826-129">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0b826-130">if-none-match</span><span class="sxs-lookup"><span data-stu-id="0b826-130">if-none-match</span></span> | <span data-ttu-id="0b826-131">string</span><span class="sxs-lookup"><span data-stu-id="0b826-131">string</span></span> | <span data-ttu-id="0b826-132">Se este cabeçalho de solicitação estiver incluso e a etag fornecida corresponder à marca atual do item, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="0b826-132">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="0b826-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b826-133">Response</span></span>

<span data-ttu-id="0b826-134">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de recursos [Permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b826-134">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="0b826-135">As permissões efetivas de compartilhamento de um DriveItem podem vir de duas fontes:</span><span class="sxs-lookup"><span data-stu-id="0b826-135">Effective sharing permissions of a DriveItem can come from two sources:</span></span>

* <span data-ttu-id="0b826-136">Permissões de compartilhamento aplicadas diretamente ao próprio DriveItem</span><span class="sxs-lookup"><span data-stu-id="0b826-136">Sharing permissions applied directly on the DriveItem itself</span></span>
* <span data-ttu-id="0b826-137">Permissões de compartilhamento herdadas de ancestrais do DriveItem</span><span class="sxs-lookup"><span data-stu-id="0b826-137">Sharing permissions inherited from the DriveItem's ancestors</span></span>

<span data-ttu-id="0b826-p103">Os chamadores podem diferenciar se a permissão é herdada ou não verificando a propriedade **inheritedFrom**. Esta propriedade é um recurso [**itemReference**](../resources/itemreference.md) que referencia o ancestral do qual a permissão é herdada.</span><span class="sxs-lookup"><span data-stu-id="0b826-p103">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="0b826-p104">Níveis de permissão do SharePoint definidos em um item retornam com um prefixo 'SP'. Por exemplo, SP.Somente exibição, SP.Acesso limitado, SP.Exibir Dados do Web Analytics. Confira a [Lista completa de funções do SharePoint](/SharePoint/sites/user-permissions-and-permission-levels#section1).</span><span class="sxs-lookup"><span data-stu-id="0b826-p104">SharePoint permission levels set on an item are returned with an 'SP' prefix. For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data. See [Full list of SharePoint roles](/SharePoint/sites/user-permissions-and-permission-levels#section1).</span></span>

## <a name="example"></a><span data-ttu-id="0b826-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b826-143">Example</span></span>

<span data-ttu-id="0b826-144">Este exemplo recupera a coleção de permissões em um item na unidade do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="0b826-144">This example retrieves the collection of permissions on an item in the signed in user's drive.</span></span>

# <a name="http"></a>[<span data-ttu-id="0b826-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b826-145">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/permissions
```
# <a name="c"></a>[<span data-ttu-id="0b826-146">C#</span><span class="sxs-lookup"><span data-stu-id="0b826-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-permissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b826-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b826-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-permissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b826-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b826-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-permissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b826-149">Java</span><span class="sxs-lookup"><span data-stu-id="0b826-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-permissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0b826-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b826-150">Response</span></span>

<span data-ttu-id="0b826-151">Esta resposta de exemplo inclui três permissões, a primeira é um link de compartilhamento com permissões de edição, a segunda é uma permissão explícita para um usuário chamado John, que foi herdada da pasta pai, e a terceira é um link de compartilhamento de leitura e gravação criado por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0b826-151">This example response includes three permissions, the first is a sharing link with edit permissions, the second is an explicit permission for a user named John, which was inherited from a parent folder, and the third is a read-write sharing link created by an application.</span></span>

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "Contoso Time Manager"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="0b826-152">Comentários</span><span class="sxs-lookup"><span data-stu-id="0b826-152">Remarks</span></span>

<span data-ttu-id="0b826-p105">A relação **permissions** de um DriveItem não pode ser expandida como parte de uma chamada para [get DriveItem](driveitem-get.md) ou uma coleção de DriveItems. Você deve acessar a propriedade permissions diretamente.</span><span class="sxs-lookup"><span data-stu-id="0b826-p105">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](driveitem-get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="error-responses"></a><span data-ttu-id="0b826-155">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="0b826-155">Error responses</span></span>

<span data-ttu-id="0b826-156">Veja mais informações sobre como os erros são retornados no tópico [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="0b826-156">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions",
  "suppressions": [
  ]
} -->
