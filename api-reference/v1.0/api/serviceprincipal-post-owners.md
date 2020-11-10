---
title: 'servicePrincipal: Adicionar proprietário'
description: Use esta API para adicionar um proprietário para a entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 8a1c063046d9d0deab8acfec7a78d9c28507a9fa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980065"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="29fef-103">servicePrincipal: Adicionar proprietário</span><span class="sxs-lookup"><span data-stu-id="29fef-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="29fef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29fef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="29fef-105">Use esta API para adicionar um proprietário para a [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="29fef-105">Use this API to add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="29fef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="29fef-106">Permissions</span></span>
<span data-ttu-id="29fef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29fef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29fef-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29fef-109">Permission type</span></span>      | <span data-ttu-id="29fef-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29fef-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29fef-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29fef-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="29fef-112">Application.ReadWrite.All e Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29fef-112">Application.ReadWrite.All and Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29fef-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29fef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29fef-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29fef-114">Not supported.</span></span>    |
|<span data-ttu-id="29fef-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29fef-115">Application</span></span> | <span data-ttu-id="29fef-116">Application.ReadWrite.OwnedBy e Directory.Read.All, Application.ReadWrite.All e Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="29fef-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29fef-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29fef-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="29fef-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29fef-118">Request headers</span></span>
| <span data-ttu-id="29fef-119">Nome</span><span class="sxs-lookup"><span data-stu-id="29fef-119">Name</span></span>       | <span data-ttu-id="29fef-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="29fef-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="29fef-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="29fef-121">Authorization</span></span> | <span data-ttu-id="29fef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29fef-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="29fef-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29fef-124">Content-Type</span></span> | <span data-ttu-id="29fef-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29fef-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29fef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29fef-127">Request body</span></span>
<span data-ttu-id="29fef-128">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="29fef-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="29fef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="29fef-129">Response</span></span>

<span data-ttu-id="29fef-130">Se bem-sucedido, este método retorna um código de resposta `204 No Content` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29fef-130">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29fef-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="29fef-131">Examples</span></span>
### <a name="request"></a><span data-ttu-id="29fef-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29fef-132">Request</span></span>
<span data-ttu-id="29fef-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29fef-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="29fef-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="29fef-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="29fef-135">C#</span><span class="sxs-lookup"><span data-stu-id="29fef-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29fef-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29fef-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29fef-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29fef-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29fef-138">Java</span><span class="sxs-lookup"><span data-stu-id="29fef-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="29fef-139">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="29fef-139">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="29fef-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="29fef-140">Response</span></span>
<span data-ttu-id="29fef-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="29fef-141">The following is an example of the response.</span></span>

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

