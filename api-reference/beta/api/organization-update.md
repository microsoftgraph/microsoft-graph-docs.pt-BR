---
title: Atualize a organização
description: Atualize as propriedades da organização autenticada no momento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 32a522b3ed8a21189f60ef68ce6990c2a7e78938
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346622"
---
# <a name="update-organization"></a><span data-ttu-id="f659b-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="f659b-103">Update organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f659b-104">Atualize as propriedades da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="f659b-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="f659b-105">Nesse caso, `organization` é definido como uma coleção de exatamente um registro e, portanto, sua **ID** deve ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="f659b-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="f659b-106">O **ID** também é conhecido como **tenantid** da organização.</span><span class="sxs-lookup"><span data-stu-id="f659b-106">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="f659b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f659b-107">Permissions</span></span>

<span data-ttu-id="f659b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f659b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f659b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f659b-110">Permission type</span></span> | <span data-ttu-id="f659b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f659b-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f659b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f659b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f659b-113">Organization. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="f659b-113">Organization.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="f659b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f659b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f659b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f659b-115">Not supported.</span></span> |
|<span data-ttu-id="f659b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f659b-116">Application</span></span> | <span data-ttu-id="f659b-117">Organization. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f659b-117">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f659b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f659b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f659b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f659b-119">Request headers</span></span>

| <span data-ttu-id="f659b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f659b-120">Name</span></span>       | <span data-ttu-id="f659b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f659b-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="f659b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f659b-122">Authorization</span></span>  | <span data-ttu-id="f659b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f659b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f659b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f659b-125">Content-Type</span></span>   | <span data-ttu-id="f659b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f659b-126">application/json</span></span> |


## <a name="request-body"></a><span data-ttu-id="f659b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f659b-127">Request body</span></span>

<span data-ttu-id="f659b-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f659b-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f659b-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f659b-131">Property</span></span>  | <span data-ttu-id="f659b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f659b-132">Type</span></span> |<span data-ttu-id="f659b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f659b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f659b-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="f659b-134">marketingNotificationEmails</span></span>|<span data-ttu-id="f659b-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f659b-135">String collection</span></span>|                                        <span data-ttu-id="f659b-136">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="f659b-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="f659b-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="f659b-137">privacyProfile</span></span>|[<span data-ttu-id="f659b-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="f659b-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="f659b-139">O perfil de privacidade de uma organização (definir statementUrl e contactEmail).</span><span class="sxs-lookup"><span data-stu-id="f659b-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="f659b-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="f659b-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="f659b-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f659b-141">String collection</span></span>||
|<span data-ttu-id="f659b-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="f659b-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="f659b-143">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f659b-143">String collection</span></span>||
|<span data-ttu-id="f659b-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="f659b-144">technicalNotificationMails</span></span>|<span data-ttu-id="f659b-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f659b-145">String collection</span></span>|                                        <span data-ttu-id="f659b-146">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="f659b-146">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="f659b-147">Como o recurso de **organização** oferece suporte a [extensões](/graph/extensibility-overview), você `PATCH` pode usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância de **organização** existente.</span><span class="sxs-lookup"><span data-stu-id="f659b-147">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="f659b-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f659b-148">Response</span></span>

<span data-ttu-id="f659b-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f659b-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f659b-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f659b-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f659b-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f659b-152">Request</span></span>
<span data-ttu-id="f659b-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f659b-153">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f659b-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="f659b-154">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f659b-155">C#</span><span class="sxs-lookup"><span data-stu-id="f659b-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f659b-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f659b-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f659b-157">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f659b-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f659b-158">Java</span><span class="sxs-lookup"><span data-stu-id="f659b-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f659b-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="f659b-159">Response</span></span>

<span data-ttu-id="f659b-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f659b-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="f659b-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="f659b-161">See also</span></span>

- [<span data-ttu-id="f659b-162">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="f659b-162">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f659b-163">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="f659b-163">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

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
