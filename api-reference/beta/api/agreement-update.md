---
title: Atualizar contrato
description: Atualize as propriedades de um objeto agreement.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 77c3fbf6aa37d283e02408a1000d4a5f521a3fd5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048194"
---
# <a name="update-agreement"></a><span data-ttu-id="2471e-103">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="2471e-103">Update agreement</span></span>

<span data-ttu-id="2471e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2471e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2471e-105">Atualize as propriedades de um [objeto agreement.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="2471e-105">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2471e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2471e-106">Permissions</span></span>
<span data-ttu-id="2471e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2471e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2471e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2471e-109">Permission type</span></span>                        | <span data-ttu-id="2471e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2471e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2471e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2471e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2471e-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2471e-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="2471e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2471e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2471e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2471e-114">Not supported.</span></span> |
|<span data-ttu-id="2471e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2471e-115">Application</span></span>                            | <span data-ttu-id="2471e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2471e-116">Not supported.</span></span> |

<span data-ttu-id="2471e-117">Ao chamar em nome de um usuário, o usuário precisa pertencer a uma das seguintes funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="2471e-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="2471e-118">Para saber mais sobre funções de diretório, consulte Funções do [Azure AD integrados](/azure/active-directory/roles/permissions-reference):</span><span class="sxs-lookup"><span data-stu-id="2471e-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="2471e-119">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="2471e-119">Global Administrator</span></span>
+ <span data-ttu-id="2471e-120">Administrador de Acesso Condicional</span><span class="sxs-lookup"><span data-stu-id="2471e-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="2471e-121">Administrador de Segurança</span><span class="sxs-lookup"><span data-stu-id="2471e-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="2471e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2471e-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2471e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2471e-123">Request headers</span></span>
| <span data-ttu-id="2471e-124">Nome</span><span class="sxs-lookup"><span data-stu-id="2471e-124">Name</span></span>         | <span data-ttu-id="2471e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="2471e-125">Type</span></span>        | <span data-ttu-id="2471e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="2471e-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2471e-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="2471e-127">Authorization</span></span> | <span data-ttu-id="2471e-128">string</span><span class="sxs-lookup"><span data-stu-id="2471e-128">string</span></span> | <span data-ttu-id="2471e-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2471e-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2471e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2471e-131">Request body</span></span>
<span data-ttu-id="2471e-132">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="2471e-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2471e-133">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="2471e-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2471e-134">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2471e-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2471e-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2471e-135">Property</span></span>     | <span data-ttu-id="2471e-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="2471e-136">Type</span></span>        | <span data-ttu-id="2471e-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="2471e-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2471e-138">displayName</span><span class="sxs-lookup"><span data-stu-id="2471e-138">displayName</span></span>|<span data-ttu-id="2471e-139">String</span><span class="sxs-lookup"><span data-stu-id="2471e-139">String</span></span>|<span data-ttu-id="2471e-140">Nome de exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="2471e-140">Display name of the agreement.</span></span>|
|<span data-ttu-id="2471e-141">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="2471e-141">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="2471e-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="2471e-142">Boolean</span></span>|<span data-ttu-id="2471e-143">Se o usuário precisa expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="2471e-143">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="2471e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2471e-144">Response</span></span>
<span data-ttu-id="2471e-145">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de [contrato](../resources/agreement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2471e-145">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2471e-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2471e-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2471e-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2471e-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2471e-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="2471e-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```
# <a name="c"></a>[<span data-ttu-id="2471e-149">C#</span><span class="sxs-lookup"><span data-stu-id="2471e-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2471e-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2471e-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2471e-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2471e-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2471e-152">Java</span><span class="sxs-lookup"><span data-stu-id="2471e-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2471e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="2471e-153">Response</span></span>
><span data-ttu-id="2471e-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2471e-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 105

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


