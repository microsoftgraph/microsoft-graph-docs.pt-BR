---
title: Excluir administrativeUnit
description: Excluir um administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0c85db2be5c856254197bc77fac7ceea3f1ee6f0
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408651"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="c1beb-103">Excluir administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="c1beb-103">Delete administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1beb-104">Excluir um [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="c1beb-104">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1beb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c1beb-105">Permissions</span></span>
<span data-ttu-id="c1beb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1beb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c1beb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1beb-108">Permission type</span></span>      | <span data-ttu-id="c1beb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c1beb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1beb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1beb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c1beb-111">AdministrativeUnit. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="c1beb-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c1beb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1beb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1beb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1beb-113">Not supported.</span></span>    |
|<span data-ttu-id="c1beb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1beb-114">Application</span></span> | <span data-ttu-id="c1beb-115">AdministrativeUnit. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c1beb-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1beb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1beb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c1beb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1beb-117">Request headers</span></span>
| <span data-ttu-id="c1beb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c1beb-118">Name</span></span>       | <span data-ttu-id="c1beb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1beb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c1beb-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1beb-120">Authorization</span></span>  | <span data-ttu-id="c1beb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1beb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1beb-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1beb-123">Request body</span></span>
<span data-ttu-id="c1beb-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c1beb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1beb-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1beb-125">Response</span></span>

<span data-ttu-id="c1beb-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1beb-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1beb-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1beb-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1beb-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1beb-129">Request</span></span>
<span data-ttu-id="c1beb-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1beb-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1beb-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1beb-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1beb-132">C#</span><span class="sxs-lookup"><span data-stu-id="c1beb-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1beb-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1beb-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1beb-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c1beb-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c1beb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1beb-135">Response</span></span>
<span data-ttu-id="c1beb-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c1beb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
