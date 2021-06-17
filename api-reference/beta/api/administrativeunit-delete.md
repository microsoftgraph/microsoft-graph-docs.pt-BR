---
title: Excluir administrativeUnit
description: Excluir um administrativeUnit.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6b9f2c9813e56475280109ad8fd66ee4680ea663
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992048"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="ca5d2-103">Excluir administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="ca5d2-103">Delete administrativeUnit</span></span>

<span data-ttu-id="ca5d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca5d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca5d2-105">Excluir um [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="ca5d2-105">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca5d2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ca5d2-106">Permissions</span></span>
<span data-ttu-id="ca5d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca5d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ca5d2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca5d2-109">Permission type</span></span>      | <span data-ttu-id="ca5d2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca5d2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca5d2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca5d2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ca5d2-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ca5d2-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ca5d2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca5d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca5d2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca5d2-114">Not supported.</span></span>    |
|<span data-ttu-id="ca5d2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca5d2-115">Application</span></span> | <span data-ttu-id="ca5d2-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca5d2-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca5d2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca5d2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ca5d2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca5d2-118">Request headers</span></span>
| <span data-ttu-id="ca5d2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ca5d2-119">Name</span></span>       | <span data-ttu-id="ca5d2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca5d2-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ca5d2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca5d2-121">Authorization</span></span>  | <span data-ttu-id="ca5d2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca5d2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca5d2-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca5d2-124">Request body</span></span>
<span data-ttu-id="ca5d2-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca5d2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca5d2-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca5d2-126">Response</span></span>

<span data-ttu-id="ca5d2-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca5d2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca5d2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca5d2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca5d2-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca5d2-130">Request</span></span>
<span data-ttu-id="ca5d2-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca5d2-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca5d2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca5d2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="c"></a>[<span data-ttu-id="ca5d2-133">C#</span><span class="sxs-lookup"><span data-stu-id="ca5d2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca5d2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca5d2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca5d2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca5d2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca5d2-136">Java</span><span class="sxs-lookup"><span data-stu-id="ca5d2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ca5d2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca5d2-137">Response</span></span>
<span data-ttu-id="ca5d2-p104">Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="ca5d2-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


