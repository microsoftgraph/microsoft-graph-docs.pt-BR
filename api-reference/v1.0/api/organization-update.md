---
title: Atualize a organização
description: Atualize as propriedades da organização autenticada no momento.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9df86cb8b32b087952ce50bbd5e8c18aac6d3f1c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063020"
---
# <a name="update-organization"></a><span data-ttu-id="c0c1c-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="c0c1c-103">Update organization</span></span>

<span data-ttu-id="c0c1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0c1c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0c1c-105">Atualize as propriedades da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="c0c1c-105">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="c0c1c-106">Nesse caso, `organization` é definido como uma coleção de exatamente um registro e, portanto, sua **ID** deve ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0c1c-106">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="c0c1c-107">O **ID** também é conhecido como **tenantid** da organização.</span><span class="sxs-lookup"><span data-stu-id="c0c1c-107">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0c1c-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0c1c-108">Permissions</span></span>

<span data-ttu-id="c0c1c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0c1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0c1c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0c1c-111">Permission type</span></span> | <span data-ttu-id="c0c1c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0c1c-112">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0c1c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0c1c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c0c1c-114">Organization. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="c0c1c-114">Organization.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0c1c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0c1c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0c1c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0c1c-116">Not supported.</span></span>    |
|<span data-ttu-id="c0c1c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0c1c-117">Application</span></span> | <span data-ttu-id="c0c1c-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0c1c-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0c1c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0c1c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c0c1c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0c1c-120">Request headers</span></span>

| <span data-ttu-id="c0c1c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c0c1c-121">Name</span></span>       | <span data-ttu-id="c0c1c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0c1c-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="c0c1c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0c1c-123">Authorization</span></span>  | <span data-ttu-id="c0c1c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0c1c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0c1c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0c1c-126">Content-Type</span></span>   | <span data-ttu-id="c0c1c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c0c1c-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0c1c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0c1c-128">Request body</span></span>

<span data-ttu-id="c0c1c-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="c0c1c-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c0c1c-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="c0c1c-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c0c1c-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c0c1c-131">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c0c1c-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0c1c-132">Property</span></span>     | <span data-ttu-id="c0c1c-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0c1c-133">Type</span></span>   |<span data-ttu-id="c0c1c-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0c1c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0c1c-135">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="c0c1c-135">marketingNotificationEmails</span></span>|<span data-ttu-id="c0c1c-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0c1c-136">String collection</span></span>|                                        <span data-ttu-id="c0c1c-137">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="c0c1c-137">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="c0c1c-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="c0c1c-138">privacyProfile</span></span>|[<span data-ttu-id="c0c1c-139">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="c0c1c-139">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="c0c1c-140">O perfil de privacidade de uma organização (definir statementUrl e contactEmail).</span><span class="sxs-lookup"><span data-stu-id="c0c1c-140">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="c0c1c-141">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="c0c1c-141">securityComplianceNotificationMails</span></span>|<span data-ttu-id="c0c1c-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0c1c-142">String collection</span></span>||
|<span data-ttu-id="c0c1c-143">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="c0c1c-143">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="c0c1c-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0c1c-144">String collection</span></span>||
|<span data-ttu-id="c0c1c-145">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="c0c1c-145">technicalNotificationMails</span></span>|<span data-ttu-id="c0c1c-146">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0c1c-146">String collection</span></span>|                                        <span data-ttu-id="c0c1c-147">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="c0c1c-147">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="c0c1c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0c1c-148">Response</span></span>

<span data-ttu-id="c0c1c-149">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c0c1c-149">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c0c1c-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0c1c-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0c1c-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0c1c-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c0c1c-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0c1c-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/{id}
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
# <a name="c"></a>[<span data-ttu-id="c0c1c-153">C#</span><span class="sxs-lookup"><span data-stu-id="c0c1c-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0c1c-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0c1c-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0c1c-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0c1c-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0c1c-156">Java</span><span class="sxs-lookup"><span data-stu-id="c0c1c-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0c1c-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0c1c-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

