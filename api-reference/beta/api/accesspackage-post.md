---
title: Criar accessPackage
description: Criar um novo accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a70de297dcd22588914d8613635687f07aaf40b0
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994110"
---
# <a name="create-accesspackage"></a><span data-ttu-id="bcc7a-103">Criar accessPackage</span><span class="sxs-lookup"><span data-stu-id="bcc7a-103">Create accessPackage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcc7a-104">Criar um novo objeto [accessPackage](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="bcc7a-104">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcc7a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bcc7a-105">Permissions</span></span>

<span data-ttu-id="bcc7a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcc7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bcc7a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcc7a-108">Permission type</span></span>                        | <span data-ttu-id="bcc7a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bcc7a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bcc7a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcc7a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bcc7a-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcc7a-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="bcc7a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcc7a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcc7a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcc7a-113">Not supported.</span></span> |
| <span data-ttu-id="bcc7a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bcc7a-114">Application</span></span>                            | <span data-ttu-id="bcc7a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcc7a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcc7a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcc7a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="bcc7a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcc7a-117">Request headers</span></span>

| <span data-ttu-id="bcc7a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bcc7a-118">Name</span></span>          | <span data-ttu-id="bcc7a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcc7a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bcc7a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcc7a-120">Authorization</span></span> | <span data-ttu-id="bcc7a-121">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="bcc7a-121">Bearer \{token\}.</span></span> <span data-ttu-id="bcc7a-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcc7a-122">Required.</span></span> |
| <span data-ttu-id="bcc7a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bcc7a-123">Content-Type</span></span>  | <span data-ttu-id="bcc7a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bcc7a-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bcc7a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcc7a-125">Request body</span></span>

<span data-ttu-id="bcc7a-126">No corpo da solicitação, forneça uma representação JSON do objeto [accessPackage](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="bcc7a-126">In the request body, supply a JSON representation of [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bcc7a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcc7a-127">Response</span></span>

<span data-ttu-id="bcc7a-128">Se tiver êxito, este método retornará um código de resposta criado 201 e um novo objeto [accessPackage](../resources/accesspackage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcc7a-128">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bcc7a-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bcc7a-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bcc7a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcc7a-130">Request</span></span>

<span data-ttu-id="bcc7a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcc7a-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bcc7a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcc7a-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="bcc7a-133">C#</span><span class="sxs-lookup"><span data-stu-id="bcc7a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackage-from-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bcc7a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcc7a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackage-from-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bcc7a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcc7a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackage-from-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bcc7a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcc7a-136">Response</span></span>

<span data-ttu-id="bcc7a-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bcc7a-137">The following is an example of the response.</span></span>

> <span data-ttu-id="bcc7a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bcc7a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
