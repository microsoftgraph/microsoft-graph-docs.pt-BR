---
title: Obter contrato
description: Recupere as propriedades e as relações de um objeto de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 96c574b688958b48a90074e4d7b830eba0501677
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048208"
---
# <a name="get-agreement"></a><span data-ttu-id="04ae6-103">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="04ae6-103">Get agreement</span></span>

<span data-ttu-id="04ae6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04ae6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04ae6-105">Recupere as propriedades e as relações de um [objeto de](../resources/agreement.md) contrato.</span><span class="sxs-lookup"><span data-stu-id="04ae6-105">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="04ae6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="04ae6-106">Permissions</span></span>
<span data-ttu-id="04ae6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04ae6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04ae6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04ae6-109">Permission type</span></span>                        | <span data-ttu-id="04ae6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04ae6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="04ae6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04ae6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="04ae6-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="04ae6-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="04ae6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04ae6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04ae6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04ae6-114">Not supported.</span></span> |
|<span data-ttu-id="04ae6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04ae6-115">Application</span></span>                            | <span data-ttu-id="04ae6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04ae6-116">Not supported.</span></span> |

<span data-ttu-id="04ae6-117">Ao chamar em nome de um usuário, o usuário precisa pertencer a uma das seguintes funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="04ae6-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="04ae6-118">Para saber mais sobre funções de diretório, consulte Funções do [Azure AD integrados](/azure/active-directory/roles/permissions-reference):</span><span class="sxs-lookup"><span data-stu-id="04ae6-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="04ae6-119">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="04ae6-119">Global Administrator</span></span>
+ <span data-ttu-id="04ae6-120">Administrador de Acesso Condicional</span><span class="sxs-lookup"><span data-stu-id="04ae6-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="04ae6-121">Administrador de Segurança</span><span class="sxs-lookup"><span data-stu-id="04ae6-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="04ae6-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04ae6-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements/{id}
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="04ae6-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04ae6-123">Request headers</span></span>
| <span data-ttu-id="04ae6-124">Nome</span><span class="sxs-lookup"><span data-stu-id="04ae6-124">Name</span></span>         | <span data-ttu-id="04ae6-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="04ae6-125">Type</span></span>        | <span data-ttu-id="04ae6-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="04ae6-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="04ae6-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="04ae6-127">Authorization</span></span> | <span data-ttu-id="04ae6-128">string</span><span class="sxs-lookup"><span data-stu-id="04ae6-128">string</span></span> | <span data-ttu-id="04ae6-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04ae6-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04ae6-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04ae6-131">Request body</span></span>
<span data-ttu-id="04ae6-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04ae6-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="04ae6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="04ae6-133">Response</span></span>
<span data-ttu-id="04ae6-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04ae6-134">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="04ae6-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04ae6-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04ae6-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04ae6-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="04ae6-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="04ae6-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}?$expand=files
```
# <a name="c"></a>[<span data-ttu-id="04ae6-138">C#</span><span class="sxs-lookup"><span data-stu-id="04ae6-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04ae6-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04ae6-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04ae6-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04ae6-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04ae6-141">Java</span><span class="sxs-lookup"><span data-stu-id="04ae6-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="04ae6-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="04ae6-142">Response</span></span>
><span data-ttu-id="04ae6-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="04ae6-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
