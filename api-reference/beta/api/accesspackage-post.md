---
title: Criar accessPackage
description: Crie um novo accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ccbe9c22f04087431ba0b4ae4df53eca1ff76a04
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400954"
---
# <a name="create-accesspackage"></a><span data-ttu-id="a1ed3-103">Criar accessPackage</span><span class="sxs-lookup"><span data-stu-id="a1ed3-103">Create accessPackage</span></span>

<span data-ttu-id="a1ed3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1ed3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1ed3-105">Crie um novo [objeto accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="a1ed3-105">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

<span data-ttu-id="a1ed3-106">O pacote de acesso será adicionado a um [accessPackageCatalog existente.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="a1ed3-106">The access package will be added to an existing [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span> <span data-ttu-id="a1ed3-107">Depois que o pacote de acesso for criado, você poderá criar [accessPackageAssignmentPolicies](../resources/accesspackageassignmentpolicy.md) que especificam como os usuários são atribuídos ao pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="a1ed3-107">After the access package is created, you can then create [accessPackageAssignmentPolicies](../resources/accesspackageassignmentpolicy.md) which specify how users are assigned to the access package.</span></span>


## <a name="permissions"></a><span data-ttu-id="a1ed3-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1ed3-108">Permissions</span></span>

<span data-ttu-id="a1ed3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1ed3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1ed3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1ed3-111">Permission type</span></span>                        | <span data-ttu-id="a1ed3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1ed3-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a1ed3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1ed3-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1ed3-114">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1ed3-114">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="a1ed3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1ed3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1ed3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1ed3-116">Not supported.</span></span> |
| <span data-ttu-id="a1ed3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1ed3-117">Application</span></span>                            | <span data-ttu-id="a1ed3-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1ed3-118">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1ed3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1ed3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="a1ed3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1ed3-120">Request headers</span></span>

| <span data-ttu-id="a1ed3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a1ed3-121">Name</span></span>          | <span data-ttu-id="a1ed3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1ed3-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a1ed3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1ed3-123">Authorization</span></span> | <span data-ttu-id="a1ed3-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1ed3-p103">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="a1ed3-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="a1ed3-126">Content-type</span></span>  | <span data-ttu-id="a1ed3-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1ed3-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a1ed3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1ed3-129">Request body</span></span>

<span data-ttu-id="a1ed3-130">No corpo da solicitação, fornece uma representação JSON de um [objeto accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="a1ed3-130">In the request body, supply a JSON representation of an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a1ed3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1ed3-131">Response</span></span>

<span data-ttu-id="a1ed3-132">Se tiver êxito, este método retornará um código de resposta Criado 201 e um novo [objeto accessPackage](../resources/accesspackage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1ed3-132">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a1ed3-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a1ed3-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a1ed3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1ed3-134">Request</span></span>

<span data-ttu-id="a1ed3-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1ed3-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1ed3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1ed3-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a1ed3-137">C#</span><span class="sxs-lookup"><span data-stu-id="a1ed3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackage-from-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1ed3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1ed3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackage-from-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1ed3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1ed3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackage-from-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a1ed3-140">Java</span><span class="sxs-lookup"><span data-stu-id="a1ed3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackage-from-accesspackages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a1ed3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1ed3-141">Response</span></span>

<span data-ttu-id="a1ed3-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1ed3-142">The following is an example of the response.</span></span>

> <span data-ttu-id="a1ed3-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a1ed3-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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


