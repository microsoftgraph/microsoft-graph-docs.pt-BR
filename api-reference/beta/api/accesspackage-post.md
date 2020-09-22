---
title: Criar accessPackage
description: Criar um novo accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2fc35b0c2de4f8d152cef00194bf74b5fd5b8845
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977948"
---
# <a name="create-accesspackage"></a><span data-ttu-id="6da39-103">Criar accessPackage</span><span class="sxs-lookup"><span data-stu-id="6da39-103">Create accessPackage</span></span>

<span data-ttu-id="6da39-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6da39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6da39-105">Criar um novo objeto [accessPackage](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="6da39-105">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6da39-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6da39-106">Permissions</span></span>

<span data-ttu-id="6da39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6da39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6da39-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6da39-109">Permission type</span></span>                        | <span data-ttu-id="6da39-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6da39-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6da39-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6da39-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6da39-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6da39-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="6da39-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6da39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6da39-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6da39-114">Not supported.</span></span> |
| <span data-ttu-id="6da39-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6da39-115">Application</span></span>                            | <span data-ttu-id="6da39-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6da39-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6da39-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6da39-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="6da39-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6da39-118">Request headers</span></span>

| <span data-ttu-id="6da39-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6da39-119">Name</span></span>          | <span data-ttu-id="6da39-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6da39-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6da39-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6da39-121">Authorization</span></span> | <span data-ttu-id="6da39-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="6da39-122">Bearer \{token\}.</span></span> <span data-ttu-id="6da39-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6da39-123">Required.</span></span> |
| <span data-ttu-id="6da39-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6da39-124">Content-Type</span></span>  | <span data-ttu-id="6da39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6da39-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6da39-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6da39-126">Request body</span></span>

<span data-ttu-id="6da39-127">No corpo da solicitação, forneça uma representação JSON do objeto [accessPackage](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="6da39-127">In the request body, supply a JSON representation of [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6da39-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6da39-128">Response</span></span>

<span data-ttu-id="6da39-129">Se tiver êxito, este método retornará um código de resposta criado 201 e um novo objeto [accessPackage](../resources/accesspackage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6da39-129">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6da39-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6da39-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6da39-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6da39-131">Request</span></span>

<span data-ttu-id="6da39-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6da39-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6da39-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6da39-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6da39-134">C#</span><span class="sxs-lookup"><span data-stu-id="6da39-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackage-from-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6da39-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6da39-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackage-from-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6da39-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6da39-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackage-from-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6da39-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6da39-137">Response</span></span>

<span data-ttu-id="6da39-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6da39-138">The following is an example of the response.</span></span>

> <span data-ttu-id="6da39-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6da39-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


