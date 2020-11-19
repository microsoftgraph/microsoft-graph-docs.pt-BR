---
title: Atualizar orgcontact
description: Atualize as propriedades do objeto orgcontact.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c425af3a39a2a9f13a46792d8482d59804c8d37f
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352148"
---
# <a name="update-orgcontact"></a><span data-ttu-id="a1af7-103">Atualizar orgcontact</span><span class="sxs-lookup"><span data-stu-id="a1af7-103">Update orgcontact</span></span>

<span data-ttu-id="a1af7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1af7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1af7-105">Atualize as propriedades do objeto orgcontact.</span><span class="sxs-lookup"><span data-stu-id="a1af7-105">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a1af7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1af7-106">Permissions</span></span>
<span data-ttu-id="a1af7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1af7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1af7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1af7-109">Permission type</span></span>      | <span data-ttu-id="a1af7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1af7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1af7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1af7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a1af7-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1af7-112">Not supported.</span></span>    |
|<span data-ttu-id="a1af7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1af7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1af7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1af7-114">Not supported.</span></span>    |
|<span data-ttu-id="a1af7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1af7-115">Application</span></span> | <span data-ttu-id="a1af7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1af7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1af7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1af7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a1af7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1af7-118">Request headers</span></span>
| <span data-ttu-id="a1af7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a1af7-119">Name</span></span>       | <span data-ttu-id="a1af7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1af7-120">Type</span></span> | <span data-ttu-id="a1af7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1af7-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a1af7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1af7-122">Authorization</span></span>  | <span data-ttu-id="a1af7-123">string</span><span class="sxs-lookup"><span data-stu-id="a1af7-123">string</span></span>  | <span data-ttu-id="a1af7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1af7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1af7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1af7-126">Request body</span></span>
<span data-ttu-id="a1af7-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a1af7-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a1af7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1af7-130">Property</span></span>     | <span data-ttu-id="a1af7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1af7-131">Type</span></span>   |<span data-ttu-id="a1af7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1af7-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1af7-133">city</span><span class="sxs-lookup"><span data-stu-id="a1af7-133">city</span></span>|<span data-ttu-id="a1af7-134">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-134">String</span></span>||
|<span data-ttu-id="a1af7-135">country</span><span class="sxs-lookup"><span data-stu-id="a1af7-135">country</span></span>|<span data-ttu-id="a1af7-136">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-136">String</span></span>||
|<span data-ttu-id="a1af7-137">department</span><span class="sxs-lookup"><span data-stu-id="a1af7-137">department</span></span>|<span data-ttu-id="a1af7-138">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-138">String</span></span>||
|<span data-ttu-id="a1af7-139">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="a1af7-139">onPremisesSyncEnabled</span></span>|<span data-ttu-id="a1af7-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1af7-140">Boolean</span></span>||
|<span data-ttu-id="a1af7-141">displayName</span><span class="sxs-lookup"><span data-stu-id="a1af7-141">displayName</span></span>|<span data-ttu-id="a1af7-142">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-142">String</span></span>||
|<span data-ttu-id="a1af7-143">givenName</span><span class="sxs-lookup"><span data-stu-id="a1af7-143">givenName</span></span>|<span data-ttu-id="a1af7-144">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-144">String</span></span>||
|<span data-ttu-id="a1af7-145">jobTitle</span><span class="sxs-lookup"><span data-stu-id="a1af7-145">jobTitle</span></span>|<span data-ttu-id="a1af7-146">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-146">String</span></span>||
|<span data-ttu-id="a1af7-147">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a1af7-147">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="a1af7-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1af7-148">DateTimeOffset</span></span>||
|<span data-ttu-id="a1af7-149">email</span><span class="sxs-lookup"><span data-stu-id="a1af7-149">mail</span></span>|<span data-ttu-id="a1af7-150">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-150">String</span></span>||
|<span data-ttu-id="a1af7-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="a1af7-151">mailNickname</span></span>|<span data-ttu-id="a1af7-152">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-152">String</span></span>||
|<span data-ttu-id="a1af7-153">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="a1af7-153">mobilePhone</span></span>|<span data-ttu-id="a1af7-154">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-154">String</span></span>||
|<span data-ttu-id="a1af7-155">officeLocation</span><span class="sxs-lookup"><span data-stu-id="a1af7-155">officeLocation</span></span>|<span data-ttu-id="a1af7-156">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-156">String</span></span>||
|<span data-ttu-id="a1af7-157">postalCode</span><span class="sxs-lookup"><span data-stu-id="a1af7-157">postalCode</span></span>|<span data-ttu-id="a1af7-158">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-158">String</span></span>||
|<span data-ttu-id="a1af7-159">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="a1af7-159">proxyAddresses</span></span>|<span data-ttu-id="a1af7-160">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-160">String</span></span>||
|<span data-ttu-id="a1af7-161">state</span><span class="sxs-lookup"><span data-stu-id="a1af7-161">state</span></span>|<span data-ttu-id="a1af7-162">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-162">String</span></span>||
|<span data-ttu-id="a1af7-163">streetAddress</span><span class="sxs-lookup"><span data-stu-id="a1af7-163">streetAddress</span></span>|<span data-ttu-id="a1af7-164">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-164">String</span></span>||
|<span data-ttu-id="a1af7-165">surname</span><span class="sxs-lookup"><span data-stu-id="a1af7-165">surname</span></span>|<span data-ttu-id="a1af7-166">String</span><span class="sxs-lookup"><span data-stu-id="a1af7-166">String</span></span>||
|<span data-ttu-id="a1af7-167">businessPhones</span><span class="sxs-lookup"><span data-stu-id="a1af7-167">businessPhones</span></span>|<span data-ttu-id="a1af7-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1af7-168">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="a1af7-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1af7-169">Response</span></span>

<span data-ttu-id="a1af7-170">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a1af7-170">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a1af7-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1af7-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1af7-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1af7-172">Request</span></span>
<span data-ttu-id="a1af7-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1af7-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1af7-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1af7-174">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a1af7-175">C#</span><span class="sxs-lookup"><span data-stu-id="a1af7-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1af7-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1af7-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1af7-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1af7-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a1af7-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1af7-178">Response</span></span>
<span data-ttu-id="a1af7-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1af7-179">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact"
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


