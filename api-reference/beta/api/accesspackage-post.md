---
title: Criar accessPackage
description: Criar um novo accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3657d5ba4e3fbe120ec5bf92ebf3ddd25c43c13e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952270"
---
# <a name="create-accesspackage"></a><span data-ttu-id="84f2e-103">Criar accessPackage</span><span class="sxs-lookup"><span data-stu-id="84f2e-103">Create accessPackage</span></span>

<span data-ttu-id="84f2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84f2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84f2e-105">Criar um novo objeto [accessPackage](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="84f2e-105">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="84f2e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="84f2e-106">Permissions</span></span>

<span data-ttu-id="84f2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84f2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84f2e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84f2e-109">Permission type</span></span>                        | <span data-ttu-id="84f2e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84f2e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="84f2e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84f2e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="84f2e-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84f2e-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="84f2e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84f2e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84f2e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84f2e-114">Not supported.</span></span> |
| <span data-ttu-id="84f2e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84f2e-115">Application</span></span>                            | <span data-ttu-id="84f2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84f2e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84f2e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84f2e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="84f2e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84f2e-118">Request headers</span></span>

| <span data-ttu-id="84f2e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="84f2e-119">Name</span></span>          | <span data-ttu-id="84f2e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="84f2e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="84f2e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="84f2e-121">Authorization</span></span> | <span data-ttu-id="84f2e-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="84f2e-122">Bearer \{token\}.</span></span> <span data-ttu-id="84f2e-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84f2e-123">Required.</span></span> |
| <span data-ttu-id="84f2e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="84f2e-124">Content-Type</span></span>  | <span data-ttu-id="84f2e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84f2e-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="84f2e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84f2e-126">Request body</span></span>

<span data-ttu-id="84f2e-127">No corpo da solicitação, forneça uma representação JSON do objeto [accessPackage](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="84f2e-127">In the request body, supply a JSON representation of [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="84f2e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="84f2e-128">Response</span></span>

<span data-ttu-id="84f2e-129">Se tiver êxito, este método retornará um código de resposta criado 201 e um novo objeto [accessPackage](../resources/accesspackage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84f2e-129">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="84f2e-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="84f2e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="84f2e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84f2e-131">Request</span></span>

<span data-ttu-id="84f2e-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="84f2e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="84f2e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="84f2e-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="84f2e-134">C#</span><span class="sxs-lookup"><span data-stu-id="84f2e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackage-from-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84f2e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84f2e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackage-from-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84f2e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84f2e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackage-from-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84f2e-137">Java</span><span class="sxs-lookup"><span data-stu-id="84f2e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackage-from-accesspackages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="84f2e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="84f2e-138">Response</span></span>

<span data-ttu-id="84f2e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="84f2e-139">The following is an example of the response.</span></span>

> <span data-ttu-id="84f2e-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84f2e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


