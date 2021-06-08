---
title: Atualize a organização
description: Atualize as propriedades da organização autenticada no momento.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cae41ed267ea4595134247cf1ac3967ce34141a5
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785927"
---
# <a name="update-organization"></a><span data-ttu-id="c1a40-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="c1a40-103">Update organization</span></span>

<span data-ttu-id="c1a40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1a40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1a40-105">Atualize as propriedades da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="c1a40-105">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="c1a40-106">Nesse caso, é definido como uma coleção de exatamente um registro e, portanto, sua ID deve ser `organization` especificada na  solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1a40-106">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="c1a40-107">A **ID** também é conhecida como **tenantId** da organização.</span><span class="sxs-lookup"><span data-stu-id="c1a40-107">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1a40-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="c1a40-108">Permissions</span></span>

<span data-ttu-id="c1a40-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1a40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1a40-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c1a40-111">Permission type</span></span> | <span data-ttu-id="c1a40-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c1a40-112">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1a40-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c1a40-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c1a40-114">Organization.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c1a40-114">Organization.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c1a40-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c1a40-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1a40-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c1a40-116">Not supported.</span></span> |
|<span data-ttu-id="c1a40-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c1a40-117">Application</span></span> | <span data-ttu-id="c1a40-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1a40-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1a40-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c1a40-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c1a40-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c1a40-120">Request headers</span></span>

| <span data-ttu-id="c1a40-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c1a40-121">Name</span></span>       | <span data-ttu-id="c1a40-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1a40-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="c1a40-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c1a40-123">Authorization</span></span>  | <span data-ttu-id="c1a40-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1a40-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1a40-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1a40-126">Content-Type</span></span>   | <span data-ttu-id="c1a40-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c1a40-127">application/json</span></span> |


## <a name="request-body"></a><span data-ttu-id="c1a40-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c1a40-128">Request body</span></span>

<span data-ttu-id="c1a40-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c1a40-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c1a40-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1a40-132">Property</span></span>  | <span data-ttu-id="c1a40-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1a40-133">Type</span></span> |<span data-ttu-id="c1a40-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1a40-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1a40-135">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="c1a40-135">marketingNotificationEmails</span></span>|<span data-ttu-id="c1a40-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1a40-136">String collection</span></span>|                                        <span data-ttu-id="c1a40-137">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="c1a40-137">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="c1a40-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="c1a40-138">privacyProfile</span></span>|[<span data-ttu-id="c1a40-139">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="c1a40-139">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="c1a40-140">O perfil de privacidade de uma organização (definir statementUrl e contactEmail).</span><span class="sxs-lookup"><span data-stu-id="c1a40-140">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="c1a40-141">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="c1a40-141">securityComplianceNotificationMails</span></span>|<span data-ttu-id="c1a40-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1a40-142">String collection</span></span>||
|<span data-ttu-id="c1a40-143">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="c1a40-143">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="c1a40-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1a40-144">String collection</span></span>||
|<span data-ttu-id="c1a40-145">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="c1a40-145">technicalNotificationMails</span></span>|<span data-ttu-id="c1a40-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1a40-146">String collection</span></span>|                                        <span data-ttu-id="c1a40-147">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="c1a40-147">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="c1a40-148">Como o **recurso da** organização dá suporte a extensões, você pode usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo em propriedades [personalizadas](/graph/extensibility-overview)de uma extensão em uma instância `PATCH` da **organização** existente.</span><span class="sxs-lookup"><span data-stu-id="c1a40-148">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="c1a40-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1a40-149">Response</span></span>

<span data-ttu-id="c1a40-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1a40-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1a40-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c1a40-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1a40-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c1a40-153">Request</span></span>
<span data-ttu-id="c1a40-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1a40-154">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c1a40-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1a40-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{id}
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```
# <a name="c"></a>[<span data-ttu-id="c1a40-156">C#</span><span class="sxs-lookup"><span data-stu-id="c1a40-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1a40-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1a40-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1a40-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1a40-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1a40-159">Java</span><span class="sxs-lookup"><span data-stu-id="c1a40-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c1a40-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="c1a40-160">Response</span></span>

<span data-ttu-id="c1a40-161">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c1a40-161">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="c1a40-162">Confira também</span><span class="sxs-lookup"><span data-stu-id="c1a40-162">See also</span></span>

- [<span data-ttu-id="c1a40-163">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="c1a40-163">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c1a40-164">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="c1a40-164">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


