---
title: Criar connectorGroup
description: Use essa API para criar um novo connectorGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: dd11c3b86bc2e4036f56b3bd5d83f426fab0e1bd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047151"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="ab2f3-103">Criar connectorGroup</span><span class="sxs-lookup"><span data-stu-id="ab2f3-103">Create connectorGroup</span></span>

<span data-ttu-id="ab2f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab2f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab2f3-105">Criar um novo [connectorGroup](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="ab2f3-105">Create a new [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ab2f3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab2f3-106">Permissions</span></span>
<span data-ttu-id="ab2f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab2f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab2f3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab2f3-109">Permission type</span></span>      | <span data-ttu-id="ab2f3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab2f3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab2f3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab2f3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ab2f3-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ab2f3-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ab2f3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab2f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab2f3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab2f3-114">Not supported.</span></span>    |
|<span data-ttu-id="ab2f3-115">Application</span><span class="sxs-lookup"><span data-stu-id="ab2f3-115">Application</span></span> | <span data-ttu-id="ab2f3-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab2f3-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab2f3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab2f3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups

```
## <a name="request-headers"></a><span data-ttu-id="ab2f3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab2f3-118">Request headers</span></span>
| <span data-ttu-id="ab2f3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ab2f3-119">Name</span></span>       | <span data-ttu-id="ab2f3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab2f3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ab2f3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab2f3-121">Authorization</span></span>  | <span data-ttu-id="ab2f3-122">Portador.</span><span class="sxs-lookup"><span data-stu-id="ab2f3-122">Bearer.</span></span> <span data-ttu-id="ab2f3-123">Requried</span><span class="sxs-lookup"><span data-stu-id="ab2f3-123">Requried</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab2f3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab2f3-124">Request body</span></span>
<span data-ttu-id="ab2f3-125">No corpo da solicitação, fornece uma representação JSON do [objeto connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="ab2f3-125">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ab2f3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab2f3-126">Response</span></span>

<span data-ttu-id="ab2f3-127">Se tiver êxito, este método retornará o código de resposta e o `201 Created` [objeto connectorGroup](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab2f3-127">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab2f3-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab2f3-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab2f3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab2f3-129">Request</span></span>
<span data-ttu-id="ab2f3-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab2f3-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab2f3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab2f3-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connectorgroups"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "isDefault": false
}
```
# <a name="c"></a>[<span data-ttu-id="ab2f3-132">C#</span><span class="sxs-lookup"><span data-stu-id="ab2f3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connectorgroup-from-connectorgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab2f3-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab2f3-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectorgroup-from-connectorgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab2f3-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab2f3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connectorgroup-from-connectorgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab2f3-135">Java</span><span class="sxs-lookup"><span data-stu-id="ab2f3-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connectorgroup-from-connectorgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ab2f3-136">No corpo da solicitação, fornece uma representação JSON do [objeto connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="ab2f3-136">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ab2f3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab2f3-137">Response</span></span>
<span data-ttu-id="ab2f3-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab2f3-138">Here is an example of the response.</span></span> <span data-ttu-id="ab2f3-139">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ab2f3-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false,
  "region": "region-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



