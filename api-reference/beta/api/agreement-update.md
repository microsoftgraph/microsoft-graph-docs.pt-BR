---
title: Atualizar contrato
description: Atualize as propriedades de um objeto agreement.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: ee62ae7f42c958304549883afbd66e022230bdd5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942868"
---
# <a name="update-agreement"></a><span data-ttu-id="181ec-103">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="181ec-103">Update agreement</span></span>

<span data-ttu-id="181ec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="181ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="181ec-105">Atualize as propriedades de um [objeto agreement.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="181ec-105">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="181ec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="181ec-106">Permissions</span></span>
<span data-ttu-id="181ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="181ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="181ec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="181ec-109">Permission type</span></span>                        | <span data-ttu-id="181ec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="181ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="181ec-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="181ec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="181ec-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="181ec-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="181ec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="181ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="181ec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="181ec-114">Not supported.</span></span> |
|<span data-ttu-id="181ec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="181ec-115">Application</span></span>                            | <span data-ttu-id="181ec-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="181ec-116">Not supported.</span></span> |

<span data-ttu-id="181ec-117">Ao chamar em nome de um usuário, o usuário precisa pertencer a uma das seguintes funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="181ec-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="181ec-118">Para saber mais sobre funções de diretório, consulte Funções do [Azure AD integrados](/azure/active-directory/roles/permissions-reference):</span><span class="sxs-lookup"><span data-stu-id="181ec-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="181ec-119">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="181ec-119">Global Administrator</span></span>
+ <span data-ttu-id="181ec-120">Administrador de Acesso Condicional</span><span class="sxs-lookup"><span data-stu-id="181ec-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="181ec-121">Administrador de Segurança</span><span class="sxs-lookup"><span data-stu-id="181ec-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="181ec-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="181ec-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="181ec-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="181ec-123">Request headers</span></span>
| <span data-ttu-id="181ec-124">Nome</span><span class="sxs-lookup"><span data-stu-id="181ec-124">Name</span></span>         | <span data-ttu-id="181ec-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="181ec-125">Type</span></span>        | <span data-ttu-id="181ec-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="181ec-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="181ec-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="181ec-127">Authorization</span></span> | <span data-ttu-id="181ec-128">string</span><span class="sxs-lookup"><span data-stu-id="181ec-128">string</span></span> | <span data-ttu-id="181ec-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="181ec-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="181ec-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="181ec-131">Request body</span></span>
<span data-ttu-id="181ec-132">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="181ec-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="181ec-133">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="181ec-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="181ec-134">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="181ec-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="181ec-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="181ec-135">Property</span></span>     | <span data-ttu-id="181ec-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="181ec-136">Type</span></span>        | <span data-ttu-id="181ec-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="181ec-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="181ec-138">displayName</span><span class="sxs-lookup"><span data-stu-id="181ec-138">displayName</span></span>|<span data-ttu-id="181ec-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="181ec-139">String</span></span>|<span data-ttu-id="181ec-140">Nome de exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="181ec-140">Display name of the agreement.</span></span>|
|<span data-ttu-id="181ec-141">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="181ec-141">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="181ec-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="181ec-142">Boolean</span></span>|<span data-ttu-id="181ec-143">Se o usuário precisa expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="181ec-143">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="181ec-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="181ec-144">Response</span></span>
<span data-ttu-id="181ec-145">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de [contrato](../resources/agreement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="181ec-145">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="181ec-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="181ec-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="181ec-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="181ec-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="181ec-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="181ec-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="181ec-149">C#</span><span class="sxs-lookup"><span data-stu-id="181ec-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="181ec-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="181ec-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="181ec-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="181ec-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="181ec-152">Java</span><span class="sxs-lookup"><span data-stu-id="181ec-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="181ec-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="181ec-153">Response</span></span>
><span data-ttu-id="181ec-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="181ec-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


