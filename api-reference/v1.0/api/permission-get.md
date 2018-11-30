---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Obter permissões
ms.openlocfilehash: f2b727878478b7a3e996448e1f6285ea74f7d9a3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004104"
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a><span data-ttu-id="923af-102">Obter permissão de compartilhamento para um arquivo ou pasta</span><span class="sxs-lookup"><span data-stu-id="923af-102">Get sharing permission for a file or folder</span></span>

<span data-ttu-id="923af-103">Retornar a permissão de compartilhamento eficaz de um recurso de permissão específico.</span><span class="sxs-lookup"><span data-stu-id="923af-103">Return the effective sharing permission for a particular permission resource.</span></span>

<span data-ttu-id="923af-104">Permissões efetivas de um item podem vir de duas fontes: permissões definidas diretamente no próprio item, ou permissões herdadas de ancestrais do item.</span><span class="sxs-lookup"><span data-stu-id="923af-104">Effective permissions of an item can come from two sources: permissions set directly on the item itself or permissions that are inherited from the item's ancestors.</span></span>

<span data-ttu-id="923af-p101">Os chamadores podem diferenciar se a permissão é herdada ou não verificando a propriedade `inheritedFrom` Esta propriedade é um recurso [itemReference](../resources/itemreference.md) que faz referência ao ancestral do qual a permissão é herdada.</span><span class="sxs-lookup"><span data-stu-id="923af-p101">Callers can differentiate if the permission is inherited or not by checking the `inheritedFrom` property. This property is an [ItemReference](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="923af-107">Níveis de permissão do SharePoint definidos em um item retornam com um prefixo 'SP'.</span><span class="sxs-lookup"><span data-stu-id="923af-107">SharePoint permission levels set on an item are returned with an 'SP' prefix.</span></span> <span data-ttu-id="923af-108">Por exemplo, SP.Somente exibição, SP.Acesso limitado, SP.Exibir Dados do Web Analytics.</span><span class="sxs-lookup"><span data-stu-id="923af-108">For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data.</span></span> <span data-ttu-id="923af-109">Consulte a [Lista completa de funções do SharePoint](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span><span class="sxs-lookup"><span data-stu-id="923af-109">See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="permissions"></a><span data-ttu-id="923af-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="923af-110">Permissions</span></span>

<span data-ttu-id="923af-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="923af-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="923af-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="923af-113">Permission type</span></span>      | <span data-ttu-id="923af-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="923af-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="923af-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="923af-115">Delegated (work or school account)</span></span> | <span data-ttu-id="923af-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="923af-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="923af-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="923af-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="923af-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="923af-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="923af-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="923af-119">Application</span></span> | <span data-ttu-id="923af-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="923af-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="923af-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="923af-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
GET /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="923af-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="923af-122">Optional query parameters</span></span>

<span data-ttu-id="923af-123">Esse método é compatível com o [parâmetro de consulta $select](/graph/query-parameters) para formar a resposta.</span><span class="sxs-lookup"><span data-stu-id="923af-123">This method support the [$select query parameter](/graph/query-parameters) to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="923af-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="923af-124">Response</span></span>

<span data-ttu-id="923af-125">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [Permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="923af-125">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="923af-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="923af-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="923af-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="923af-127">Request</span></span>

<span data-ttu-id="923af-128">Aqui está um exemplo da solicitação para acessar uma permissão em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="923af-128">Here is an example of the request to access a permission on a folder.</span></span>

<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a><span data-ttu-id="923af-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="923af-129">Response</span></span>

<span data-ttu-id="923af-130">Se for bem-sucedido, esse método retornará um recurso [Permission](../resources/permission.md) para a ID especificada.</span><span class="sxs-lookup"><span data-stu-id="923af-130">If successful, this method returns a [Permission](../resources/permission.md) resource for the specified ID.</span></span> 

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a><span data-ttu-id="923af-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="923af-131">Remarks</span></span>

<span data-ttu-id="923af-132">O recurso [Permission](../resources/permission.md) usa _facets_ para fornecer informações sobre o tipo de permissão representado pelo recurso.</span><span class="sxs-lookup"><span data-stu-id="923af-132">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="923af-p104">Permissões com uma faceta [**link**](../resources/sharinglink.md) representam links de compartilhamento criados no item. Os links de compartilhamento contêm um token exclusivo que fornece acesso ao item para qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="923af-p104">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="923af-135">Permissões com uma faceta [**invitation**](../resources/sharinginvitation.md) representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="923af-135">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

### <a name="error-responses"></a><span data-ttu-id="923af-136">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="923af-136">Error responses</span></span>

<span data-ttu-id="923af-137">Saiba mais sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="923af-137">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get a DriveItem's sharing permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions"
} -->
