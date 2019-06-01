---
title: Atualize a organização
description: Atualize as propriedades da organização autenticada no momento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 37ea4cab912a9488a7974ca039bd25246ffadce6
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657823"
---
# <a name="update-organization"></a><span data-ttu-id="497c6-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="497c6-103">Update organization</span></span>

<span data-ttu-id="497c6-104">Atualize as propriedades da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="497c6-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="497c6-105">Nesse caso, `organization` é definido como uma coleção de exatamente um registro e, portanto, sua **ID** deve ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="497c6-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="497c6-106">O **ID** também é conhecido como **tenantid** da organização.</span><span class="sxs-lookup"><span data-stu-id="497c6-106">The **ID** is also known as the **tenantId** of the organization.</span></span>


## <a name="permissions"></a><span data-ttu-id="497c6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="497c6-107">Permissions</span></span>

<span data-ttu-id="497c6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="497c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="497c6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="497c6-110">Permission type</span></span> | <span data-ttu-id="497c6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="497c6-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="497c6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="497c6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="497c6-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="497c6-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="497c6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="497c6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="497c6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="497c6-115">Not supported.</span></span>    |
|<span data-ttu-id="497c6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="497c6-116">Application</span></span> | <span data-ttu-id="497c6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="497c6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="497c6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="497c6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}

```

## <a name="request-headers"></a><span data-ttu-id="497c6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="497c6-119">Request headers</span></span>

| <span data-ttu-id="497c6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="497c6-120">Name</span></span>       | <span data-ttu-id="497c6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="497c6-121">Type</span></span> | <span data-ttu-id="497c6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="497c6-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="497c6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="497c6-123">Authorization</span></span>  | <span data-ttu-id="497c6-124">string</span><span class="sxs-lookup"><span data-stu-id="497c6-124">string</span></span>  | <span data-ttu-id="497c6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="497c6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="497c6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="497c6-127">Request body</span></span>

<span data-ttu-id="497c6-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="497c6-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="497c6-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="497c6-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="497c6-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="497c6-130">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="497c6-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="497c6-131">Property</span></span>     | <span data-ttu-id="497c6-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="497c6-132">Type</span></span>   |<span data-ttu-id="497c6-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="497c6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="497c6-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="497c6-134">marketingNotificationEmails</span></span>|<span data-ttu-id="497c6-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="497c6-135">String collection</span></span>|                                        <span data-ttu-id="497c6-136">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="497c6-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="497c6-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="497c6-137">privacyProfile</span></span>|[<span data-ttu-id="497c6-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="497c6-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="497c6-139">O perfil de privacidade de uma organização (definir statementUrl e contactEmail).</span><span class="sxs-lookup"><span data-stu-id="497c6-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="497c6-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="497c6-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="497c6-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="497c6-141">String collection</span></span>||
|<span data-ttu-id="497c6-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="497c6-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="497c6-143">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="497c6-143">String collection</span></span>||
|<span data-ttu-id="497c6-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="497c6-144">technicalNotificationMails</span></span>|<span data-ttu-id="497c6-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="497c6-145">String collection</span></span>|                                        <span data-ttu-id="497c6-146">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="497c6-146">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="497c6-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="497c6-147">Response</span></span>

<span data-ttu-id="497c6-148">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="497c6-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="497c6-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="497c6-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="497c6-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="497c6-150">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="497c6-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="497c6-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="497c6-152">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="497c6-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="497c6-153">C#</span><span class="sxs-lookup"><span data-stu-id="497c6-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="497c6-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="497c6-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_organization-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
