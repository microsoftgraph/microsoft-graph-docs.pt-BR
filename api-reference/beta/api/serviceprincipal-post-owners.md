---
title: 'servicePrincipal: Adicionar proprietário'
description: Adicione um proprietário para a entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 58c994132cbda2159587f0f48ccdce59d79505cb
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134166"
---
# <a name="serviceprincipal-add-owner"></a><span data-ttu-id="5c321-103">servicePrincipal: Adicionar proprietário</span><span class="sxs-lookup"><span data-stu-id="5c321-103">servicePrincipal: Add owner</span></span>

<span data-ttu-id="5c321-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c321-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c321-105">Adicione um proprietário para a [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="5c321-105">Add an owner for the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5c321-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c321-106">Permissions</span></span>
<span data-ttu-id="5c321-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c321-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c321-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c321-109">Permission type</span></span>      | <span data-ttu-id="5c321-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c321-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c321-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c321-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c321-112">Application.ReadWrite.All e Directory.Read.All, Application.ReadWrite.All e Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5c321-112">Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.All and Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5c321-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c321-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c321-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c321-114">Not supported.</span></span>    |
|<span data-ttu-id="5c321-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c321-115">Application</span></span> | <span data-ttu-id="5c321-116">Application.ReadWrite.OwnedBy e Directory.Read.All, Application.ReadWrite.All e Directory.Read.All, Application.ReadWrite.OwnedBy e Directory.ReadWrite.All, Application.ReadWrite.All e Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c321-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Application.ReadWrite.OwnedBy and Directory.ReadWrite.All, Application.ReadWrite.All and Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5c321-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c321-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="5c321-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c321-118">Request headers</span></span>
| <span data-ttu-id="5c321-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5c321-119">Name</span></span>       | <span data-ttu-id="5c321-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c321-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="5c321-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c321-121">Authorization</span></span> | <span data-ttu-id="5c321-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c321-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5c321-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c321-124">Request body</span></span>
<span data-ttu-id="5c321-125">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="5c321-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5c321-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c321-126">Response</span></span>

<span data-ttu-id="5c321-127">Se bem-sucedido, este método retorna um código de resposta `204 No Content` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c321-127">If successful, this method returns a `204 No Content` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c321-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5c321-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="5c321-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c321-129">Request</span></span>
<span data-ttu-id="5c321-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c321-130">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5c321-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c321-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5c321-132">C#</span><span class="sxs-lookup"><span data-stu-id="5c321-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c321-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c321-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c321-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c321-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c321-135">Java</span><span class="sxs-lookup"><span data-stu-id="5c321-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="5c321-136">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="5c321-136">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="5c321-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c321-137">Response</span></span>
<span data-ttu-id="5c321-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5c321-138">The following is an example of the response.</span></span>

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



