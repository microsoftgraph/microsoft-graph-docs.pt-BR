---
title: Atribuir um conector a um aplicativo
description: Use esta API para atribuir um conector a um aplicativo
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1d937f6a52d80896714519bc43b0dc2595f9d902
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996413"
---
# <a name="assign-a-connectorgroup-to-an-application"></a><span data-ttu-id="7b5f1-103">Atribuir um conector a um aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b5f1-103">Assign a connectorGroup to an application</span></span>

<span data-ttu-id="7b5f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b5f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b5f1-105">Atribuir um [conector](../resources/connectorgroup.md) a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="7b5f1-105">Assign a [connectorGroup](../resources/connectorgroup.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b5f1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b5f1-106">Permissions</span></span>
<span data-ttu-id="7b5f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b5f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b5f1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b5f1-109">Permission type</span></span>      | <span data-ttu-id="7b5f1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b5f1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b5f1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b5f1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7b5f1-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7b5f1-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7b5f1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b5f1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b5f1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b5f1-114">Not supported.</span></span>    |
|<span data-ttu-id="7b5f1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b5f1-115">Application</span></span> | <span data-ttu-id="7b5f1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b5f1-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7b5f1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b5f1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /applications/{id}/connectorGroup/$ref

```
## <a name="request-headers"></a><span data-ttu-id="7b5f1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b5f1-118">Request headers</span></span>
| <span data-ttu-id="7b5f1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7b5f1-119">Name</span></span>       | <span data-ttu-id="7b5f1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b5f1-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7b5f1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b5f1-121">Authorization</span></span>  | <span data-ttu-id="7b5f1-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="7b5f1-122">Bearer.</span></span> <span data-ttu-id="7b5f1-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b5f1-123">Required.</span></span>|
| <span data-ttu-id="7b5f1-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="7b5f1-124">Content-type</span></span> | <span data-ttu-id="7b5f1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b5f1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b5f1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b5f1-127">Request body</span></span>
<span data-ttu-id="7b5f1-128">No corpo da solicitação, forneça uma representação JSON de um objeto do objeto de [conexão](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="7b5f1-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7b5f1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b5f1-129">Response</span></span>

<span data-ttu-id="7b5f1-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b5f1-130">If successful, this method returns `201 Created` response code and an [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b5f1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b5f1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b5f1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b5f1-132">Request</span></span>
<span data-ttu-id="7b5f1-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b5f1-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7b5f1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b5f1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/connectorGroup/$ref

Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="7b5f1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b5f1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7b5f1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b5f1-136">Response</span></span>
<span data-ttu-id="7b5f1-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7b5f1-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Assign a connectorGroup to an application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


