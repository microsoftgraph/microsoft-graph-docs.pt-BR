---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Listar quem tem acesso a um arquivo
ms.openlocfilehash: 8b8671fbad37601a42127119f8bef6e5eca23dea
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="list-sharing-permissions-on-a-driveitem"></a><span data-ttu-id="d13ce-102">Listar permissões de compartilhamento em um DriveItem</span><span class="sxs-lookup"><span data-stu-id="d13ce-102">List permissions on a DriveItem</span></span>

<span data-ttu-id="d13ce-103">Liste as permissões efetivas de compartilhamento de um [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d13ce-103">List the effective permissions of on a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="access-to-sharing-permissions"></a><span data-ttu-id="d13ce-104">Acessar permissões de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="d13ce-104">Access to sharing permissions</span></span>

<span data-ttu-id="d13ce-105">A coleção de permissões inclui informações potencialmente confidenciais e pode não estar disponível para todos os chamadores.</span><span class="sxs-lookup"><span data-stu-id="d13ce-105">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="d13ce-106">Para o proprietário do item, todas as permissões de compartilhamento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="d13ce-106">For the owner of the item, all permissions will be returned. This includes co-owners.</span></span> <span data-ttu-id="d13ce-107">Isto inclui os coproprietários.</span><span class="sxs-lookup"><span data-stu-id="d13ce-107">This includes co-owners.</span></span>
* <span data-ttu-id="d13ce-108">Para um chamador não proprietário, somente as permissões de compartilhamento que se aplicam ao chamador são retornadas.</span><span class="sxs-lookup"><span data-stu-id="d13ce-108">For a non-owner caller, only the permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="d13ce-109">Propriedades de permissão de compartilhamento que contêm segredos (por exemplo, `shareId` e `webUrl`) são retornadas somente para chamadores que são capazes de criar a permissão de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="d13ce-109">Permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the Permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="d13ce-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="d13ce-110">Permissions</span></span>

<span data-ttu-id="d13ce-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d13ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d13ce-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d13ce-113">Permission type</span></span>      | <span data-ttu-id="d13ce-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d13ce-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d13ce-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d13ce-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d13ce-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d13ce-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d13ce-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d13ce-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d13ce-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d13ce-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d13ce-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d13ce-119">Application</span></span> | <span data-ttu-id="d13ce-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d13ce-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d13ce-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d13ce-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d13ce-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d13ce-122">Optional query parameters</span></span>

<span data-ttu-id="d13ce-123">Este método dá suporte aos `$select` [Parâmetros de consulta OData](../../../concepts/query_parameters.md) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d13ce-123">This method supports , , and `$select` [OData Query Parameters](../../../concepts/query_parameters.md) to customize the response.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="d13ce-124">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="d13ce-124">Optional request headers</span></span>

| <span data-ttu-id="d13ce-125">Name</span><span class="sxs-lookup"><span data-stu-id="d13ce-125">Name</span></span>          | <span data-ttu-id="d13ce-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d13ce-126">Type</span></span>   | <span data-ttu-id="d13ce-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d13ce-127">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d13ce-128">if-none-match</span><span class="sxs-lookup"><span data-stu-id="d13ce-128">if-none-match</span></span> | <span data-ttu-id="d13ce-129">string</span><span class="sxs-lookup"><span data-stu-id="d13ce-129">string</span></span> | <span data-ttu-id="d13ce-130">Se este cabeçalho de solicitação estiver incluso e a etag fornecida corresponder à marca atual do item, uma resposta `HTTP 304 Not Modified` será exibida.</span><span class="sxs-lookup"><span data-stu-id="d13ce-130">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="d13ce-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d13ce-131">Response</span></span>

<span data-ttu-id="d13ce-132">Se for bem-sucedido, esse método retornará um código de resposta `200 OK` e uma coleção de recursos [Permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d13ce-132">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="d13ce-133">As permissões efetivas de compartilhamento de um DriveItem podem vir de duas fontes:</span><span class="sxs-lookup"><span data-stu-id="d13ce-133">Effective permissions of an item can come from two sources:</span></span>

* <span data-ttu-id="d13ce-134">Permissões de compartilhamento aplicadas diretamente ao próprio DriveItem</span><span class="sxs-lookup"><span data-stu-id="d13ce-134">Sharing permissions applied directly on the DriveItem itself</span></span>
* <span data-ttu-id="d13ce-135">Permissões de compartilhamento herdadas de ancestrais do DriveItem</span><span class="sxs-lookup"><span data-stu-id="d13ce-135">Sharing permissions inherited from the DriveItem's ancestors</span></span>

<span data-ttu-id="d13ce-p103">Os chamadores podem diferenciar se a permissão é herdada ou não verificando a propriedade **inheritedFrom**. Esta propriedade é um recurso [**itemReference**](../resources/itemreference.md) que referencia o ancestral do qual a permissão é herdada.</span><span class="sxs-lookup"><span data-stu-id="d13ce-p103">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="d13ce-138">Os níveis de permissão do SharePoint definidos em um item retornam com um prefixo 'SP'.</span><span class="sxs-lookup"><span data-stu-id="d13ce-138">SharePoint permission levels set on an item are returned with an 'SP' prefix.</span></span> <span data-ttu-id="d13ce-139">Por exemplo, SP.Somente exibição, SP.Acesso limitado, SP.Exibir Dados do Web Analytics.</span><span class="sxs-lookup"><span data-stu-id="d13ce-139">For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data.</span></span> <span data-ttu-id="d13ce-140">Confira a [Lista completa de funções do SharePoint](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span><span class="sxs-lookup"><span data-stu-id="d13ce-140">See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="example"></a><span data-ttu-id="d13ce-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d13ce-141">Example</span></span>

<span data-ttu-id="d13ce-142">Este exemplo recupera a coleção de permissões em um item na unidade do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d13ce-142">This example retrieves the collection of permissions on an item in the signed in user's drive.</span></span>

<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/permissions
```

### <a name="response"></a><span data-ttu-id="d13ce-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d13ce-143">Response</span></span>

<span data-ttu-id="d13ce-144">Esta resposta de exemplo inclui três permissões, a primeira é um link de compartilhamento com permissões de edição, a segunda é uma permissão explícita para um usuário chamado John, que foi herdada da pasta pai, e a terceira é um link de compartilhamento de leitura e gravação criado por um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d13ce-144">This example response includes three permissions, the first is a sharing link with edit permissions, the second is an explicit permission for a user named John, which was inherited from a parent folder, and the third is a read-write sharing link created by an application.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="d13ce-145">Comentários</span><span class="sxs-lookup"><span data-stu-id="d13ce-145">Remarks</span></span>

<span data-ttu-id="d13ce-p105">A relação **permissions** de um DriveItem não pode ser expandida como parte de uma chamada para [get DriveItem](driveitem_get.md) ou uma coleção de DriveItems. Você deve acessar a propriedade permissions diretamente.</span><span class="sxs-lookup"><span data-stu-id="d13ce-p105">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](driveitem_get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="error-responses"></a><span data-ttu-id="d13ce-148">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="d13ce-148">Error responses</span></span>

<span data-ttu-id="d13ce-149">Veja mais informações sobre como os erros são retornados no tópico [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="d13ce-149">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions"
} -->
