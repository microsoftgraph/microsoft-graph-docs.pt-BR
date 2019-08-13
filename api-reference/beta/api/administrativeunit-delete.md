---
title: Excluir administrativeUnit
description: Excluir um administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a6978c3046c9652068021141d0b5ec9aef5c8e8d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319031"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="c4072-103">Excluir administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="c4072-103">Delete administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4072-104">Excluir um [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="c4072-104">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4072-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4072-105">Permissions</span></span>
<span data-ttu-id="c4072-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4072-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c4072-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4072-108">Permission type</span></span>      | <span data-ttu-id="c4072-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4072-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4072-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4072-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c4072-111">AdministrativeUnit. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="c4072-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c4072-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4072-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4072-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4072-113">Not supported.</span></span>    |
|<span data-ttu-id="c4072-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4072-114">Application</span></span> | <span data-ttu-id="c4072-115">AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c4072-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4072-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4072-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c4072-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4072-117">Request headers</span></span>
| <span data-ttu-id="c4072-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c4072-118">Name</span></span>       | <span data-ttu-id="c4072-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4072-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c4072-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4072-120">Authorization</span></span>  | <span data-ttu-id="c4072-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4072-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4072-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4072-123">Request body</span></span>
<span data-ttu-id="c4072-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4072-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4072-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4072-125">Response</span></span>

<span data-ttu-id="c4072-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4072-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4072-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4072-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4072-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4072-129">Request</span></span>
<span data-ttu-id="c4072-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4072-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c4072-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4072-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4072-132">C#</span><span class="sxs-lookup"><span data-stu-id="c4072-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4072-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4072-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4072-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c4072-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c4072-135">Java</span><span class="sxs-lookup"><span data-stu-id="c4072-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c4072-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4072-136">Response</span></span>
<span data-ttu-id="c4072-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4072-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
