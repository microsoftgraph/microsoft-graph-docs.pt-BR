---
title: Atribuir um connectorGroup a um aplicativo
description: Use essa API para atribuir um connectorGroup a um aplicativo
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: ccf3255a5d8aa7416560848a0915cdb78aa77764
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786149"
---
# <a name="assign-a-connectorgroup-to-an-application"></a><span data-ttu-id="31987-103">Atribuir um connectorGroup a um aplicativo</span><span class="sxs-lookup"><span data-stu-id="31987-103">Assign a connectorGroup to an application</span></span>

<span data-ttu-id="31987-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31987-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31987-105">Atribua um [connectorGroup](../resources/connectorgroup.md) a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="31987-105">Assign a [connectorGroup](../resources/connectorgroup.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="31987-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="31987-106">Permissions</span></span>
<span data-ttu-id="31987-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31987-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31987-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31987-109">Permission type</span></span>      | <span data-ttu-id="31987-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31987-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31987-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31987-111">Delegated (work or school account)</span></span> | <span data-ttu-id="31987-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="31987-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="31987-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31987-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31987-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31987-114">Not supported.</span></span>    |
|<span data-ttu-id="31987-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31987-115">Application</span></span> | <span data-ttu-id="31987-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31987-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="31987-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31987-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /applications/{id}/connectorGroup/$ref

```
## <a name="request-headers"></a><span data-ttu-id="31987-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31987-118">Request headers</span></span>
| <span data-ttu-id="31987-119">Nome</span><span class="sxs-lookup"><span data-stu-id="31987-119">Name</span></span>       | <span data-ttu-id="31987-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="31987-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="31987-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="31987-121">Authorization</span></span>  | <span data-ttu-id="31987-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="31987-122">Bearer.</span></span> <span data-ttu-id="31987-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31987-123">Required.</span></span>|
| <span data-ttu-id="31987-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="31987-124">Content-type</span></span> | <span data-ttu-id="31987-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31987-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="31987-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31987-127">Request body</span></span>
<span data-ttu-id="31987-128">No corpo da solicitação, fornece uma representação JSON de um [objeto connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="31987-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="31987-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="31987-129">Response</span></span>

<span data-ttu-id="31987-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31987-130">If successful, this method returns `201 Created` response code and an [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31987-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31987-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="31987-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31987-132">Request</span></span>
<span data-ttu-id="31987-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="31987-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="31987-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="31987-134">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="31987-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31987-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="31987-136">C#</span><span class="sxs-lookup"><span data-stu-id="31987-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31987-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31987-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31987-138">Java</span><span class="sxs-lookup"><span data-stu-id="31987-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-application-from-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="31987-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="31987-139">Response</span></span>
<span data-ttu-id="31987-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="31987-140">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response"
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



