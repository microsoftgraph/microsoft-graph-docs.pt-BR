---
title: Criar accessPackage
description: Crie um novo accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e6f6a80316bbdf12792bb47078be7f4e3ca9b48c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048642"
---
# <a name="create-accesspackage"></a><span data-ttu-id="14bf5-103">Criar accessPackage</span><span class="sxs-lookup"><span data-stu-id="14bf5-103">Create accessPackage</span></span>

<span data-ttu-id="14bf5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14bf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14bf5-105">Crie um novo [objeto accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="14bf5-105">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="14bf5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="14bf5-106">Permissions</span></span>

<span data-ttu-id="14bf5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14bf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14bf5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14bf5-109">Permission type</span></span>                        | <span data-ttu-id="14bf5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14bf5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="14bf5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14bf5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="14bf5-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14bf5-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="14bf5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14bf5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14bf5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14bf5-114">Not supported.</span></span> |
| <span data-ttu-id="14bf5-115">Application</span><span class="sxs-lookup"><span data-stu-id="14bf5-115">Application</span></span>                            | <span data-ttu-id="14bf5-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14bf5-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14bf5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14bf5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="14bf5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14bf5-118">Request headers</span></span>

| <span data-ttu-id="14bf5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="14bf5-119">Name</span></span>          | <span data-ttu-id="14bf5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="14bf5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="14bf5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="14bf5-121">Authorization</span></span> | <span data-ttu-id="14bf5-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14bf5-p102">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="14bf5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="14bf5-124">Content-Type</span></span>  | <span data-ttu-id="14bf5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14bf5-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="14bf5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14bf5-126">Request body</span></span>

<span data-ttu-id="14bf5-127">No corpo da solicitação, fornece uma representação JSON do [objeto accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="14bf5-127">In the request body, supply a JSON representation of [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="14bf5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="14bf5-128">Response</span></span>

<span data-ttu-id="14bf5-129">Se tiver êxito, este método retornará um código de resposta Criado 201 e um novo [objeto accessPackage](../resources/accesspackage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14bf5-129">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14bf5-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="14bf5-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14bf5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14bf5-131">Request</span></span>

<span data-ttu-id="14bf5-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14bf5-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14bf5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="14bf5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackage_from_accesspackages"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
Content-type: application/json

{
  "catalogId": "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  "displayName": "sales reps",
  "description": "outside sales representatives"
}
```
# <a name="c"></a>[<span data-ttu-id="14bf5-134">C#</span><span class="sxs-lookup"><span data-stu-id="14bf5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackage-from-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14bf5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14bf5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackage-from-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14bf5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14bf5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackage-from-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14bf5-137">Java</span><span class="sxs-lookup"><span data-stu-id="14bf5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackage-from-accesspackages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14bf5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="14bf5-138">Response</span></span>

<span data-ttu-id="14bf5-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14bf5-139">The following is an example of the response.</span></span>

> <span data-ttu-id="14bf5-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="14bf5-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "catalogId": "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  "displayName": "sales reps",
  "description": "outside sales representatives",
  "isHidden": false,
  "isRoleScopesVisible": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


