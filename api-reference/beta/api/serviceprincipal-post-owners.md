---
title: 'servicePrincipalName: Adicionar proprietário'
description: Adicione um proprietário para a entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 2c31da548b332b0974fa4846ec5583ac71299075
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333468"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="42d65-103">servicePrincipalName: Adicionar proprietário</span><span class="sxs-lookup"><span data-stu-id="42d65-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="42d65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42d65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42d65-105">Adicione um proprietário para o [servicePrincipalName](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="42d65-105">Add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="42d65-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="42d65-106">Permissions</span></span>
<span data-ttu-id="42d65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42d65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42d65-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42d65-109">Permission type</span></span>      | <span data-ttu-id="42d65-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42d65-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42d65-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42d65-111">Delegated (work or school account)</span></span> | <span data-ttu-id="42d65-112">Application. ReadWrite. All e Directory. Read. All, Application. ReadWrite. All e Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="42d65-112">Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.All and Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="42d65-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42d65-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42d65-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42d65-114">Not supported.</span></span>    |
|<span data-ttu-id="42d65-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42d65-115">Application</span></span> | <span data-ttu-id="42d65-116">Application. ReadWrite. OwnedBy e Directory. Read. All, Application. ReadWrite. All e Directory. Read. All, Application. ReadWrite. OwnedBy e Directory. ReadWrite. All, Application. ReadWrite. All e Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="42d65-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.OwnedBy and Directory.ReadWrite.All, Application.ReadWrite.All and Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="42d65-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42d65-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="42d65-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42d65-118">Request headers</span></span>
| <span data-ttu-id="42d65-119">Nome</span><span class="sxs-lookup"><span data-stu-id="42d65-119">Name</span></span>       | <span data-ttu-id="42d65-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="42d65-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="42d65-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="42d65-121">Authorization</span></span> | <span data-ttu-id="42d65-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42d65-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="42d65-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42d65-124">Request body</span></span>
<span data-ttu-id="42d65-125">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md) .</span><span class="sxs-lookup"><span data-stu-id="42d65-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="42d65-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="42d65-126">Response</span></span>

<span data-ttu-id="42d65-127">Se bem-sucedido, este método retorna um código de resposta `204 No Content` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42d65-127">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42d65-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="42d65-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="42d65-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42d65-129">Request</span></span>
<span data-ttu-id="42d65-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42d65-130">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="42d65-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="42d65-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="42d65-132">C#</span><span class="sxs-lookup"><span data-stu-id="42d65-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42d65-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42d65-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42d65-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42d65-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="42d65-135">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md) .</span><span class="sxs-lookup"><span data-stu-id="42d65-135">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="42d65-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="42d65-136">Response</span></span>
<span data-ttu-id="42d65-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="42d65-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
