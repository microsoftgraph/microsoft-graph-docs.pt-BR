---
title: Atualizar orgcontact
description: Atualize as propriedades do objeto orgcontact.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 26396518b40023e7a4b5666fb1d00b4effd83546
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785239"
---
# <a name="update-orgcontact"></a><span data-ttu-id="86a5f-103">Atualizar orgcontact</span><span class="sxs-lookup"><span data-stu-id="86a5f-103">Update orgcontact</span></span>

<span data-ttu-id="86a5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86a5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86a5f-105">Atualize as propriedades do objeto orgcontact.</span><span class="sxs-lookup"><span data-stu-id="86a5f-105">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="86a5f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="86a5f-106">Permissions</span></span>
<span data-ttu-id="86a5f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86a5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86a5f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86a5f-109">Permission type</span></span>      | <span data-ttu-id="86a5f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86a5f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86a5f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86a5f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="86a5f-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86a5f-112">Not supported.</span></span>    |
|<span data-ttu-id="86a5f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86a5f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86a5f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86a5f-114">Not supported.</span></span>    |
|<span data-ttu-id="86a5f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86a5f-115">Application</span></span> | <span data-ttu-id="86a5f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86a5f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="86a5f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86a5f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="86a5f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86a5f-118">Request headers</span></span>
| <span data-ttu-id="86a5f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="86a5f-119">Name</span></span>       | <span data-ttu-id="86a5f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="86a5f-120">Type</span></span> | <span data-ttu-id="86a5f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="86a5f-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="86a5f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="86a5f-122">Authorization</span></span>  | <span data-ttu-id="86a5f-123">string</span><span class="sxs-lookup"><span data-stu-id="86a5f-123">string</span></span>  | <span data-ttu-id="86a5f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86a5f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86a5f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86a5f-126">Request body</span></span>
<span data-ttu-id="86a5f-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="86a5f-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="86a5f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86a5f-130">Property</span></span>     | <span data-ttu-id="86a5f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="86a5f-131">Type</span></span>   |<span data-ttu-id="86a5f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="86a5f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86a5f-133">city</span><span class="sxs-lookup"><span data-stu-id="86a5f-133">city</span></span>|<span data-ttu-id="86a5f-134">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-134">String</span></span>||
|<span data-ttu-id="86a5f-135">country</span><span class="sxs-lookup"><span data-stu-id="86a5f-135">country</span></span>|<span data-ttu-id="86a5f-136">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-136">String</span></span>||
|<span data-ttu-id="86a5f-137">department</span><span class="sxs-lookup"><span data-stu-id="86a5f-137">department</span></span>|<span data-ttu-id="86a5f-138">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-138">String</span></span>||
|<span data-ttu-id="86a5f-139">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="86a5f-139">onPremisesSyncEnabled</span></span>|<span data-ttu-id="86a5f-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="86a5f-140">Boolean</span></span>||
|<span data-ttu-id="86a5f-141">displayName</span><span class="sxs-lookup"><span data-stu-id="86a5f-141">displayName</span></span>|<span data-ttu-id="86a5f-142">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-142">String</span></span>||
|<span data-ttu-id="86a5f-143">givenName</span><span class="sxs-lookup"><span data-stu-id="86a5f-143">givenName</span></span>|<span data-ttu-id="86a5f-144">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-144">String</span></span>||
|<span data-ttu-id="86a5f-145">jobTitle</span><span class="sxs-lookup"><span data-stu-id="86a5f-145">jobTitle</span></span>|<span data-ttu-id="86a5f-146">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-146">String</span></span>||
|<span data-ttu-id="86a5f-147">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="86a5f-147">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="86a5f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86a5f-148">DateTimeOffset</span></span>||
|<span data-ttu-id="86a5f-149">email</span><span class="sxs-lookup"><span data-stu-id="86a5f-149">mail</span></span>|<span data-ttu-id="86a5f-150">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-150">String</span></span>||
|<span data-ttu-id="86a5f-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="86a5f-151">mailNickname</span></span>|<span data-ttu-id="86a5f-152">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-152">String</span></span>||
|<span data-ttu-id="86a5f-153">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="86a5f-153">mobilePhone</span></span>|<span data-ttu-id="86a5f-154">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-154">String</span></span>||
|<span data-ttu-id="86a5f-155">officeLocation</span><span class="sxs-lookup"><span data-stu-id="86a5f-155">officeLocation</span></span>|<span data-ttu-id="86a5f-156">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-156">String</span></span>||
|<span data-ttu-id="86a5f-157">postalCode</span><span class="sxs-lookup"><span data-stu-id="86a5f-157">postalCode</span></span>|<span data-ttu-id="86a5f-158">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-158">String</span></span>||
|<span data-ttu-id="86a5f-159">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="86a5f-159">proxyAddresses</span></span>|<span data-ttu-id="86a5f-160">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-160">String</span></span>||
|<span data-ttu-id="86a5f-161">estado</span><span class="sxs-lookup"><span data-stu-id="86a5f-161">state</span></span>|<span data-ttu-id="86a5f-162">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-162">String</span></span>||
|<span data-ttu-id="86a5f-163">streetAddress</span><span class="sxs-lookup"><span data-stu-id="86a5f-163">streetAddress</span></span>|<span data-ttu-id="86a5f-164">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-164">String</span></span>||
|<span data-ttu-id="86a5f-165">surname</span><span class="sxs-lookup"><span data-stu-id="86a5f-165">surname</span></span>|<span data-ttu-id="86a5f-166">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-166">String</span></span>||
|<span data-ttu-id="86a5f-167">businessPhones</span><span class="sxs-lookup"><span data-stu-id="86a5f-167">businessPhones</span></span>|<span data-ttu-id="86a5f-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="86a5f-168">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="86a5f-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="86a5f-169">Response</span></span>

<span data-ttu-id="86a5f-170">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="86a5f-170">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="86a5f-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86a5f-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86a5f-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86a5f-172">Request</span></span>
<span data-ttu-id="86a5f-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="86a5f-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="86a5f-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="86a5f-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_orgcontact"
}-->
```http
PATCH https://graph.microsoft.com/beta/contacts/{id}
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="86a5f-175">C#</span><span class="sxs-lookup"><span data-stu-id="86a5f-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86a5f-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86a5f-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86a5f-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86a5f-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="86a5f-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="86a5f-178">Response</span></span>
<span data-ttu-id="86a5f-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="86a5f-179">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update orgcontact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


