---
title: Excluir contrato
description: Excluir um objeto agreement.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 13cf687f49715a74dfae6160ca0c883267f6fdac
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942913"
---
# <a name="delete-agreement"></a><span data-ttu-id="3aae7-103">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="3aae7-103">Delete agreement</span></span>

<span data-ttu-id="3aae7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aae7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3aae7-105">Excluir um [objeto agreement.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="3aae7-105">Delete an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3aae7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3aae7-106">Permissions</span></span>
<span data-ttu-id="3aae7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3aae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aae7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3aae7-109">Permission type</span></span>                        | <span data-ttu-id="3aae7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3aae7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3aae7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3aae7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3aae7-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aae7-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="3aae7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3aae7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aae7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3aae7-114">Not supported.</span></span> |
|<span data-ttu-id="3aae7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3aae7-115">Application</span></span>                            | <span data-ttu-id="3aae7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3aae7-116">Not supported.</span></span> |

<span data-ttu-id="3aae7-117">Ao chamar em nome de um usuário, o usuário precisa pertencer a uma das seguintes funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="3aae7-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="3aae7-118">Para saber mais sobre funções de diretório, consulte Funções do [Azure AD integrados](/azure/active-directory/roles/permissions-reference):</span><span class="sxs-lookup"><span data-stu-id="3aae7-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="3aae7-119">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="3aae7-119">Global Administrator</span></span>
+ <span data-ttu-id="3aae7-120">Administrador de Acesso Condicional</span><span class="sxs-lookup"><span data-stu-id="3aae7-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="3aae7-121">Administrador de Segurança</span><span class="sxs-lookup"><span data-stu-id="3aae7-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3aae7-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3aae7-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3aae7-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3aae7-123">Request headers</span></span>
| <span data-ttu-id="3aae7-124">Nome</span><span class="sxs-lookup"><span data-stu-id="3aae7-124">Name</span></span>         | <span data-ttu-id="3aae7-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="3aae7-125">Type</span></span>        | <span data-ttu-id="3aae7-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aae7-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3aae7-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="3aae7-127">Authorization</span></span> | <span data-ttu-id="3aae7-128">string</span><span class="sxs-lookup"><span data-stu-id="3aae7-128">string</span></span> | <span data-ttu-id="3aae7-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3aae7-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3aae7-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3aae7-131">Request body</span></span>
<span data-ttu-id="3aae7-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3aae7-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3aae7-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aae7-133">Response</span></span>
<span data-ttu-id="3aae7-p104">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3aae7-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3aae7-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3aae7-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3aae7-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3aae7-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3aae7-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3aae7-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_agreement"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}
```
# <a name="c"></a>[<span data-ttu-id="3aae7-139">C#</span><span class="sxs-lookup"><span data-stu-id="3aae7-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3aae7-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3aae7-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3aae7-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3aae7-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3aae7-142">Java</span><span class="sxs-lookup"><span data-stu-id="3aae7-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3aae7-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3aae7-143">Response</span></span>
><span data-ttu-id="3aae7-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3aae7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


