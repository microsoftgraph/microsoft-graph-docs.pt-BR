---
title: Atualize a organização
description: Atualize as propriedades da organização autenticada no momento.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4968a1f686df8acfda23b283e99e42b56f90cb0a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975502"
---
# <a name="update-organization"></a><span data-ttu-id="b95b9-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="b95b9-103">Update organization</span></span>

<span data-ttu-id="b95b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b95b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b95b9-105">Atualize as propriedades da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="b95b9-105">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="b95b9-106">Nesse caso, `organization` é definido como uma coleção de exatamente um registro e, portanto, sua **ID** deve ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="b95b9-106">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="b95b9-107">O **ID** também é conhecido como **tenantid** da organização.</span><span class="sxs-lookup"><span data-stu-id="b95b9-107">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="b95b9-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b95b9-108">Permissions</span></span>

<span data-ttu-id="b95b9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b95b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b95b9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b95b9-111">Permission type</span></span> | <span data-ttu-id="b95b9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b95b9-112">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b95b9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b95b9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b95b9-114">Organization. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="b95b9-114">Organization.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b95b9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b95b9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b95b9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b95b9-116">Not supported.</span></span> |
|<span data-ttu-id="b95b9-117">Application</span><span class="sxs-lookup"><span data-stu-id="b95b9-117">Application</span></span> | <span data-ttu-id="b95b9-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b95b9-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b95b9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b95b9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b95b9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b95b9-120">Request headers</span></span>

| <span data-ttu-id="b95b9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b95b9-121">Name</span></span>       | <span data-ttu-id="b95b9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b95b9-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="b95b9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b95b9-123">Authorization</span></span>  | <span data-ttu-id="b95b9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b95b9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b95b9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b95b9-126">Content-Type</span></span>   | <span data-ttu-id="b95b9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b95b9-127">application/json</span></span> |


## <a name="request-body"></a><span data-ttu-id="b95b9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b95b9-128">Request body</span></span>

<span data-ttu-id="b95b9-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b95b9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b95b9-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b95b9-132">Property</span></span>  | <span data-ttu-id="b95b9-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="b95b9-133">Type</span></span> |<span data-ttu-id="b95b9-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="b95b9-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b95b9-135">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="b95b9-135">marketingNotificationEmails</span></span>|<span data-ttu-id="b95b9-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b95b9-136">String collection</span></span>|                                        <span data-ttu-id="b95b9-137">**Anotações** : não anulável.</span><span class="sxs-lookup"><span data-stu-id="b95b9-137">**Notes** : not nullable.</span></span>            |
|<span data-ttu-id="b95b9-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="b95b9-138">privacyProfile</span></span>|[<span data-ttu-id="b95b9-139">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="b95b9-139">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="b95b9-140">O perfil de privacidade de uma organização (definir statementUrl e contactEmail).</span><span class="sxs-lookup"><span data-stu-id="b95b9-140">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="b95b9-141">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="b95b9-141">securityComplianceNotificationMails</span></span>|<span data-ttu-id="b95b9-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b95b9-142">String collection</span></span>||
|<span data-ttu-id="b95b9-143">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="b95b9-143">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="b95b9-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b95b9-144">String collection</span></span>||
|<span data-ttu-id="b95b9-145">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="b95b9-145">technicalNotificationMails</span></span>|<span data-ttu-id="b95b9-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b95b9-146">String collection</span></span>|                                        <span data-ttu-id="b95b9-147">**Anotações** : não anulável.</span><span class="sxs-lookup"><span data-stu-id="b95b9-147">**Notes** : not nullable.</span></span>            |

<span data-ttu-id="b95b9-148">Como o recurso de **organização** oferece suporte a [extensões](/graph/extensibility-overview), você pode usar a `PATCH` operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância de **organização** existente.</span><span class="sxs-lookup"><span data-stu-id="b95b9-148">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="b95b9-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b95b9-149">Response</span></span>

<span data-ttu-id="b95b9-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b95b9-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b95b9-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b95b9-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b95b9-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b95b9-153">Request</span></span>
<span data-ttu-id="b95b9-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b95b9-154">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b95b9-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="b95b9-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b95b9-156">C#</span><span class="sxs-lookup"><span data-stu-id="b95b9-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b95b9-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b95b9-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b95b9-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b95b9-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b95b9-159">Java</span><span class="sxs-lookup"><span data-stu-id="b95b9-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b95b9-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="b95b9-160">Response</span></span>

<span data-ttu-id="b95b9-161">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b95b9-161">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="b95b9-162">Confira também</span><span class="sxs-lookup"><span data-stu-id="b95b9-162">See also</span></span>

- [<span data-ttu-id="b95b9-163">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="b95b9-163">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b95b9-164">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="b95b9-164">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

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


