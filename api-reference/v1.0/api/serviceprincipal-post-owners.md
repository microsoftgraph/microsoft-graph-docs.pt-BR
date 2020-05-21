---
title: 'servicePrincipalName: Adicionar proprietário'
description: Use esta API para adicionar um proprietário para a entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: cb0f6f8e2ce809a1e3a3dadda209975205616658
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334799"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="dacbb-103">servicePrincipalName: Adicionar proprietário</span><span class="sxs-lookup"><span data-stu-id="dacbb-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="dacbb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dacbb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dacbb-105">Use esta API para adicionar um proprietário para o [servicePrincipalName](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="dacbb-105">Use this API to add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dacbb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dacbb-106">Permissions</span></span>
<span data-ttu-id="dacbb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dacbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dacbb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dacbb-109">Permission type</span></span>      | <span data-ttu-id="dacbb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dacbb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dacbb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dacbb-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="dacbb-112">Application. ReadWrite. All e Directory. Read. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="dacbb-112">Application.ReadWrite.All and Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dacbb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dacbb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dacbb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dacbb-114">Not supported.</span></span>    |
|<span data-ttu-id="dacbb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dacbb-115">Application</span></span> | <span data-ttu-id="dacbb-116">Application. ReadWrite. OwnedBy e Directory. Read. All, Application. ReadWrite. All e Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="dacbb-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dacbb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dacbb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="dacbb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dacbb-118">Request headers</span></span>
| <span data-ttu-id="dacbb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dacbb-119">Name</span></span>       | <span data-ttu-id="dacbb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dacbb-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="dacbb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dacbb-121">Authorization</span></span> | <span data-ttu-id="dacbb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dacbb-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dacbb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dacbb-124">Content-Type</span></span> | <span data-ttu-id="dacbb-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dacbb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dacbb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dacbb-127">Request body</span></span>
<span data-ttu-id="dacbb-128">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="dacbb-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dacbb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dacbb-129">Response</span></span>

<span data-ttu-id="dacbb-130">Se bem-sucedido, este método retorna um código de resposta `204 No Content` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dacbb-130">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dacbb-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dacbb-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="dacbb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dacbb-132">Request</span></span>
<span data-ttu-id="dacbb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dacbb-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dacbb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dacbb-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dacbb-135">C#</span><span class="sxs-lookup"><span data-stu-id="dacbb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dacbb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dacbb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dacbb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dacbb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="dacbb-138">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="dacbb-138">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="dacbb-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="dacbb-139">Response</span></span>
<span data-ttu-id="dacbb-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dacbb-140">The following is an example of the response.</span></span>

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
