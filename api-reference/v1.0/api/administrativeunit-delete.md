---
title: Excluir administrativeUnit
description: Excluir um administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 79739889099924555d5282689ea0baa310bc2844
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054221"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="0d46e-103">Excluir administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="0d46e-103">Delete administrativeUnit</span></span>

<span data-ttu-id="0d46e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d46e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d46e-105">Excluir um [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="0d46e-105">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0d46e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d46e-106">Permissions</span></span>
<span data-ttu-id="0d46e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d46e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0d46e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d46e-109">Permission type</span></span>      | <span data-ttu-id="0d46e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d46e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d46e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d46e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0d46e-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0d46e-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0d46e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d46e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d46e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d46e-114">Not supported.</span></span>    |
|<span data-ttu-id="0d46e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d46e-115">Application</span></span> | <span data-ttu-id="0d46e-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d46e-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d46e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d46e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0d46e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d46e-118">Request headers</span></span>
| <span data-ttu-id="0d46e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0d46e-119">Name</span></span>       | <span data-ttu-id="0d46e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d46e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0d46e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d46e-121">Authorization</span></span>  | <span data-ttu-id="0d46e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d46e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d46e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d46e-124">Request body</span></span>
<span data-ttu-id="0d46e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d46e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d46e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d46e-126">Response</span></span>

<span data-ttu-id="0d46e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d46e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d46e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d46e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d46e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d46e-130">Request</span></span>
<span data-ttu-id="0d46e-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d46e-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0d46e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d46e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}
```
# <a name="c"></a>[<span data-ttu-id="0d46e-133">C#</span><span class="sxs-lookup"><span data-stu-id="0d46e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d46e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d46e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d46e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d46e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0d46e-136">Java</span><span class="sxs-lookup"><span data-stu-id="0d46e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="0d46e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d46e-137">Response</span></span>
<span data-ttu-id="0d46e-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d46e-138">Here is an example of the response.</span></span> <span data-ttu-id="0d46e-139">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0d46e-139">Note: The response object shown here might be shortened for readability.</span></span>
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
