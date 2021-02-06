---
title: Adicionar conector a connectorGroup
description: Use essa API para adicionar um conector a um connectorGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 94b4f17dce85108d853cb0d3c21a4f9fc7bf573d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129804"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="f3281-103">Adicionar conector a connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f3281-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="f3281-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3281-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3281-105">Adicione um [conector](../resources/connector.md) a um [connectorGroup](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="f3281-105">Add a [connector](../resources/connector.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

<span data-ttu-id="f3281-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3281-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3281-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3281-108">Permission type</span></span>      | <span data-ttu-id="f3281-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3281-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3281-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3281-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f3281-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f3281-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f3281-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3281-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3281-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3281-113">Not supported.</span></span>    |
|<span data-ttu-id="f3281-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3281-114">Application</span></span> | <span data-ttu-id="f3281-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3281-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f3281-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3281-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="f3281-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3281-117">Request headers</span></span>
| <span data-ttu-id="f3281-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f3281-118">Name</span></span>       | <span data-ttu-id="f3281-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3281-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f3281-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3281-120">Authorization</span></span>  | <span data-ttu-id="f3281-121">Portador.</span><span class="sxs-lookup"><span data-stu-id="f3281-121">Bearer.</span></span> <span data-ttu-id="f3281-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3281-122">Required.</span></span>|
| <span data-ttu-id="f3281-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="f3281-123">Content-type</span></span> | <span data-ttu-id="f3281-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3281-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f3281-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3281-126">Request body</span></span>
<span data-ttu-id="f3281-127">No corpo da solicitação, fornece uma representação JSON de um link para um [objeto do](../resources/connector.md) conector.</span><span class="sxs-lookup"><span data-stu-id="f3281-127">In the request body, supply a JSON representation of a link to a [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f3281-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3281-128">Response</span></span>

<span data-ttu-id="f3281-129">Se bem-sucedido, este método retorna um código de resposta e um `201 Created` objeto [de](../resources/connector.md) conector no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3281-129">If successful, this method returns a `201 Created` response code and a [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3281-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3281-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3281-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3281-131">Request</span></span>
<span data-ttu-id="f3281-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3281-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f3281-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3281-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connector_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref
Content-type: application/json
Content-length: 104

{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="f3281-134">C#</span><span class="sxs-lookup"><span data-stu-id="f3281-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connector-from-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f3281-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3281-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connector-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f3281-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3281-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connector-from-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f3281-137">Java</span><span class="sxs-lookup"><span data-stu-id="f3281-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connector-from-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f3281-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3281-138">Response</span></span>
<span data-ttu-id="f3281-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f3281-139">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add connector to connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



